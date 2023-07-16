# 📄 Installation

## Step 1

Run the sql file 'runme.sql'

## Step 2

Headover to ox\_inventory/data/items.lua and paste in these items. Adjust the weights etc. to your liking

```lua
['beehive'] = {
	label = 'Bee Hive',
	weight = 1000,
	client = {
		export = 'Renewed-Beekeeping.placeHive',
	}
},

['beewax'] = {
	label = 'Bee Wax',
	weight = 250
},

['emptyjar'] = {
	label = 'Empty Jar',
	weight = 50
},

['honeyjar'] = {
	label = 'Honey Jar',
	weight = 200
},
```

## Step 3

Headover to ox\_inventory/web/images and paste in the images from Renewed-Beekeeping/images



And that's it you are now ready to use Renewed Beekeeping
