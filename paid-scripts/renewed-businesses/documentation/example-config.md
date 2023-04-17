---
description: An example of what a configured business should look like
---

# 📃 Example Config



```lua
Config.Businesses['uwu'] = {

    -- This table is required and will control most of the business information such as job etc.
    Job = {
        jobName = 'catcafe', -- Job name that has access to the restaurant.
        businessName = 'CAt Café', -- This name will be used for Renewed banking and other places
        societyAccount = 'catcafe', -- The Society account that is connected to your business through Renewed Banking/esx society/qb management
        grade = 0, -- This gradename can deal with the manager menu for creating items, changing prices, etc.
        managerCoords = { -- Use the /zone from ox_lib and remember to specify that its a sphere like. /zone sphere
            coords = vec3(-578.3, -1066.9, 26.55),
            size = 0.40,
        },
    },

    -- This table will allow the business to have an offline shop where players can purchase products when no employer is nearby
    shop = {
        shopLabel = 'UwU Café Shop', -- Shop Label
        shopSlots = 40, -- Shop Slots
        shopWeight = 100, -- The maximum amount of storage for items the store has
        shopCoords = vec4(-584.7, -1060.64, 21.34, 273.86), -- Shop coords (where the players can purchase products)
        model = 'a_f_y_topless_01', -- Ped Model
    },

    -- This table controls which stations are available for the restaurant to use
    Stations = {
        {
            label = 'Stove Prep', -- Label showed in inventory crafting when opened
            text = '[E] Cook', -- This will be the text of the Target OR TextUI if target is false
            coords = vec3(-590.46, -1056.55, 22.36), -- Coords for the sphere
            target = false, -- If set to true then target will be enabled otherwise its text ui
            radius = 0.45, -- Radius of the sphere
            type = {'food', 'drink'} -- Controls weather or not this station is for foods or drinks or both
        },
    },

    -- This table adds stashes which the STAFF of the restauratn can access
    Stashes = {
        {
            label = 'UwU Café Stash', -- Label of the stash when opened
            text = '[E] View Stash', -- if target = false then this text will be visible with textui
            target = false, -- If set to true you must use target to open the stash otherwise it will be opened by drawText saying [E] View Stash
            slots = 100, -- How many slots the inventory stash has
            weight = 100, -- How much weight the stash can hold
            coords = vec3(-588.7, -1067.1, 22.3), -- Coords of the stash
            radius = 0.60, -- size of the sphere for the stash
        }
    },

    -- This table controls the crafting stations for the business, usefull for cutting boards and other misc stuff
    Crafting = {
        {
            label = 'Cutting Board', -- Label of the crafting station when opened
            text = '[E] Cut', -- Text when targetting // viewing the text ui
            radius = 0.45, -- Radius of the sphere
            coords = vec3(-590.49, -1062.97, 22.36), -- Coords for the sphere
            target = false, -- Weather or not Target is enabled for this station

            --[[
                Dump all your items you want to be craftable here, you can follow the guide below to see how to configure it
                https://overextended.github.io/docs/ox_inventory/Guides/crafting
            ]]
            items = {
                {
                    name = 'sandwichbread',
                    ingredients = {
                        breadloaf = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 10,
                },
                {
                    name = 'cutstrawberry',
                    ingredients = {
                        strawberry = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'strawberryjuice',
                    ingredients = {
                        cutstrawberry = 5,
                        blender = 0.01
                    },
                    duration = 7500,
                    count = 2,
                },
                {
                    name = 'cutapples',
                    ingredients = {
                        apples = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'applejuice',
                    ingredients = {
                        cutapples = 5,
                        blender = 0.01
                    },
                    duration = 7500,
                    count = 2,
                },
                {
                    name = 'cutpickle',
                    ingredients = {
                        pickle = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'cutpineapple',
                    ingredients = {
                        pineapple = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'pineapplejuice',
                    ingredients = {
                        cutpineapple = 5,
                        blender = 0.01
                    },
                    duration = 7500,
                    count = 2,
                },
                {
                    name = 'cutorange',
                    ingredients = {
                        orange = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'orangejuice',
                    ingredients = {
                        cutorange = 5,
                        blender = 0.01
                    },
                    duration = 7500,
                    count = 2,
                },
                {
                    name = 'cutblueberry',
                    ingredients = {
                        blueberry = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'blueberryjuice',
                    ingredients = {
                        cutblueberry = 5,
                        blender = 0.01
                    },
                    duration = 7500,
                    count = 2,
                },
                {
                    name = 'cutlime',
                    ingredients = {
                        lime = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'limejuice',
                    ingredients = {
                        cutlime = 5,
                        blender = 0.01
                    },
                    duration = 7500,
                    count = 2,
                },
                {
                    name = 'grapejuice',
                    ingredients = {
                        grapes = 1,
                        blender = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'cutlemon',
                    ingredients = {
                        lemon = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'lemonjuice',
                    ingredients = {
                        cutlemon = 5,
                        blender = 0.01
                    },
                    duration = 7500,
                    count = 2,
                },
                {
                    name = 'cutkiwi',
                    ingredients = {
                        kiwi = 5,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 2,
                },
                {
                    name = 'choplettuce',
                    ingredients = {
                        lettuce = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'choptomato',
                    ingredients = {
                        tomato = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'slicedtomato',
                    ingredients = {
                        tomato = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'potatoslice',
                    ingredients = {
                        potatoes = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'potatoskins',
                    ingredients = {
                        potatoes = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 2,
                },
                {
                    name = 'choppotato',
                    ingredients = {
                        potatoes = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 7,
                },
                {
                    name = 'chopsquash',
                    ingredients = {
                        squash = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'chopspinach',
                    ingredients = {
                        spinach = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'chopcelery',
                    ingredients = {
                        celery = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'chopredpepper',
                    ingredients = {
                        redpeppers = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'slicedredpepper',
                    ingredients = {
                        redpeppers = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 3,
                },
                {
                    name = 'chopgreenpepper',
                    ingredients = {
                        greenpepper = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'slicedgreenpepper',
                    ingredients = {
                        greenpepper = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 3,
                },
                {
                    name = 'chophotpepper',
                    ingredients = {
                        hotpepper = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'chopcarrots',
                    ingredients = {
                        carrots = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'chopcucumbers',
                    ingredients = {
                        cucumbers = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'chopbroccoli',
                    ingredients = {
                        broccoli = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },
                {
                    name = 'cubemozzarella',
                    ingredients = {
                        mozzarella = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 10,
                },
                {
                    name = 'stringmozzarella',
                    ingredients = {
                        mozzarella = 1,
                        grater = 0.01
                    },
                    duration = 7500,
                    count = 15,
                },
                {
                    name = 'cubeprovolone',
                    ingredients = {
                        provolone = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 10,
                },
                {
                    name = 'stringprovolone',
                    ingredients = {
                        provolone = 1,
                        grater = 0.01
                    },
                    duration = 7500,
                    count = 15,
                },
                {
                    name = 'cubecheddar',
                    ingredients = {
                        provolone = 1,
                        kitchenknife = 0.01
                    },
                    duration = 7500,
                    count = 10,
                },
                {
                    name = 'stringcheddar',
                    ingredients = {
                        provolone = 1,
                        grater = 0.01
                    },
                    duration = 7500,
                    count = 15,
                },
                {
                    name = 'parmesanflakes',
                    ingredients = {
                        provolone = 1,
                        grater = 0.01
                    },
                    duration = 7500,
                    count = 15,
                },

                -- meat --

                {
                    name = 'slicedbologna',
                    ingredients = {
                        bologna = 1,
                        cleaver = 0.01
                    },
                    duration = 7500,
                    count = 10,
                },

                {
                    name = 'slicedham',
                    ingredients = {
                        wholeham = 1,
                        cleaver = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },

                {
                    name = 'dicedham',
                    ingredients = {
                        slicedham = 1,
                        cleaver = 0.01
                    },
                    duration = 7500,
                    count = 10,
                },

                {
                    name = 'nystrip',
                    ingredients = {
                        meetslab = 1,
                        cleaver = 0.01
                    },
                    duration = 7500,
                    count = 3,
                },

                {
                    name = 'filet',
                    ingredients = {
                        meetslab = 1,
                        cleaver = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },

                {
                    name = 'chickenstrips',
                    ingredients = {
                        packagedchicken = 1,
                        cleaver = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },

                {
                    name = 'chickenwings',
                    ingredients = {
                        packagedchicken = 1,
                        cleaver = 0.01
                    },
                    duration = 7500,
                    count = 5,
                },

                {
                    name = 'baconbits',
                    ingredients = {
                        bacon = 1,
                        cleaver = 0.01
                    },
                    duration = 7500,
                    count = 7,
                },
            }
        }
    },

    -- This table controls the trays for the business
    Trays = {
        {
            slots = 20, -- The amount of slots for the tray
            weight = 100, -- Amount of weight the stash can hold
            coords = vec3(-584.0, -1062.03, 22.42), -- Coords of the tray
            size = 0.3, -- Size of the sphere
        },
        {
            slots = 20, -- The amount of slots for the tray
            weight = 100, -- Amount of weight the stash can hold
            coords = vec3(-584.09, -1059.31, 22.42), -- Coords of the tray
            size = 0.3, -- Size of the sphere
        },
    },

    -- This table controls the DUI objects for the table
    DUI = {
        {
            label = 'UwU Café Menu', -- Label will be displayed inside the manager menu for the DUI
            ytd = 'denis3d_catcafe_txd', -- YTD File name for the DUI
            ytdname = 't_m_catcafe_imageatlas01', -- Name of the DUI inside the YTD
            width = 512, -- Width of the texture normally its 512 but check in OpenIV to make sure
            height = 512 -- Height of the texture normally its 512 but check in OpenIV to make sure
        },
        {
            label = 'UwU Café Paintings', -- Label will be displayed inside the manager menu for the DUI
            ytd = 'denis3d_catcafe_txd', -- YTD File name for the DUI
            ytdname = 't_m_catcafe_imageatlas02', -- Name of the DUI inside the YTD
            width = 512, -- Width of the texture normally its 512 but check in OpenIV to make sure
            height = 512 -- Height of the texture normally its 512 but check in OpenIV to make sure
        },
    },

    -- This table controls the registers for the business where customers can pay for their food
    Registers = {
        {
            label = 'UwU Café Register', -- Label will be displayed inside the menu when the customer is paying
            coords = vec3(-584.03, -1061.45, 22.37), -- Coords of the register
            size = 0.22, -- Size of the sphere
        },
        {
            label = 'UwU Café Register',-- Label will be displayed inside the menu when the customer is paying
            coords = vec3(-584.06, -1058.73, 22.37), -- Coords of the register
            size = 0.22, -- Size of the sphere
        }
    },

    -- This table controls the ingredeints for the business
    bannedIngredients = {
        --["phone"] = true, -- Here we have an example of banning the item "phone" to be used as an ingredient
    },

    -- This table controls the menu types we have in the business (food, side, dessert, drink)
    MenuTypes = {
        ['main'] = 10, -- This is the amount of ingredients the menu type can have
        ['side'] = 4, -- This is the amount of ingredients the menu type can have
        ['dessert'] = 4, -- This is the amount of ingredients the menu type can have
        ['drink'] = 4, -- This is the amount of ingredients the menu type can have
    },

    -- This table is required and controls the zone outside of the business
    Zone = {
        points = { -- The points of the zones
            vec3(-564.0, -1107.0, 27.0),
            vec3(-615.0, -1085.0, 27.0),
            vec3(-613.0, -1040.0, 27.0),
            vec3(-565.0, -1047.0, 27.0),
        },
        thickness = 12.0, -- Thickness (aka height) of the zone
    },

    -- This table create a blip for the business
    blip = {
        name = 'UwU Café', -- blip name
        coords = vec3(-580.97, -1067.21, 22.34), -- blip coords
        id = 621, -- blip id
        scale = 0.8, -- blip scale
        colour = 41 -- blip colour
    },

    -- This table controls the chairs for the business
    Chairs = {
        vec4(-573.04, -1058.81, 22.5, 180.75),
        vec4(-573.92, -1058.82, 22.5, 180.75),
        vec4(-573.06, -1060.7, 22.5, 0.75),
        vec4(-573.91, -1060.72, 22.5, 0.75),
        vec4(-572.98, -1062.46, 22.5, 180.75),
        vec4(-573.84, -1062.45, 22.5, 180.75),
        vec4(-573.05, -1064.37, 22.5, 0.75),
        vec4(-573.89, -1064.37, 22.5, 0.75),
        vec4(-573.0, -1066.11, 22.5, 180.75),
        vec4(-573.9, -1066.1, 22.5, 180.75),
        vec4(-573.07, -1068.03, 22.5, 0.75),
        vec4(-573.87, -1068.01, 22.5, 0.75),
        vec4(-580.84, -1051.22, 22.35, 277.75),
        vec4(-579.78, -1052.51, 22.35, 329.75),
        vec4(-577.61, -1052.6, 22.35, 35.75),
        vec4(-576.86, -1051.03, 22.35, 108.75),
        vec4(-579.72, -1062.12, 22.35, 0.75),
        vec4(-580.7, -1062.55, 22.35, 45.75),
        vec4(-581.02, -1063.46, 22.35, 90.75),
        vec4(-580.64, -1064.45, 22.35, 135.75),
        vec4(-579.71, -1064.79, 22.35, 180.75),
        vec4(-578.67, -1064.47, 22.35, 225.75),
        vec4(-578.33, -1063.39, 22.35, 270.75),
        vec4(-578.76, -1062.34, 22.35, 315.75),
        vec4(-586.18, -1064.68, 22.6, 90.75),
        vec4(-586.17, -1065.69, 22.6, 90.75),
        vec4(-586.15, -1066.68, 22.6, 90.75),
        vec4(-586.17, -1067.69, 22.6, 90.75),
        vec4(-591.21, -1049.06, 22.35, 180.75),
        vec4(-589.95, -1049.06, 22.35, 180.75),
        vec4(-598.44, -1050.99, 22.35, 270.0),
        vec4(-598.45, -1050.1, 22.35, 270.0),
        vec4(-596.26, -1053.52, 22.35, 0),
        vec4(-573.72, -1052.29, 26.61, 270.0),
        vec4(-573.73, -1053.45, 26.61, 270.0),
        vec4(-569.68, -1066.56, 26.62, 90.0),
        vec4(-569.7, -1068.13, 26.62, 90.0),
        vec4(-570.97, -1069.42, 26.62, 0),
        vec4(-572.61, -1069.4, 26.62, 0),
        vec4(-577.09, -1065.14, 26.61, 165.0),
        vec4(-578.82, -1065.24, 26.61, 200.0),
        vec4(-578.24, -1067.83, 26.61, 0),
        vec4(-577.0, -1062.6, 26.61, 0),
        vec4(-579.1, -1061.28, 26.61, 270.0),
        vec4(-577.39, -1057.87, 26.61, 180.0),
        vec4(-578.59, -1057.9, 26.61, 180.0),
    }
}
```
