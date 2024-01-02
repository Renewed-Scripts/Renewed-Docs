# 🔵 Setters and Getters

{% hint style="info" %}
This page is for developers who want to implement Renewed-Fuel within their resources.
{% endhint %}

## Getters

### Client

Statebag: Entity(vehicleId).state.fuel

```lua
local vehicle = cache.vehicle -- Ox Lib example
local fuel = Entity(vehicle).state.fuel

-- Optimized way (Use this if you need to get vehicle fuels in LOOPS)
local function enteredCar()
    local vehicle = cahe.vehicle
    local state = Entity(vehicle).state
    while true do
        print(state.fuel)
    end
end
```

Export: exports\['Renewed-Fuel']:GetFuel(vehicleId) -- (Not recommended)

```lua
local fuel, fuelType = exports['Renewed-Fuel']:GetFuel(cache.vehicle) -- ox lib example
```

### Server

Statebag: Entity(vehicleId).state.fuel

```lua
local vehicle = GetVehiclePedIsIn(GetPlayerPed(source))
local fuel = Entity(vehicle).state.fuel
local fuelType = Entity(vehicle).state.fuelType
```

## Setters

### Client

Export: exports\['Renewed-Fuel']:SetFuel(vehicleId)

```lua
exports['Renewed-Fuel']:SetFuel(cache.vehicle, amount, fuelType) 
-- fueltype defaults to current fuelType or 86 if nil
```

### &#x20;Server

Export: exports\['Renewed-Fuel']:SetFuel(vehicleId)

```lua
local vehicle = GetVehiclePedIsIn(GetPlayerPed(source))
exports['Renewed-Fuel']:SetFuel(vehicle, amount, fuelType) 
```



### Gas Station exports

Get the gas station tank storage

```lua
local Storage = exports['Renewed-Fuel']:GetStorage(StationId, tankId) 
-- Station ID is the ID in the db, the tankId, is 1-4 depending on how many tanks the station have 
```

Set the gas station tank storage

```lua
exports['Renewed-Fuel']:SetStorage(StationId, tankId, amount, fuelType)
-- Station ID is the ID in the db, tankId is 1-4 depending how many tanks the station have
```
