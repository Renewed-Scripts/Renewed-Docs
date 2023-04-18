---
description: All the events that can be used Client Side with Renewed Lib
---

# Events

This tells the client that the player has left or changed character and to prepare for the new data being sent

```lua
AddEventHandler('Renewed-Lib:client:PlayerUnloaded', function()
    -- player left // changed character
end)
```



This tells the client that the new player has loaded and you can use the Player table however you'd like as it contains CharId, Name and Groups

```lua
AddEventHandler('Renewed-Lib:client:PlayerLoaded', function(Player)
    -- Player Loads in and sends all their Table --
    print(json.encode(Player))
end)
```



This tells the client that the Players group has been updated

```lua
AddEventHandler('Renewed-Lib:client:UpdateGroup', function(newGroups)
    -- Update playergroups --
    Player.Group = newGroups
end)
```

