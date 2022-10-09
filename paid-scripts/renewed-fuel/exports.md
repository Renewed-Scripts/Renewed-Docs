# 🔵 Exports



{% hint style="info" %}
This page is for developers who want to utilize some of ours functions and exports within their scripts
{% endhint %}

### GetFuel

This export will return the amount of fuel the given vehicle has. Look below for an example

```
GetFuel(Vehicle: entity)

local vehicle = QBCore.Functions.GetClosestVehicle()
local fuel = exports['Renewed-Fuel']:GetFuel(vehicle)
print(fuel) -- Prints the amount of fuel the closest vehicle has.
```

### SetFuel (CLIENT AND SERVER EXPORT)

This export is used for setting the fuel in vehicles, please use the below example to implement it into your scripts!

```
SetFuel(Vehicle: entity, Fuel: number)

local vehicle = QBCore.Functions.GetClosestVehicle()
exports['Renewed-Fuel']:SetFuel(vehicle, 100) -- Sets the closest vehicle Fuel to 100
```

