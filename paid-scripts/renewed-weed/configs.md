---
description: Here you will see all possible Configs
---

# 📚 Configs

### Plant Config

```lua
return {

    -- plant config --
    maxWeight = 5, -- How much can a perfectly healthy plant weight?
    GrowthTime = 300, -- How many minutes it takes for a plant to grow
    Distance = 400, -- What's the distance in GTA units before the weed get spawned / despawned
    canClimb = false, -- Can the player climb on top of the weed plant(s)?


    -- Plant Update Config --
    updateInterval = 10, -- How many minutes inbetween plant state updates (water, hunger, deletion etc.)
    plantInterval = 30, -- How many seconds in between plants being updated? the lower the more heavy it's on the server the longer the more delay there is (30 - 60 seconds seem to be the sweatspot)
    damageLimit = 5, -- The threshold of water + fertilizer a plant can have before it starts taking damage
    thirstInterval = { min = 3, max = 10 }, -- The amount of thirst a plants loose every update interval
    hungerInterval = { min = 3, max = 10 }, -- The amount of hunger a plants loose every update interval
    healthInterval = { min = 10, max = 40 }, -- The amount of health a plants loose every update interval


    -- Male Plant Config --
    maxFemale = 10, -- maximum amount of female seeds IF plant is male and is at 100% health
    maxMale = 5, -- maximum amount of male seeds IF plant is male and is at 100% health


    -- Watering can Config --
    waterToDurability = 10, -- How much durability does the watering can get per water bottle
    maxWaterDurability = 10, -- From 0 to full water on a plant how much durability minus? ( 10 = 0-100% water only removes 10 durability from the watering can)
    canWeight = 5, -- How much can a watering can weight when it's full of water


    -- Brick Config --
    driedWeight = 50, -- How much does 1 dried weed weight? if you change it inside your inventory change it here for the weed bricks
    minWeed = 5, -- How much dried weed minimum can you use to make a brick?
    maxWeed = 50, -- How much dried weed maximum can you use to make a brick?


    -- Misc stuff --
    circleProgress = true, -- Use circle progress bar instead of the default one
    clearPlantingAnim = true, -- Clear the planting animation IMMEDIATELY after planting a plant

    -- Here are ALL the item names for all the items used for weed growing, change them incase your server uses different names and such.
    Items = {
        water = 'water',
        driedweed = 'driedweed',
        wateringcan = 'wateringcan',
        fertilizer = 'fertilizer',
        emptybag = 'emptybag',
        fullbag = 'fullbag',
        weedbrick = 'weedbrick'
    },

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

    objectOffsets = {
        {
            prop = `bkr_prop_weed_01_small_01b`,
            offset = vec3(0.0, 0.0, -0.5)
        },
        {
            prop = `bkr_prop_weed_med_01a`,
            offset = vec3(0.0, 0.0, -2.5)
        },
        {
            prop = `bkr_prop_weed_med_01b`,
            offset = vec3(0.0, 0.0, -2.5)
        },
        {
            prop = `bkr_prop_weed_lrg_01a`,
            offset = vec3(0.0, 0.0, -2.5)
        },
        {
            prop = `bkr_prop_weed_lrg_01b`,
            offset = vec3(0.0, 0.0, -2.5)
        },
    }
}
```

### Strain Config

