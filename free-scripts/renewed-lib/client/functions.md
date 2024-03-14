---
description: These are all the client side Functions
---

# Functions

Import the Lib by using this export as you would with a normal core

```lua
local Renewed = exports['Renewed-Lib']:getLib()
```



### getPlayerGroup()

```lua

-- @brief This will return a table with the player's current job/gang(s)
-- @return table containing the player's current job/gang(s)
Renewed.getPlayerGroup()

-- USAGE --

local groups = Renewed.getPlayerGroup()

print(json.encode(groups))

-- OUTPUT --
{
    Group = {
        ['mechanic'] = 4,
        ['ballas'] = 2
    },
    job = 'mechanic',
    gang = 'ballas',
    charId = 'QB245361',
    name = 'Test Player'
}
```


### getCharId()

```lua

-- @brief This will return the player's character ID
-- @return the player's character ID
Renewed.getCharId()

-- USAGE --

local charId = Renewed.getCharId()

print(charId)

-- OUTPUT --
'QB245361'
```



### addObject()
```lua

-- @brief Adds an object that will auto spawn/despawn
--
-- Adding objects has never been easier.  You can utilize this function to add
-- objects in the world that will spawn/despawn when in/out of distance.
--
-- @param payload [in]  A table containing the following information:
--   - object (hash): The hash of the object to be loaded
--   - dist (int): The distance at which the object will spawn
--   - coords (vector): A vector of the coordinates for initial placement
--   - heading (float): The heading of the initial placement
--   - snapGrount (boolean): Use this to snap the object to the ground
--   - freeze (boolean): Use this to freeze the object in place
--   - canClimb (boolean): Use this to specify if players can climb on the object
--   - colissions (boolean): Use this to change if the object can collide
--   - anim (list): A list containing the animation and dictionary for the object
--   - animSpeed (float): The speed of the animation for the object
--   - id (string): A unique ID for your object
--   - target (table): A table containing ox target parameters
--   - interact (table): A table containing interact parameters
Renewed.addObject(payload)

-- USAGE --
Renewed.addObject({
    object = `prop_weed_01`,
    dist = 300,
    coords = vec3(-596.54, -1096.99, 22.18),
    heading = 308.0,
    snapGround = true,
    freeze = true,
    canClimb = true,
    colissions = true,
    anim = {
        'amb@world_human_gardener_plant@male@base',
        'base'
    },
    animSpeed = 1.0,
    id = 'brandNewObject_323'
    target = {
        {
            name = 'brandNewPed_323',
            icon = 'fas fa-cannabis',
            label = 'Harvest',
            event = 'weed:client:harvest',
            id = 'brandNewObjectLol',
            canInteract = function(_, distance)
                return distance < 1.5
            end,
        }
    }
})
```



### changeObject()

```lua

-- @brief Changes an object model, its location, and heading
--
-- @param id (string): The unique ID of the object you created
-- @param newObject (string): The name of the new model to use
-- @param newCoords (vector): A vector containing the new coordinates to use
-- @param newHeading (float): The new heading to use
Renewed.changeObject(id, newObject, newCoords, newHeading)

-- USAGE --
Renewed.changeObject('brandNewObject_323', `prop_weed_02`, vec3(100, 50, 50), 120.0)
```



### changeAnim()

```lua
-- @brief Changes an object's animation
--
-- @param id (string): The unique ID of the object you created
-- @param anim (list): A list containing the dictionary and animation for the object
-- @param animSpeec (float): The animation speed
Renewed.changeAnim(id, anim, animSpeed)

-- USAGE --
Renewed.changeAnim('brandNewObject_323', {"amb@world_human_gardener_plant@female@base",
    "base"}, 0.8)
```



### removeObject()
```lua

-- @brief Removes an object from being created
--
-- @param id (string): The unique ID of the object you created
Renewed.removeObject(id)

-- USAGE --
Renewed.removeObject('brandNewObject_323')
```



### removeResourceObj()
```lua

-- @brief Removes all objects created by the invoking resource
--
-- @param resource (string or nil): The name of the invoking resource
Renewed.removeResourceObj(resource)

-- USAGE --
Renewed.removeResourceObj('my-resource-name')
```



