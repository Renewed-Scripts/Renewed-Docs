---
description: The entire config for Renewed Vehiclekeys
---

# 📚 Config

```lua
return {
    lockChance = 1.0, -- (100%) Chance of local vehicles to be locked around the world
    useKeyItem = false, -- set to true if you want to use a item based key system

    engineKey = 'G', -- Key to toggle the engine on and off
    lockKey = 'L', -- Key to toggle the lock on and off

    immune = {
        [`bmx`] = true,
    },

    -- Specific Doors that are ALWAYS locked no matter what
    doorsBlocked = {
        [`stockade`] = {[1] = true, [2] = true}
    },

    -- How much durability is taken away from a lockpick item when used
    durability = {
        lockpick = { min = 2, max = 5 },
        advancedlockpick = { min = 2, max = 5 },
    },

    -- Minigame specific difficulty settings
    minigame = {
        hotwire = { time = {min = 75, max = 150}, turns = {min = 1, max = 5} },
        lockpick = { time = {min = 75, max = 150}, turns = {min = 1, max = 5} },
        advancedlockpick = { time = {min = 50, max = 100}, turns = {min = 1, max = 2} },
    },

    -- Vehicle Config
    vehicles = {
        -- Compacts --
        [0] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },


        -- Sedans --
        [1] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },


        -- SUVS --
        [2] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },


        -- COUPES --
        [3] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },


        -- MUSCLES --
        [4] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- SPORT CLASSICS --
        [5] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- Sports --
        [6] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- SUPERS --
        [7] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- MOTORCYCLES --
        [8] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
            noLocks = true, -- This vehicle cannot be locked!
        },

        -- OFF-ROAD --
        [9] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },


        -- Industrial --
        [10] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- Utility --
        [11] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- Vans --
        [12] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- Cycles --
        [13] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
            noLocks = true, -- This vehicle cannot be locked!
        },

        -- Boats --
        [14] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- Helicopters --
        [15] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },


        -- Planes --
        [16] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- Service --
        [17] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- Emergency --
        [18] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = false, -- Can this vehicle be hotwired?
            search = false, -- Can this vehicle be searched?
        },

        -- Military --
        [19] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- Commercial --
        [20] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- Trains --
        [21] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },

        -- Open Wheel --
        [22] = {
            pickable = true, -- Can this vehicle be lock picked?
            pickItem = {'lockpick', 'advancedlockpick'}, -- What item is required to lock pick this vehicle?
            hotwire = true, -- Can this vehicle be hotwired?
            search = true, -- Can this vehicle be searched?
        },
    },


    -- List of all the weapons that peds do not become scared of when you aim at them
    blockedWeapons = {
        [`WEAPON_UNARMED`] = true,
        [`WEAPON_KNIFE`] = true,
        [`WEAPON_NIGHTSTICK`] = true,
        [`WEAPON_HAMMER`] = true,
        [`WEAPON_BAT`] = true,
        [`WEAPON_CROWBAR`] = true,
        [`WEAPON_GOLFCLUB`] = true,
        [`WEAPON_BOTTLE`] = true,
        [`WEAPON_DAGGER`] = true,
        [`WEAPON_HATCHET`] = true,
        [`WEAPON_MACHETE`] = true,
        [`WEAPON_FLASHLIGHT`] = true,
        [`WEAPON_SWITCHBLADE`] = true,
        [`WEAPON_POOLCUE`] = true,
        [`WEAPON_WRENCH`] = true,
        [`WEAPON_BATTLEAXE`] = true,
        [`WEAPON_GRENADE`] = true,
        [`WEAPON_STICKYBOMB`] = true,
        [`WEAPON_BZGAS`] = true,
        [`WEAPON_MOLOTOV`] = true,
        [`WEAPON_FIREEXTINGUISHER`] = true,
        [`WEAPON_PETROLCAN`] = true,
        [`WEAPON_FLARE`] = true,
        [`WEAPON_BALL`] = true,
        [`WEAPON_SNOWBALL`] = true,
        [`WEAPON_SMOKEGRENADE`] = true,
    }
}
```

