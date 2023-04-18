# Functions

Import the Library into your resource like this

```lua
local Renewed = exports['Renewed-Lib']:getLib()
```



Checking a players job

```lua
local success = Renewed.hasGroup(source, group, grade)

print(success) -- Returns true / false if the player does not have the group
```



Get Character ID

```lua
local CharId =  Renewed.getCharId(source)

print(CharId) -- Returns the name or false if the player is not loaded in the server
```



Get Character Name

```lua
local name = Renewed.getCharName(source)

print(name) -- Returns the name or false if the player is not loaded in the server
```



Remove Player Money

```lua
local success = Renewed.removeMoney(source, amount, moneyType, reason)

-- True/False weather or not the player had enough money and it was removed
print(success) 
```



Add Player Money

```lua
local success = Renewed.addMoney(source, amount, moneyType, reason)

print(success) -- True/False if the money was added
```



Add Player Needs

```lua
local success = Renewed.addNeeds(source, needs) -- Needs = {hunger = 0, thrist = 0}

print(success) -- prints true/false depending if the needs were added
```
