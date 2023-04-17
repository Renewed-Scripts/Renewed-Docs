---
description: Use this when starting a new business Config
---

# 📃 Empty Config

```lua
-- Make sure to change 'example' to whatever you want
Config.Businesses['example'] = {

    Job = {
        jobName = '',
        businessName = '',
        societyAccount = '',
        grade = 0,
        managerCoords = {
            coords = vec3(0, 0, 0),
            size = 0.40,
        },
    },

    shop = {
        shopLabel = '',
        shopSlots = 40,
        shopWeight = 100,
        shopCoords = vec4(0, 0, 0, 0),
        model = '',
    },

    Stations = {
        {
            label = '',
            text = '',
            coords = vec3(0,0, 0),
            target = false,
            radius = 0.45,
            type = {'food', 'drink'}
        },
    },

    Stashes = {
        {
            label = '',
            text = '',
            slots = 100,
            weight = 100,
            coords = vec3(0, 0, 0),
            radius = 0.60,
            target = false,
        }
    },

    Crafting = {
        {
            label = '',
            text = '',
            radius = 0.45,
            coords = vec3(0, 0, 0),
            target = false,

            --[[
                Dump all your items you want to be craftable here, you can follow the guide below to see how to configure it
                https://overextended.github.io/docs/ox_inventory/Guides/crafting
            ]]
            items = {}
        }
    },

    Trays = {
        {
            slots = 20,
            weight = 100,
            coords = vec3(0, 0, 0),
            size = 0.3,
        },
        {
            slots = 20,
            weight = 100,
            coords = vec3(0, 0, 0),
            size = 0.3,
        },
    },

    DUI = {
        {
            label = '',
            ytd = '',
            ytdname = '',
            width = 512,
            height = 512
        },
        {
            label = '',
            ytd = '',
            ytdname = '',
            width = 512,
            height = 512
        },
    },

    Registers = {
        {
            label = '',
            coords = vec3(0, 0, 0),
            size = 0.22,
        },
        {
            label = '',
            coords = vec3(0, 0, 0),
            size = 0.22,
        }
    },

    bannedIngredients = {
        --["phone"] = true,
    },

    MenuTypes = {
        ['main'] = 10,
        ['side'] = 4,
        ['dessert'] = 4,
        ['drink'] = 4,
    },

    Zone = {
        points = {
            vec3(0, 0, 0),
            vec3(0, 0, 0),
            vec3(0, 0, 0),
            vec3(0, 0, 0),
        },
        thickness = 12.0,
    },

    blip = {
        name = '',
        coords = vec3(0, 0, 0),
        id = 621,
        scale = 0.8,
        colour = 41
    },

    Chairs = {
    }
}
```
