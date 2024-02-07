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

['dryingrack'] = {
	label = 'Drying Rack',
	weight = 2500,
	consume = 0,
	server = {
		export = 'Renewed-Weed.placeDryingRack'
	}
},

['dryingrackadvanced'] = {
	label = 'Advanced Drying Rack',
	weight = 5000,
	consume = 0,
	server = {
		export = 'Renewed-Weed.placeDryingRack'
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

* Run the SQL file inside of Renewed-Weed!

That is it for installing the Weed System! the rest is drag and drop hope you enjoy!
