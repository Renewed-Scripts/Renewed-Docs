---
description: >-
  Here you will get a brief and precise tutorial on how to install Renewed Weed
  for your server!
---

# 📄 Installation

### Step 1

* Head over to ox\_inventor/data/items.lua and apste the following items in!

```lua
['female_seed'] = {
	label = 'Female Seed',
	weight = 1,
	client = {
		export = 'Renewed-Weed.placeWeed',
		image = 'weed_seed.png'
	}
},

['male_seed'] = {
	label = 'Male Seed',
	weight = 1,
	client = {
		image = 'weed_seed.png'
	}
},

['wetweed'] = {
	label = 'Wet Bud',
	weight = 0,
	decay = true,
	degrade = 1200, -- 20 hours
},

['driedweed'] = {
	label = 'Dry Bud',
	weight = 50,
	buttons = {
		{
			label = 'Make into a brick',
			action = function(slot)
				exports['Renewed-Weed']:makeBrick(slot)
			end
		}
	}
},

['weedbrick'] = {
	label = 'Weed Brick',
	weight = 0,
},

['joint'] = {
	label = 'Joint',
	weight = 25,
},

['emptybag'] = {
	label = 'Empty Bag',
	weight = 5,
},

['fullbag'] = {
	label = 'Bag of Weed',
	description = 'A 3 oz bag of weed',
	weight = 55,
},

['wateringcan'] = {
	label = 'Watering Can',
	weight = 0,
},

['fertilizer'] = {
	label = 'Fertilizer',
	weight = 1500,
},

['scale'] = {
	label = 'Fertilizer',
	weight = 1500,
},
```

### Step 2

* Copy the images inside Renewed-Weed/images and paste them into ox\_inventory/web/images



### Step 3

*   Headover to ox\_inventory/modules/inventory/server.lua and find the function&#x20;

    ```lua
    local function prepareInventorySave(inv, buffer, time)
    ```
* now replace that ENTIRE function with this

```lua
local function prepareInventorySave(inv, buffer, time)
    local shouldSave = not inv.datastore and inv.changed
    local n = 0

    for k, v in pairs(inv.items) do
		local decayed, newItem = Items.UpdateDurability(inv, v, Items(v.name), nil, time)

        if (not decayed or decayed and newItem) and shouldSave then
            n += 1
            buffer[n] = {
                name = newItem and newItem.name or v.name,
                count = newItem and newItem.count or v.count,
                slot = k,
                metadata = newItem and next(newItem.metadata) and newItem.metadata or next(v.metadata) and v.metadata or nil
            }
        end
	end

    if not shouldSave then return end

    local data = next(buffer) and json.encode(buffer) or nil
    inv.changed = false
    table.wipe(buffer)

    if inv.player then
        if shared.framework == 'esx' then return end

        return 1, { data, inv.owner }
    end

    if inv.type == 'trunk' then
        return 2, { data, inv.dbId }
    end

    if inv.type == 'glovebox' then
        return 3, { data, inv.dbId }
    end

    return 4, { data, inv.owner and tostring(inv.owner) or '', inv.dbId }
end
```

### Step 3

* Headover to ox\_inventory/items/server.lua around line 418 and find this function

```lua
function Items.UpdateDurability(inv, slot, item, value, ostime)
    local durability = slot.metadata.durability

    if not durability then return end

    if value then
        durability = value
    elseif ostime and durability > 100 and ostime >= durability then
        durability = 0
    end

    if item.decay and durability == 0 then
        return Inventory.RemoveItem(inv, slot.name, slot.count, nil, slot.slot)
    end

    if slot.metadata.durability == durability then return end

    inv.changed = true
    slot.metadata.durability = durability

    inv:syncSlotsWithClients({
        {
            item = slot,
            inventory = inv.id
        }
    }, { left = inv.weight }, true)
end
```

Then replace that function with this

```lua
function Items.UpdateDurability(inv, slot, item, value, ostime)
    local durability = slot.metadata.durability or value

    if not durability then return end

    if value then
        durability = value
    elseif ostime and durability > 100 and ostime >= durability then
        durability = 0
    end

	if item.decay and durability == 0 then
		local success = Inventory.RemoveItem(inv, slot.name, slot.count, nil, slot.slot)
		local newItem

		if success and slot.name == 'wetweed' then
			local weight = slot.metadata?.weight or 100
			local amount = math.floor(weight / 100)
			success = Inventory.AddItem(inv, 'driedweed', amount, { strain = slot.metadata?.strain, strainQuality = slot.metadata?.strainQuality }, slot.slot)
			newItem = {name = 'driedweed', count = amount, metadata = { strain = slot.metadata?.strain, strainQuality = slot.metadata?.strainQuality }}
		end

		return success, newItem
    end

    if slot.metadata.durability == durability then return end

    inv.changed = true
    slot.metadata.durability = durability

    inv:syncSlotsWithClients({
        {
            item = slot,
            inventory = inv.id
        }
    }, true)
end
```

### Step 4

* Run the SQL file inside of Renewed-Weed!

That is it for installing the Weed System! the rest is drag and drop hope you enjoy!
