---
description: These are all the client side Functions
---

# Functions

Import the Lib by using this export as you would with a normal core

```lua
local Renewed = exports['Renewed-Lib']:getLib()
```



This will return a table with all the players current job/gang(s).

```lua
local groups = Renewed.getPlayerGroup()

print(json.encode(groups))
```



Spawning a ped has never been easier, you can utilize this function to spawn peds that will automatically spawn/despawn when not in distance

```lua
Renewed.addPed({ 
    model = `a_f_y_business_01`, -- The ped to be spawned
    dist = 300, -- Distance of when the ped should be loaded in
    coords = vec3(-596.54, -1096.99, 22.18), -- The coords for the ped
    heading = 308.0, -- Heading of the ped
    scenario = false, -- Use this if you want the ped to play a scenario
    freeze = true, -- use this if the ped should be frozen
    invincible = true, -- use this if the ped should be invincible 
    tempevents = true,-- use this if the ped should block temporary events
    id = 'brandNewPed_323', -- Unique ID for the ped
    
    -- Normal ox Target stuff --
    target = {
        {
            name = 'brandNewPed_323',
            icon = 'fas fa-shopping-basket',
            label = 'View Shop',
            event = 'Renewed-Businesses:client:openStore',
            id = 'brandNewShopLol',
            canInteract = function(_, distance)
                return distance < 1.5
            end,
        }
    }
})
```



