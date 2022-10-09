---
description: This page will give you a brief overlook on how to install this resource
---

# 📄 How to install

{% hint style="info" %}
Utilize this section if you have trouble installing the script

Step 3 can be skipped if u do not wish to use material vouchers
{% endhint %}

### Step 1

* Download the latest version of the script from your keymaster

### Step 2

* Put it in your server directory somewhere

### Step 3

* Add the following to your qb-core/shared/items.lua

```lua
['matticket']					 = {['name'] = 'matticket', 					['label'] = 'Material Voucher',			 ['weight'] = 100, 		['type'] = 'item', 		['image'] = 'matticket.png', 			['unique'] = false,		['useable'] = false, 	['shouldClose'] = false,	   ['combinable'] = nil,   ['description'] = 'Turn this in at sanitation to be rewarded with some scrapped material',
```

* Now head over to your inventory and put in the matticket.png to your qb-inventory/html/images folder

### Step 4

* Now head over to your qb-core/server/player.lua and add the following to your PlayerData

```lua
PlayerData.metadata['garbage'] = PlayerData.metadata['garbage'] or 0
```

### Step 5

* Put ensure Renewed-Garbage in your server.cfg and thats it! ENJOY



