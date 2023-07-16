# 📄 Installation

## Step 1

Run the sql file 'runme.sql'

## Step 2

Head over to ox\_inventory/data/items.lua and paste in these items. Adjust the weights etc. to your liking

```lua
['beehive'] = {
	label = 'Bee Hive',
	weight = 1000,
	description = 'A wooden beehive used for beekeeping. Handle with care!',
	client = {
		export = 'Renewed-Beekeeping.placeHive',
	}
},

['beewax'] = {
	label = 'Bees Wax',
	weight = 250,
	description = 'Pure, golden beeswax obtained from beehives. It has various uses.',
},

['emptyjar'] = {
	label = 'Empty Jar',
	weight = 50,
	description = 'A glass jar with no contents. Can be used for storage or crafting.',
},

['honeyjar'] = {
	label = 'Honey Jar',
	weight = 200,
	description = 'A jar filled with delicious, golden honey. A sweet treat!',
},
```

## Step 3

Head over to ox\_inventory/web/images and paste in the images from Renewed-Beekeeping/images



And that's it you are now ready to use Renewed Beekeeping
