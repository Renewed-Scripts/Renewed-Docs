---
description: All the following exports are SERVER SIDED ONLY
---

# 👨❤👨 Group Exports

{% hint style="info" %}
Here you can find all exports related to Groups within the phone!
{% endhint %}

## Utility Exports

### NotifyGroup

```
This export is used to notify the entire group about specific objectives or events.

-- STOCK EXPORT -- 
exports['qb-phone']:NotifyGroup(group, msg, type)

-- PARAMETERS --
- group (string): The identifier of the group.
- message (string): The message to be sent to the group.
- type (string): The type of notification.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(source)
exports['qb-phone']:NotifyGroup(group, "Hey cuties :)", 'success')

```

### pNotifyGroup

```
This export is used to notify the entire group about a specific objective, utilizing the built-in Phone notification type.

(Uses the build in Phone notification type)

Find the colour codes here:
https://htmlcolorcodes.com/

Find the icons you can use for the phone here:
https://fontawesome.com/v5/search?o=r&m=free

-- Stock Export -- 
exports['qb-phone']:pNotifyGroup(group, header, msg, icon, colour, length)

-- PARAMETERS --
- group (string): The identifier of the group.
- header (string): The header/title of the notification.
- msg (string): The detailed message for the notification.
- icon (string): The icon for the notification (FontAwesome icon class).
- color (string or number): The color of the notification.
- length (number): The duration of the notification in milliseconds.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(source)
local message = "Head to the location marked and pick up trash!"
exports['qb-phone']:pNotifyGroup(group, "Garbage Job", msg, "fas fa-recycle", "#008FFF", 7500)
```

### CreateBlipForGroup

```
An export to make blips that sync across group members.

find all the FiveM related blip data you will need for this here:
https://docs.fivem.net/docs/game-references/blips/

-- Stock Export -- 
exports['qb-phone']:CreateBlipForGroup(group, name, data)

-- PARAMETERS --
- group (string): The identifier of the group.
- name (string): The name/identifier for the blip.
- data (table): The data table containing blip details.

-- USAGE --
Do not copy paste this as the blip table might be broken only this as a reference

local group = exports['qb-phone']:GetGroupByMembers(src)
local blip = {
    -- NOTE YOU CAN ONLY USE ONE OF ENTITY NETID RADIUS AS THEY ALL DO THE SAME
    -- Picking none of these 3 will make it a normal blip by default
    entity = 9421, -- Use this if you have an entity spawned server side
    netId = 9421, -- Use this if you have a entity server side and you have the netId
    radius = 200, -- How big do you want the radius of the blip to be
    
    coords = vector4(231, 244, 92, 1.41) -- Just the coords for the blip
    color = 49, -- just a red colour
    alpha = 255, -- This makes the blip kinda see through if u lower it
    sprite = 57, -- Just a circle icon,
    scale = 0.7, -- How big do u want the blip to be?
    label = "Garbage Route", -- The label for the blip
    
    -- Route stuff --
    route = true, -- Will set a route for the job (Note a route is not a waypoint they cant remove it)
    routeColor = 49, -- just a red to finish off the routeColor
}

exports['qb-phone']:CreateBlipForGroup(group, "Garbage", blip)
```

### RemoveBlipForGroup

```
An export to remove blips across all group members

-- Stock Export -- 
exports['qb-phone']:RemoveBlipForGroup(group, name)

-- PARAMETERS --
- group (string): The identifier of the group.
- name (string): The name/identifier for the blip to be removed.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
exports['qb-phone']:RemoveBlipForGroup(group, "Garbage")
```

## Job Status

All exports used to modify or get the group current job statuses, you wanna use this to AVOID groups doing 2 jobs at the same time etc.

### setJobStatus

