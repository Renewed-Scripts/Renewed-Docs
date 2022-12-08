---
description: This page will give you a brief overlook on how to install this resource
---

# 📄 How to Install

### Step 1

* Download the latest version of Renewed-Chopshop from Keymaster and put ensure Renewed-Chopshop in your server.cfg
*   uncomment ox lib from the fxmanifest like shown below

    ```lua
    --'@ox_lib/init.lua'
    ```

### Step 2

* Headover to your qb-core/shared/items and paste in the following items. (Remember to remove images/ from \["image"] = if you're not using qb-businesses

```
-- Chop Shop --
['carpart_wheel']                  = {['name'] = 'carpart_wheel',                 ['label'] = 'Car Wheel',                 ['weight'] = 10000,         ['type'] = 'item',         ['image'] = 'images/carpart_wheel.png',         ['unique'] = false,     ['useable'] = false,     ['shouldClose'] = true,       ['combinable'] = nil,   ['description'] = 'A wheel from a vehicle'},
['carpart_door']                   = {['name'] = 'carpart_door',                  ['label'] = 'Car Door',                  ['weight'] = 15000,         ['type'] = 'item',         ['image'] = 'images/carpart_door.png',          ['unique'] = false,     ['useable'] = false,     ['shouldClose'] = true,       ['combinable'] = nil,   ['description'] = 'A door from a vehicle'},
['carpart_hood']                   = {['name'] = 'carpart_hood',                  ['label'] = 'Car Hood',                  ['weight'] = 15000,         ['type'] = 'item',         ['image'] = 'images/carpart_hood.png',          ['unique'] = false,     ['useable'] = false,     ['shouldClose'] = true,       ['combinable'] = nil,   ['description'] = 'A hood from a vehicle'},
['carpart_trunk']                  = {['name'] = 'carpart_trunk',                 ['label'] = 'Car Trunk',                 ['weight'] = 15000,         ['type'] = 'item',         ['image'] = 'images/carpart_trunk.png',         ['unique'] = false,     ['useable'] = false,     ['shouldClose'] = true,       ['combinable'] = nil,   ['description'] = 'A trunk from a vehicle'},
```

* and then head to your qb-inventory/html/images and paste in the images your recieved from me in the download.

### Step 3

* Head over to Renewed-Weaponscarry and paste in the following lines under local props

```
["carpart_hood"]               = { carry = true,   model = "imp_prop_impexp_bonnet_02a",   bone = 24817, x = 0.30, y = 0.40, z = 0.15, xr = 0.0, yr = -90.0,  zr = 280.0, blockAttack = true, blockCar = true, blockRun = true},
["carpart_trunk"]              = { carry = true,   model = "imp_prop_impexp_bonnet_02a",   bone = 24817, x = 0.30, y = 0.40, z = 0.15, xr = 0.0, yr = -90.0,  zr = 280.0, blockAttack = true, blockCar = true, blockRun = true},
["carpart_door"]               = { carry = true,   model = "imp_prop_impexp_car_door_04a", bone = 24817, x = 0.90, y = 0.50, z = 0.15, xr = 0.0, yr = -200.0, zr = 280.0, blockAttack = true, blockCar = true, blockRun = true},
["carpart_wheel"]              = { carry = true,   model = "v_ind_cm_tyre04",              bone = 24817, x = 0.20, y = 0.50, z = 0.05, xr = 0.0, yr = -180.0, zr = 280.0, blockAttack = true, blockCar = true, blockRun = true},
```