```lua
return {
    qualityMin = 0, -- How much minimum can your strain quality improve when fertilizing plants?
    qualityMax = 3, -- How much maximum can your strain quality improve when fertilizing plants?

    -- Big thanks to mannyonbrazzers for providing the list of strain names!
    StrainX1 = {
        'Afghani Wonder',
        'Afgooey',
        'Apollo',
        'Buddha',
        'Burmaberry',
        'BushDoctor',
        'Bushmans',
        'Chem',
        'Cherry',
        'Chocolope',
        'Cinnamon',
        'Cotton',
        'Cripple',
        'Crystal',
        'Donk',
        'Ducksfoot',
        'Dutch',
        'Elvis',
        'Orange',
        'Rosado',
        'Verde',
        'Violeta',
        'Haze',
        'Urkle',
        'Emerald',
        'G',
        'Dynamite',
        'Earthquake',
        'Elephant',
        'Endless Sky',
        'Erez',
        'Euphoria',
        'Frosty',
        'Pebbles',
        'Incredible',
        'Melt',
        'Funky',
        'Cheese',
        'Firewalker',
        'Flo',
        'Fraggle',
        'Frankenberry',
        'Leonard',
        'Freeze',
        'Skydog',
        'Special',
        'Spurkle',
        'Sputnik',
        'Fuzzy',
        'George',
        'Ghost',
        'Scout',
        'Glass',
        'Gnarsty',
        'God',
        'Tora',
        'Vortex',
        'Shark',
        'Star',
        'Starry',
        'Tangerine',
    },

    StrainX2 = {
        'Platinum',
        'Pineapple',
        'Papaya',
        'Lace',
        'Coconut',
        'Linen',
        'Bone',
        'Moss',
        'Shamrock',
        'Seafoam',
        'Pine',
        'Pakalolo',
        'Ivory',
        'Cream',
        'Egg shell',
        'Remus',
        'Salt',
        'Peanut',
        'Carob',
        'Hickory',
        'Salmon',
        'Pecan',
        'Walnut',
        'Caramel',
        'Gingerbread',
        'Syrup',
        'Parakeet',
        'Mint',
        'Seaweed',
        'Somantra',
        'Pistachio',
        'Basil',
        'Crocodile',
        'Brown',
        'Coffee',
        'Special',
        'Sweet',
        'Penny',
        'Cedar',
        'Grey',
        'Shadow',
        'Graphite',
        'Iron',
        'Pewter',
        'Cloud',
        'Silver',
        'Smoke',
        'Slate',
        'Anchor',
        'Ash',
        'Porpoise',
        'Dove',
        'Fog',
        'Flint',
        'Charcoal',
        'Pebble',
        'Lead',
        'Coin',
        'Fossil',
        'Black',
        'Ebony',
        'Crow',
        'Charcoal',
        'Onyx',
        'Pitch',
        'Soot',
        'Sable',
        'Coal',
        'Metal',
        'Obsidian',
        'Spider',
        'Leather',
        'Midnight',
        'Ink',
        'Raven',
        'Oil',
        'Grease',
    },

    StrainX3 = {
        'Chase',
        'Cocktail',
        'Cocopuff',
        'Herb',
        'Chronic',
        'Blossom',
        'Flower',
        'Weed',
        'Pot',
        'Grass',
        'Reefer',
        'Ganja',
        'Lace',
        'Butter',
        'Geek',
        'Hash',
        'Bud',
        'Plant',
        'Bush',
    }
}
```

### Weed Runs

```lua
return {
    -- START SETTINGS --
    pedModel = `mp_m_weed_01`,
    pedCoords = vec4(94.791, -1809.941, 26.083, 229.595),
    scenario = 'WORLD_HUMAN_SMOKING_POT',

    -- PRICE SETTINGS --
    pricePerGram = 100, -- How much money does the player get per 100 weight of weed, THIS SCALES BASED OFF OF THE QUALITY OF THE WEED

    pdAlert = '', -- Pre configured for Project Sloth dispatch, you can add your own in the client/utils.lua file
    alertChance = 10, -- The chance of the police being alerted when the player is caught


    -- Deliver Blip Options
    blipSettings = {
        sprite = 140,
        color = 3,
        scale = 0.8,
    },


    -- List of random peds that can spawn as "customers"
    peds = {
        `g_m_m_armgoon_01`,
        `csb_avery`,
        `csb_popov`,
        `cs_terry`,
        `cs_carbuyer`,
        `a_m_y_cyclist_01`,
    },

    -- List of random scenarios the peds will have for weed runs
    scenarios = {
        'WORLD_HUMAN_SMOKING',
        'WORLD_HUMAN_STAND_MOBILE',
        'WORLD_HUMAN_DRUG_DEALER',
        'WORLD_HUMAN_PROSTITUTE_HIGH_CLASS',
        'CODE_HUMAN_CROSS_ROAD_WAIT',
        'WORLD_HUMAN_STAND_IMPATIENT',
        'WORLD_HUMAN_HANG_OUT_STREET'
    },

    -- A list of all possible locations for the drop offs --
    locations = {
        vec4(581.162, 138.475, 99.475, 154.009),
        vec4(299.634, 363.577, 105.417, 1.405),
        vec4(799.148, -496.435, 30.627, 114.611),
        vec4(603.909, -3099.572, 6.069, 235.896),
        vec4(-659.568, -2450.371, 13.944, 234.741),
        vec4(-943.412, -1569.117, 5.178, 219.704),
        vec4(-1317.888, -939.221, 9.731, 304.581),
        vec4(-1437.909, -372.425, 38.306, 128.263),
        vec4(-1985.753, -314.807, 48.106, 62.196),
        vec4(-2312.726, 266.787, 169.602, 23.482),
        vec4(-3054.898, 174.086, 11.608, 221.611),
        vec4(-172.377, 6119.515, 31.399, 229.023),
        vec4(1726.561, 4775.276, 41.934, 254.962),
        vec4(2405.898, 4025.695, 36.044, 66.019),
        vec4(837.103, 504.867, 125.919, 158.605),
        vec4(-681.298, -171.396, 37.821, 303.818)
    }
}
```