```
An export to set the groups job to something specific.

-- Stock Export -- 
exports['qb-phone']:setJobStatus(group, status, stages)

-- PARAMETERS --
- group (string): The identifier of the group.
- status (string): The name/identifier of the job status.
- stages (table): A table containing stages for the job.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
local Stages = {
    [1] = {name = "Head to the area located on your GPS", isDone = false , id = 1},
    [2] = {name = "Find the vehicle I emailed you!", isDone = false , id = 2},
    [3] = {name = "Head to the scrapping location marked on your GPS!", isDone = false , id = 3},
    [4] = {name = "Dissasemble the vehicle for parts!", isDone = false , id = 4},
    [5] = {name = "Break down the rest of the car to get rid of the evidence!", isDone = false , id = 4},
    [6] = {name = "Get out of there before you get seen!", isDone = false , id = 5},
}

exports['qb-phone']:setJobStatus(group, "Chop Shop", Stages)
```

### getJobStatus

```
An export to get the current job the group is doing

-- Stock Export -- 
exports['qb-phone']:getJobStatus(group)

-- PARAMETERS --
- group (string): The identifier of the group.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
local job = exports["qb-phone"]:getJobStatus(group)
print(job) -- If you followed above step it will print Chop Shop
```

### resetJobStatus

```
An export to reset the current groups job status to be WAITING.

-- Stock Export -- 
exports['qb-phone']:resetJobStatus(group)

-- PARAMETERS --
- group (string): The identifier of the group.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
exports["qb-phone"]:resetJobStatus(group)
```

## Core Exports

These are the type of exports you are going to be using most frequently and cannot make a group job WITHOUT

### GetGroupByMembers

```
An export to get the players current group.
If the player has no group it will return nil.

-- Stock Export -- 
exports['qb-phone']:GetGroupByMembers(src)

-- PARAMETERS --
- src (number): The source ID of the player.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
print(group) -- Will either print the group ID or print nil.
```

### getGroupMembers

```
An export to get all the group members source ID

-- Stock Export -- 
exports['qb-phone']:getGroupMembers(group)

-- PARAMETERS --
- group (string): The identifier of the group.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
local members = exports['qb-phone']:getGroupMembers(group)
print(json.encode(members)) -- Will print the table for the group members
```

### getGroupSize

```
An export to ge the current group size.

This can be used if u want players to be a specific number to start a job.

-- Stock Export -- 
exports['qb-phone']:getGroupSize(group)

-- PARAMETERS --
- group (string): The identifier of the group.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
local size = exports['qb-phone']:getGroupSize(group)

print(size) -- Will print how many people are in the group
```

### GetGroupLeader

```
An export to get the current groups leader

This can be used to make sure only the group leader can start a job.

-- Stock Export -- 
exports['qb-phone']:GetGroupLeader(group)

-- PARAMETERS --
- group (string): The identifier of the group.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
local leader = exports['qb-phone']:GetGroupLeader(group)

print(leader) -- Will print the group leader source ID
```

### isGroupLeader

```
An export to check if a player is the group leader

-- Stock Export -- 
exports['qb-phone']:isGroupLeader(group)

-- PARAMETERS --
- src (number): The source ID of the player.
- group (string): The identifier of the group.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
local leader = exports['qb-phone']:isGroupLeader(src, group)

print(leader) -- Will print true if the source ID is the group leader
```

### DestroyGroup

```
An export to destroy a group.

-- Stock Export -- 
exports['qb-phone']:DestroyGroup(group)

-- PARAMETERS --
- group (string): The identifier of the group.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
exports['qb-phone']:DestroyGroup(group)
```

### RemovePlayerFromGroup

```
An export to remove a certain player based off their sourceID from a group

-- Stock Export -- 
exports['qb-phone']:RemovePlayerFromGroup(src, group)

-- PARAMETERS --
- src (number): The source ID of the player.
- group (string): The identifier of the group.

-- USAGE --
local group = exports['qb-phone']:GetGroupByMembers(src)
exports['qb-phone']:RemovePlayerFromGroup(src, group)

In this case I removed the sourceID here from their current group
```

## Additional NetEvents

```
This eventhandler here can be used to remove groups from server sided events.

Usefull to avoid glithces and bugs if someone crashes etc.

AddEventHandler('qb-phone:server:GroupDeleted', function(group, players)
    -- Parameters:
    --   - group (string): The identifier of the deleted group.
    --   - players (table): A table containing the source IDs of players in the deleted group.
    
    -- Perform server-side cleanup or adjustments based on the deleted group.
    print(group, json.encode(players))
end)
```
