# ⌨ Exports

### GetPlayerCarryItems

```
exports["Renewed-Weaponscarry"]:GetPlayerCarryItems()

Returns a table of all the items the player is carrying
```

### toggleProps

```
exports["Renewed-Weaponscarry"]:toggleProps()

Toggles the props for the player and wont load them untill they are toggled back on 
OR if they are in their apartments
```

### refreshProps

```
exports["Renewed-Weaponscarry"]:refreshProps()

Refreshes the props for the player toggle this at at the END of your refreshskin events
to make sure the props get removed and refreshed the proper way
```

### isCarryingObject

```
exports["Renewed-Weaponscarry"]:isCarryingObject() 

Returns true if the player is carrying any item
```

### makeObjectBusy

```
exports["Renewed-Weaponscarry"]:makeObjectBusy(item, toggle)

This acts as if the particular item was removed or used by the player
this is useful for items that can be used multiple times such as a fishing rod 
this would allow the player to when they start using the rod for it to be removed
from the players back untill they are done using it
```

### carryProp

```
exports["Renewed-Weaponscarry"]:carryProp(item)

Acts as if the player was given x item to carry
this DOES NOT work with weapons on back ONLY CARRYABLE items
```

### removeProp

```lua
exports["Renewed-Weaponscarry"]:removeProp(item)

Acts as if x item was removed from the player
this DOES NOT work with weapons on back ONLY CARRYABLE items
```

### isCarryingAnObject

```
exports["Renewed-Weaponscarry"]:isCarryingAnObject(item)

Returns true if the players is carrying a specific item
```
