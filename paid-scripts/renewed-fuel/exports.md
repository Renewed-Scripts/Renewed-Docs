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
local fuel = exports['Renewed-Fuel']:GetFuel(cache.vehicle) -- ox lib example
```

### Server

Statebag: Entity(vehicleId).state.fuel

```lua
local vehicle = GetVehiclePedIsIn(GetPlayerPed(source))
local fuel = Entity(vehicle).state.fuel
```

## Setters

### Client

Export: exports\['Renewed-Fuel']:SetFuel(vehicleId)

```lua
exports['Renewed-Fuel']:SetFuel(cache.vehicle, amount, fuelType) 
-- fueltype defaults to 86 if nil
```

### &#x20;Server

Export: exports\['Renewed-Fuel']:SetFuel(vehicleId)

```lua
local vehicle = GetVehiclePedIsIn(GetPlayerPed(source))
exports['Renewed-Fuel']:SetFuel(vehicle, amount, fuelType) 
```

