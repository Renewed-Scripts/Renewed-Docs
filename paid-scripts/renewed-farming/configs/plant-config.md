# Plant Config

```lua
return {
    circleProgress = true, -- Weather or not to use the ox lib circle progressbar or the default progressbar

    waterWalk = true, -- Weather or not to allow players to walk while watering plants

    waterPercent = 1, -- How much water is lost every 1 minute this means it takes 100 minutes to lose all water
    waterToDurability = 10, -- how much watering can durability is gained by dragging water into it

    Plants = {
        ['pumpkinseed'] = {
            stages = {
                {stage = `SM_PumpkinSeed_01`, offset = vec3(0.0, 0.0, -0.02)},
                {stage = `SM_Pumpkin_01`, offset = vec3(0.0, 0.0, -0.25)},
                {stage = `SM_Pumpkin_02`, offset = vec3(0.0, 0.0, -0.25)},
                {stage = `SM_Pumpkin_03`, offset = vec3(0.0, 0.0, -0.25)},
            },

            plantOffset = -0.24,
            deadplant = {
                stage = `SM_Pumpkin_04`,
                offset = vec3(0.0, 0.0, -0.25),
                percent = 200,
                rewards = { -- rewards for dead plants
                    pumpkinseed = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                pumpkin = { min = 1, max = 5},
                pumpkinseed = { min = 1, max = 3},
            },
        },

        ['cornseed'] = {
            stages = {
                {stage = `SM_CornSeed_01`, offset = vec3(0.0, 0.0, -0.025)},
                {stage = `SM_CornPlant_01`, offset = vec3(0.0, 0.0, -0.26)},
                {stage = `SM_CornPlant_02`, offset = vec3(0.0, 0.0, -0.26)},
                {stage = `SM_CornPlant_03`, offset = vec3(0.0, 0.0, -0.26)},
            },

            plantOffset = -0.24,
            deadplant = {
                stage = `SM_CornPlant_04`,
                offset = vec3(0.0, 0.0, -0.26),
                percent = 200,
                rewards = { -- rewards for dead plants
                    cornseed = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                corn = { min = 1, max = 5},
                cornseed = { min = 1, max = 3},
            },
        },

        ['tomatoseed'] = {
            stages = {
                {stage = `SM_TomatoSeed_01`, offset = vec3(0.0, 0.0, -0.03)},
                {stage = `SM_Tomato_01`, offset = vec3(0.0, 0.0, -0.035)},
                {stage = `SM_Tomato_02`, offset = vec3(0.0, 0.0, -0.035)},
                {stage = `SM_Tomato_03`, offset = vec3(0.0, 0.0, -0.035)},
            },
            plantOffset = -0.032,
            deadplant = {
                stage = `SM_Tomato_04`,
                offset = vec3(0.0, 0.0, -0.025),
                percent = 200,
                rewards = { -- rewards for dead plants
                    tomatoseed = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                tomato = { min = 1, max = 5},
                tomatoseed = { min = 1, max = 3},
            },
        },

        ['carrotseed'] = {
            stages = {
                {stage = `SM_CarrotSeed_01`, offset = vec3(0.0, 0.0, -0.02)},
                {stage = `SM_Carrot_01`, offset = vec3(0.0, 0.0, -0.35)},
                {stage = `SM_Carrot_02`, offset = vec3(0.0, 0.0, -0.35)},
                {stage = `SM_Carrot_03`, offset = vec3(0.0, 0.0, -0.35)},
            },
            plantOffset = -0.35,
            deadplant = {
                stage = `SM_Carrot_04`,
                offset = vec3(0.0, 0.0, -0.35),
                percent = 200,
                rewards = { -- rewards for dead plants
                    carrotseed = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                carrot = { min = 1, max = 5},
                carrotseeds = { min = 1, max = 3},
            },
        },

        ['beetrootseed'] = {
            stages = {
                {stage = `SM_RedBeetSeed_01`, offset = vec3(0.0, 0.0, -0.02)},
                {stage = `SM_RedBeet_01`, offset = vec3(0.0, 0.0, -0.20)},
                {stage = `SM_RedBeet_02`, offset = vec3(0.0, 0.0, -0.35)},
                {stage = `SM_RedBeet_03`, offset = vec3(0.0, 0.0, -0.35)},
            },
            plantOffset = -0.18,
            deadplant = {
                stage = `SM_RedBeet_04`,
                offset = vec3(0.0, 0.0, -0.35),
                percent = 200,
                rewards = { -- rewards for dead plants
                    beetrootseed = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                beetroot = { min = 1, max = 5},
                beetrootseed = { min = 1, max = 3},
            },
        },

        ['radishseed'] = {
            stages = {
                {stage = `SM_RadishSeed_01`, offset = vec3(0.0, 0.0,-0.05)},
                {stage = `SM_Radish_01`, offset = vec3(0.0, 0.0, -0.2)},
                {stage = `SM_Radish_02`, offset = vec3(0.0, 0.0, -0.2)},
                {stage = `SM_Radish_03`, offset = vec3(0.0, 0.0, -0.2)},
            },
            plantOffset = -0.19,

            deadplant = {
                stage = `SM_Radish_04`,
                offset = vec3(0.0, 0.0, -0.2),
                percent = 200,
                rewards = { -- rewards for dead plants
                    radishseed = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                radish = { min = 1, max = 5},
                radishseed = { min = 1, max = 3},
            },
        },

        ['wheatseed'] = {
            stages = {
                {stage = `SM_WheatSeed_02`, offset = vec3(0.0, 0.0, -0.02)},
                {stage = `SM_Wheat_01a`, offset = vec3(0.0, 0.0, -0.2)},
                {stage = `SM_Wheat_02a`, offset = vec3(0.0, 0.0, -0.2)},
                {stage = `SM_Wheat_03a`, offset = vec3(0.0, 0.0, -0.2)},
            },

            plantOffset = -0.24,
            deadplant = {
                stage = `SM_Wheat_04a`,
                offset = vec3(0.0, 0.0, -0.2),
                percent = 200,
                rewards = { -- rewards for dead plants
                    wheatseed = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                wheat = { min = 1, max = 5},
                wheatseed = { min = 1, max = 3},
            },
        },

        ['potato'] = {
            stages = {
                {stage = `SM_PotatoSeed_01`, offset = vec3(0.0, 0.0, -0.05)},
                {stage = `SM_Potato_01`, offset = vec3(0.0, 0.0, -0.35)},
                {stage = `SM_Potato_02`, offset = vec3(0.0, 0.0, -0.37)},
                {stage = `SM_Potato_03`, offset = vec3(0.0, 0.0, -0.39)},
            },

            plantOffset = -0.35,
            deadplant = {
                stage = `SM_Potato_04`,
                offset = vec3(0.0, 0.0, -0.39),
                percent = 200,
                rewards = { -- rewards for dead plants
                    potato = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                potato = { min = 1, max = 5},
            },
        },

        ['watermelonseed'] = {
            stages = {
                {stage = `SM_WatermelonSeed_01`, offset = vec3(0.0, 0.0, -0.02)},
                {stage = `SM_Watermelon_01`, offset = vec3(0.0, 0.0, -0.23)},
                {stage = `SM_Watermelon_02`, offset = vec3(0.0, 0.0, -0.2)},
                {stage = `SM_Watermelon_03`, offset = vec3(0.0, 0.0, -0.2)},
            },

            plantOffset = -0.22,
            deadplant = {
                stage = `SM_Watermelon_04`,
                offset = vec3(0.0, 0.0, -0.2),
                percent = 200,
                rewards = { -- rewards for dead plants
                    watermelonseed = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                watermelon = { min = 1, max = 5},
                watermelonseed = { min = 1, max = 3},
            },
        },

        ['cucumberseed'] = {
            stages = {
                {stage = `SM_CucumberSeed_01`, offset = vec3(0.0, 0.0, -0.04)},
                {stage = `SM_Cucumber_01`, offset = vec3(0.0, 0.0, -0.2)},
                {stage = `SM_Cucumber_02`, offset = vec3(0.0, 0.0, -0.2)},
                {stage = `SM_Cucumber_03`, offset = vec3(0.0, 0.0, -0.2)},
            },

            plantOffset = -0.19,
            deadplant = {
                stage = `SM_Cucumber_04`,
                offset = vec3(0.0, 0.0, -0.2),
                percent = 200,
                rewards = { -- rewards for dead plants
                    cucumberseed = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                cucumber = { min = 1, max = 5},
                cucumberseed = { min = 1, max = 3},
            },
        },

        ['sunflowerseed'] = {
            stages = {
                {stage = `SM_SunflowerSeed_01`, offset = vec3(0.0, 0.0, -0.05)},
                {stage = `SM_Sunflower_01`, offset = vec3(0.0, 0.0, -0.1)},
                {stage = `SM_Sunflower_02`, offset = vec3(0.0, 0.0, -0.1)},
                {stage = `SM_Sunflower_03`, offset = vec3(0.0, 0.0, -0.1)},
            },

            plantOffset = -0.06,
            deadplant = {
                stage = `SM_Sunflower_04`,
                offset = vec3(0.0, 0.0, -0.1),
                percent = 200,
                rewards = { -- rewards for dead plants
                    sunflowerseed = { min = 1, max = 1},
                }
            },

            growthTime = 20,
            rewards = {
                sunflower = { min = 1, max = 5},
                sunflowerseed = { min = 1, max = 3},
            },
        },

        ['garlicseed'] = {
            stages = {
                {stage = `SM_GarlicSeed_01`, offset = vec3(0.0, 0.0, -0.06)},
                {stage = `SM_Garlic_01`, offset = vec3(0.0, 0.0, -0.15)},
                {stage = `SM_Garlic_02`, offset = vec3(0.0, 0.0, -0.15)},
                {stage = `SM_Garlic_03`, offset = vec3(0.0, 0.0, -0.15)},
            },

            plantOffset = -0.12,
            deadplant = {
                stage = `SM_Garlic_04`,
                offset = vec3(0.0, 0.0, -0.15),
                percent = 200,
                rewards = { -- rewards for dead plants
                    garlicseed = { min = 1, max = 1},
                }
            },

            growthTime = 20,
            rewards = {
                garlic = { min = 1, max = 5},
                garlicseed = { min = 1, max = 3},
            },
        },

        ['cabbageseed'] = {
            stages = {
                {stage = `SM_CabbageSeed_01`, offset = vec3(0.0, 0.0, -0.02)},
                {stage = `SM_Cabbage_01`, offset = vec3(0.0, 0.0, -0.225)},
                {stage = `SM_Cabbage_02`, offset = vec3(0.0, 0.0, -0.2)},
                {stage = `SM_Cabbage_03`, offset = vec3(0.0, 0.0, -0.2)},
            },

            plantOffset = -0.22,
            deadplant = {
                stage = `SM_Cabbage_04`,
                offset = vec3(0.0, 0.0, -0.2),
                percent = 200,
                rewards = { -- rewards for dead plants
                    cabbageseed = { min = 1, max = 1},
                },
            },

            growthTime = 20,
            rewards = {
                garlic = { min = 1, max = 5},
                garlicseed = { min = 1, max = 3},
            },
        },

        ['onionseed'] = {
            stages = {
                {stage = `SM_OnionSeed_01`, offset = vec3(0.0, 0.0, -0.08)},
                {stage = `SM_Onion_01`, offset = vec3(0.0, 0.0, -0.19)},
                {stage = `SM_Onion_02`, offset = vec3(0.0, 0.0, -0.18)},
                {stage = `SM_Onion_03a`, offset = vec3(0.0, 0.0, -0.18)},
                {stage = `SM_Onion_03b`, offset = vec3(0.0, 0.0, -0.17)},
            },

            plantOffset = -0.15,
            deadplant = {
                stage = `SM_Onion_04`,
                offset = vec3(0.0, 0.0, -0.18),
                percent = 200,
                rewards = { -- rewards for dead plants
                    onionseed = { min = 1, max = 1},
                },
            },


            growthTime = 20,
            rewards = {
                garlic = { min = 1, max = 5},
                garlicseed = { min = 1, max = 3},
            },
        },
    }
}
```
