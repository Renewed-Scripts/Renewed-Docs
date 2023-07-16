# 📚 Configs

```lua
return {
    -- Loot Config --
    lootTime = 60, -- Time in seconds it takes a bee to produce wax
    lootAmount = {min = 1, max = 3}, -- Amount of wax produced per loot time

    anyPickup = false, -- Allow anyone to pickup the hive

    -- Misc stuff --
    circleProgress = true, -- Use circle progress bar instead of the default one

    -- Placement Config --
    allowedMaterials = {
        [-1286696947] = true,
        [-1942898710] = true,
        [-1595148316] = true,
        [-1885547121] = true,
        [-2041329971] = true,
        [-840216541] = true,
        [-461750719] = true,
        [-700658213] = true,
        [-913351839] = true,
        [1109728704] = true,
        [1635937914] = true,
        [1333033863] = true,
        [1144315879] = true,
        [2128369009] = true,
        [951832588] = true,
        [581794674] = true,
        [510490462] = true,
    },

    object = {
        prop = `np_beehive03`,
        fullProp = `np_beehive`,
    }
}
```
