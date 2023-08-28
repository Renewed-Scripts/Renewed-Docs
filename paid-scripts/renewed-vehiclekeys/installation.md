# 📃 Installation

### Step 1

* Head over to your ox\_inventory/data/items.lua and find ALL of your lockpick items
* This is normally lockpick and/or advanced lockpick, now add the following to the items

```lua
client = {
	event = 'lockpick:use'
}
```

Should end up looking like this

```lua
['lockpick'] = {
	label = 'Lockpick',
	weight = 160,
	client = {
		event = 'lockpick:use'
	}
},
```



### Step 2 (optional)

* Head over to ox\_inventory/data/items.lua and paste in this item

```lua
['vehiclekey'] = {
	label = 'Vehicle Key'
},
```

then head over to ox\_inventory/web/images.lua and put in the included from Renewed-Vehiclekeys



And that's it! Enjoy Renewed Vehicle Keys!
