# 📄 Installation

### Step 1

* Run the SQL file called 'runme.sql'

### Step 2

* Headover to your ox\_inventory/data/items.lua and paste in the following

```lua
['pitchfork'] = {
    label = 'Pitch Fork',
    weight = 1000,
    client = {
        export = 'Renewed-Farming.harvestPlants'
    },
},

['beetroot'] = {
    label = 'Beetroot',
    description = 'Freshly harvested beetroot, perfect for cooking or adding to salads.',
    weight = 100
},
['beetrootseed'] = {
    label = 'Beetroot Seed',
    description = 'Small seeds used to grow beetroot plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    },
},

['carrot'] = {
    label = 'Carrot',
    description = 'Crisp and nutritious carrots, a staple ingredient in many recipes. Can be enjoyed raw or cooked.',
    weight = 100
},
['carrotseed'] = {
    label = 'Carrot Seed',
    description = 'Tiny seeds used to grow carrot plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['corn'] = {
    label = 'Corn',
    description = 'Freshly harvested corn, sweet and juicy. Great for grilling or boiling.',
    weight = 100
},
['cornseed'] = {
    label = 'Corn Seed',
    description = 'Small seeds used to grow corn plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['cucumber'] = {
    label = 'Cucumber',
    description = 'Crisp and refreshing cucumbers, perfect for salads or pickling.',
    weight = 100
},
['cucumberseed'] = {
    label = 'Cucumber Seed',
    description = 'Tiny seeds used to grow cucumber plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['garlic'] = {
    label = 'Garlic',
    description = 'Aromatic garlic bulbs, known for their strong flavor and various culinary uses.',
    weight = 100
},
['garlicseed'] = {
    label = 'Garlic Seed',
    description = 'Small cloves used to grow garlic plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['potato'] = {
    label = 'Potato',
    description = 'Versatile and starchy potatoes, ideal for mashing, baking, or frying.',
    weight = 100,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['pumpkin'] = {
    label = 'Pumpkin',
    description = 'Large and festive pumpkins, perfect for carving or using in autumn recipes.',
    weight = 100,
},
['pumpkinseed'] = {
    label = 'Pumpkin Seed',
    description = 'Seeds used to grow pumpkin plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['radish'] = {
    label = 'Radish',
    description = 'Crunchy and peppery radishes, great for adding a kick to salads or pickling.',
    weight = 100
},
['radishseed'] = {
    label = 'Radish Seed',
    description = 'Small seeds used to grow radish plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['sunflower'] = {
    label = 'Sunflower',
    description = 'Bright and cheerful sunflowers, known for their tall stalks and vibrant yellow petals.',
    weight = 100
},
['sunflowerseed'] = {
    label = 'Sunflower Seed',
    description = 'Seeds used to grow sunflower plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['tomato'] = {
    label = 'Tomato',
    description = 'Juicy and flavorful tomatoes, perfect for salads, sauces, or sandwiches.',
    weight = 100
},
['tomatoseed'] = {
    label = 'Tomato Seed',
    description = 'Small seeds used to grow tomato plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['watermelon'] = {
    label = 'Watermelon',
    description = 'Large and refreshing watermelons, perfect for summertime enjoyment.',
    weight = 100
},
['watermelonseed'] = {
    label = 'Watermelon Seed',
    description = 'Seeds used to grow watermelon plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['cabbage'] = {
    label = 'Cabbage',
    description = 'Fresh and crisp cabbage, perfect for salads and cooking.',
    weight = 100
},
['cabbageseed'] = {
    label = 'Cabbage Seed',
    description = 'Seeds used to grow cabbage plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['onion'] = {
    label = 'Onion',
    description = 'Pungent and flavorful onions, a kitchen essential.',
    weight = 100
},
['onionseed'] = {
    label = 'Onion Seed',
    description = 'Seeds used to grow onion plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
},

['wheat'] = {
    label = 'Wheat',
    description = 'Golden wheat grains, a staple crop used for making flour and various food products.',
    weight = 100
},
['wheatseed'] = {
    label = 'Wheat Seed',
    description = 'Small seeds used to grow wheat plants.',
    weight = 10,
    client = {
        export = 'Renewed-Farming.placeSeed'
    }
}
```

### Step 3

* Take the images from Renewed-Farming/images and paste them into ox\_inventory/web/images

And that's it!\
\
You have now successfully installed Renewed-Farming enjoy!
