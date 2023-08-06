# Random Plants Config

```lua
--[[
    Here you would put locations for random plants that will spawn around the map, this will work for entry level people to get into farming for free.
    if You dislike this you can always just put disable to true.
]]

return {
    disable = false, -- Weather or not you want to disable this sytem.

    minusOne = true, -- Most admin menus takes the z as top of the player head and not the bottom of the player feet. If you change all locations then go ahead and set this to false.

    maxSpots = 35, -- How many random spots do you want spawned around the map on restart
    Locations = {
        {
            coords = vec3(1815.756, 4594.321, 36.847),
            type = 'random' -- Can be random, none or a specific seed from the plant config
        },

        {
            coords = vec3(1815.756, 4594.321, 36.847),
        },

        {
            coords = vec3(1815.756, 4594.321, 36.847),
        },
    }
}
```