### placeObject()
```lua

-- @brief Allows a player to interactively place an object
--
-- Placing objects has never been easier.  You can utilize this funciton to place
-- objects that will automatically spawn/despawn when in/out of range.
--
-- @param object (hash): The hash of the object to be placed
-- @param dist (int): The distance at which the object will spawn
-- @param snapGround (boolean or nil): Whether or not to snap the object to the ground
-- @param text (list or nil): A list containing help text
-- @param allowedMats (list or nil): A list containing the allowed materials that the
--        object can be on
-- @param offset (float or table or nil): The offset to use from the coordinates
-- @return A list containing the object coords and heading
Renewed.placeObject(object, dist, snapGround, text, allowedMats, offset)

-- USAGE --
local coords, heading = Renewed.placeObject('prop_weed_01', 300, true, {
        '-- Place Object --  \n',
        '[E] Place  \n',
        '[X] Cancel  \n',
        '[SCROLL UP] Change Heading  \n',
        '[SCROLL DOWN] Change Heading'
    }, {
        ['concrete'] = true,
        ['plastic'] = true
    }, {
        x = 0.0,
        y = 0.0,
        z = 0.0
    })

Renewed.addObject({
    object = `prop_weed_01`,
    dist = 300,
    coords = coords,
    heading = heading,
    snapGround = true,
    freeze = true,
    canClimb = true,
    colissions = true,
    anim = {
        'amb@world_human_gardener_plant@male@base',
        'base'
    },
    animSpeed = 1.0,
    id = 'brandNewObject_323'
    target = {
        {
            name = 'brandNewPed_323',
            icon = 'fas fa-cannabis',
            label = 'Harvest',
            event = 'weed:client:harvest',
            id = 'brandNewObjectLol',
            canInteract = function(_, distance)
                return distance < 1.5
            end,
        }
    }
})
```



### stopPlacing()
```lua

-- @brief Stops a player from placing an object
Renewed.stopPlacing()

-- USAGE --
Renewed.stopPlacing()
```



### addPed()

```lua

-- @brief Creates a ped that automatically deletes when out of range
--
-- Spawning a ped has never been easier.  You can utilize this function to spawn
-- peds that will automatically spawn/despawn when in/out of distance.
--
-- @param [in] payload  A table with the following information:
--   - model (hash): The hash of the model to be loaded
--   - dist (int): The distance at which the ped will spawn
--   - coords (vector): A vector of the coordinates for the ped
--   - heading (float): The heading of the ped
--   - freeze (boolean): Use this to freeze the ped
--   - invincible (boolean): Use this to make the ped invincible
--   - tempevents (boolean): Use this to make the ped block temporary events
--   - animDict (string): The animation dictionary to use for the ped (required if
--                        you are using animName)
--   - animName (string): The name of the animation to use for the ped
--   - scenario (boolean or string): The scenario to use for the ped
--   - id (string): A unique ID for your ped
--   - target (table): A table containing ox target parameters
--   - interact (table): A table containing interact parameters
Renewed.addPed(payload)

-- USAGE --

Renewed.addPed({ 
    model = `a_f_y_business_01`,
    dist = 300,
    coords = vec3(-596.54, -1096.99, 22.18),
    heading = 308.0,
    freeze = true,
    invincible = true,
    tempevents = true,
    animDict = 'anim@mp_player_intcelebrationfemale@the_woogie',
    animName = 'the_woogie',
    scenario = false,
    id = 'brandNewPed_323',
    
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



### removePed()
```lua

-- @brief Deletes a ped
--
-- This will delete a ped by ID specified with invoking Renewed.addPed()
--
-- @param id (string): The ID specified when creating the ped
Renewed.removePed(id)

-- USAGE --
Renewed.removePed('brandNewPed_323')
```



### setPedCoords()
```lua

-- @brief Sets the coordinates of a ped
--
-- This will change/update the coordinates of a ped created by addPed()
--
-- @param id (string): The ID specified when creating the ped
-- @param coords (vector): The new coords for the ped
-- @param heading (float): The new heading for the ped
Renewed.setPedCoords(id, coords, heading)

-- USAGE --
Renewed.setPedCoords('brandNewPed_323', vec3(150, 50, 50), 120.0)
```



### getPedById()

```lua

-- @brief Returns the ped's entity ID
--
-- This funciton will return the entity ID of a ped's unique ID that was created by
-- addPed()
--
-- @param id (string): The ID specified when creating the ped
-- @return The entity ID of the ped or nil if not spawned
Renewed.getPedById(id)

-- USAGE --
local ped = Renewed.getPedById('brandNewPed_323')

print(ped)
```
