---
description: This page will give you a brief overlook on how to install this resource
---

# 📄 How to Install

{% hint style="info" %}
Make sure to follow all steps step by step, if you encounter errors please recheck that you've completed step 1-5 correctly.
{% endhint %}

### Step 1

* Open Renewed-Fuel folder and run the SQL on your database.

### Step 2

* Remove LegacyFuel or any other Fuel Script you used prior
* Insert Renewed-Fuel into your server
* Remember to Ensure Renewed-Fuel in your server.cfg

### Step 3 (Optional if you used ps/cdn/qb/jl/Legacy Fuel)

* Open your Entire server in Visual Studio Code
* Now do a folder search for LegacyFuel (Or any other fuel script you used prior)
* Now Replace it with **Renewed-Fuel**

### Step 4

* Now open ox\_inventory and insert the following items into ox\_inventory/data/items.lua

```lua
oilbarrel = {
	label = 'Oil Barrel',
	stack = false,
	weight = 0,
},

driveshaft = {
	label = 'Drive Shaft',
	weight = 1000,
	stack = false
},

oilfilter = {
	label = 'Oil Filter',
	weight = 1000,
	stack = false
},

reliefstring = {
	label = 'Relief String',
	weight = 1000,
	stack = false
},

skewgear = {
	label = 'Skew Gear',
	weight = 1000,
	stack = false
},

timingchain = {
	label = 'Timing Chain',
	weight = 1000,
	stack = false
},
```

* now insert the images from Renewed-Fuel into ox\_inventory/web/images folder.

### Step 5 (optional)

* If you want to use native audio for when picking/putting nozzles and fueling vehicles download this resource: [https://github.com/Renewed-Scripts/Renewed-Audiobank](https://github.com/Renewed-Scripts/Renewed-Audiobank)
* Make sure to start it in the server.cfg before Renewed-Fuel



### Step 6 (optional)

* If you want players to be able to purchase stations without admin intervention add this to your server.cfg

```properties
# Make fuel stations purchaseable by players
setr fuel_buystations true
```

And that is all for installation!

