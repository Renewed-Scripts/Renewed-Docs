---
description: >-
  Here is all the exports for the script that you can incorporate into your own
  scripts
---

# 🚙 Exports

### Client

```lua
exports['Renewed-Vehiclekeys']:hasKey() -- Returns true/false if player has keys
```

### Server

```lua
-- Removes the key from a player
exports['Renewed-Vehiclekeys']:removeKey(source, plate)

-- returns true/false if the player has the key
exports['Renewed-Vehiclekeys']:hasKey(source, plate)

-- Adds a key to the specified player
exports['Renewed-Vehiclekeys']:addKey(source, plate)
```
