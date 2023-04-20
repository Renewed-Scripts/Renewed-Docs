---
description: How to add / remove items from the built in Ingredient Shops
---

# 🥔 Ingredient shop

## How to create a new Ingredient Shop

* Head over to Renewed-Businesses/Config.lua
* Find Config.IngredientShops
* Here you can add a new shop like this.

```lua
['example'] = { -- the 'example' is the key for the shop, which is used in ox_inv
    name = 'Example Shop', -- This is the name of the shop and Blip

    blip = { -- Blip Settings
        id = 52,
        colour = 4,
        scale = 0.6
    },

    locations = { -- Location can be 1 or more
        vector4(53.13, -1479.35, 28.28, 184.05),
    },

    pedModel = `mp_m_shopkeep_01` -- ped model
},
```

## How to add items to a ingredient shop

* Head over to ox\_inventory/data/items.lua
* Here you can find a random item like this&#x20;

```lua
['radio'] = {
	label = 'Radio',
	weight = 1000,
	stack = false,
	allowArmed = true
},
```

* Now we can add shopType = 'example' to add it add it to the example shop, and price = 10, to make it cost $10

```lua
['radio'] = {
	label = 'Radio',
	weight = 1000,
	stack = false,
	allowArmed = true,
	shopType = 'example',
	price = 10
},
```

## Removing items from ingredient shops

* Head over to ox\_inventory/data/items.lua
* find an item that has shopType = 'example' and price = 10 or anything like this

```lua
['radio'] = {
	label = 'Radio',
	weight = 1000,
	stack = false,
	allowArmed = true,
	shopType = 'example',
	price = 10
},
```

* Now remove the shopType and price so it looks like this

```lua
['radio'] = {
	label = 'Radio',
	weight = 1000,
	stack = false,
	allowArmed = true,
},
```

* and that is it you have now removed 'radio' from shop 'example'
