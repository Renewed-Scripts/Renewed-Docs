---
description: >-
  Put these into ox_inventory/data/items.lua, after pasting the items into
  data/items make sure to head over to ox_inventory/web/images and paste in
  every single image from Renewed-Businesses/images
---

# 📚 Items Installation

```
-- // Business Items // --

['business_tempitem'] = {
    label = "how did you get this?",
    weight = 0,
    stack = true,
    close = true,
    consume = 0,
    server = {
        export = 'Renewed-Businesses.useItem',
    }
},

-- Kitchen Tools --

['kitchenknife'] = {
	label = 'Kitchen Knife',
	weight = 50,  
	shopType = 'general',
	price = 10,  
},

['cleaver'] = {
	label = 'Meat Cleaver',
	weight = 50,  
	shopType = 'general',
	price = 10,  
},

['blender'] = {
	label = 'Blender',
	weight = 50,  
	shopType = 'general',
	price = 10,  
},

['whisk'] = {
	label = 'Whisks',
	weight = 50,  
	shopType = 'general',
	price = 10,  
},

['slicer'] = {
	label = 'Slicer',
	weight = 50,  
	shopType = 'general',
	price = 10,  
},

['potatopusher'] = {
	label = 'Potato Pusher',
	weight = 50,  
	shopType = 'general',
	price = 10,  
},

['peeler'] = {
	label = 'Peeler',
	weight = 50,  
	shopType = 'general',
	price = 10,  
},

['scooper'] = {
	label = 'Scooper',
	weight = 50,  
	shopType = 'general',
	price = 10,  
},

['grater'] = {
	label = 'Grater',
	weight = 50,  
	shopType = 'general',
	price = 10,  
},

-- Fruit --

['strawberry'] = {
	label = 'Strawberries',
	weight = 50,  
	shopType = 'farmers',
	price = 10,  
},

['cutstrawberry'] = {
	label = 'Cut Strawberries',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['strawberryjuice'] = {
	label = 'Strawberry Juice',
	weight = 50,   
	foodType = 'drink',
	nutrition = {
		healthy = 3,
		thirst = 3,
	},
},

['apples'] = {
	label = 'Apples',
	weight = 50,  
	shopType = 'farmers',
	price = 10,  
},

['cutapples'] = {
	label = 'Cut Apples',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['applejuice'] = {
	label = 'Apple Juice',
	weight = 50,   
	foodType = 'drink',
	nutrition = {
		healthy = 3,
		thirst = 3,
	},
},

['pickle'] = {
	label = 'Pickles',
	weight = 50,  
	shopType = 'farmers',
	price = 10,  
},

['cutpickle'] = {
	label = 'Cut Pickles',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['pineapple'] = {
	label = 'Pineapples',
	weight = 50,  
	shopType = 'farmers',
	price = 10,  
},

['cutpineapple'] = {
	label = 'Cut Pineapple',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['pineapplejuice'] = {
	label = 'Pineapple Juice',
	weight = 50,   
	foodType = 'drink',
	nutrition = {
		healthy = 3,
		thirst = 3,
	},
},

['orange'] = {
	label = 'Oranges',
	weight = 50,  
	shopType = 'farmers',
	price = 10,  
},

['cutorange'] = {
	label = 'Cut Oranges',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['orangejuice'] = {
	label = 'Orange Juice',
	weight = 50,   
	foodType = 'drink',
	nutrition = {
		healthy = 3,
		thirst = 3,
	},
},

['blueberry'] = {
	label = 'Blueberries',
	weight = 50,  
	shopType = 'farmers',
	price = 10,  
},

['cutblueberry'] = {
	label = 'Cut Blueberries',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['blueberryjuice'] = {
	label = 'Blueberry Juice',
	weight = 50,   
	foodType = 'drink',
	nutrition = {
		healthy = 3,
		thirst = 3,
	},
},

['boba'] = {
	label = 'Boba',
	weight = 50,   
	foodType = 'food',
	shopType = 'farmers',
	price = 10, 
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['lime'] = {
	label = 'Limes',
	weight = 50,  
	shopType = 'farmers',
	price = 10,  
},

['cutlime'] = {
	label = 'Cut Limes',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['limejuice'] = {
	label = 'Lime Juice',
	weight = 50,   
	foodType = 'drink',
	nutrition = {
		healthy = 3,
		thirst = 3,
	},
},

['banana'] = {
	label = 'Bananas',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
	nutrition = {
		healthy = 3,
		hunger = 3,
	}, 
},

['cutbananas'] = {
	label = 'Cut Bananas',
	weight = 50,   
	foodType = {'food', 'drink'},
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['grapes'] = {
	label = 'Grapes',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
	nutrition = {
		healthy = 3,
		hunger = 3,
	}, 
},

['grapejuice'] = {
	label = 'Grape Juice',
	weight = 50,   
	foodType = 'drink',
	nutrition = {
		healthy = 3,
		thirst = 3,
	},
},

['lemons'] = {
	label = 'Lemons',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['lemonjuice'] = {
	label = 'Lemon Juice',
	weight = 50,   
	foodType = 'drink',
	nutrition = {
		healthy = 3,
		thirst = 3,
	},
},

['cutlemon'] = {
	label = 'Cut Lemon',
	weight = 50,   
	foodType = 'drink',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},


['kiwi'] = {
	label = 'Kiwi',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['cutkiwi'] = {
	label = 'Cut Kiwi',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['cherry'] = {
	label = 'Cherries',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['cherryjuice'] = {
	label = 'Cherry Juice',
	weight = 50,   
	foodType = 'drink',
	nutrition = {
		healthy = 3,
		thirst = 3,
	},
},

['lettuce'] = {
	label = 'Lettuce Head',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['choplettuce'] = {
	label = 'Chopped Lettuce',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['tomato'] = {
	label = 'Tomatos',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['choptomato'] = {
	label = 'Chopped Tomato',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['slicedtomato'] = {
	label = 'Tomato Slices',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['potatoes'] = {
	label = 'Potatoes',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['potatoslice'] = {
	label = 'Sliced Potatoes',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		salt = 2,
		hunger = 3,
	},
},

['potatoskins'] = {
	label = 'Potato Skins',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		salt = 2,
		hunger = 3,
	},
},

['choppotato'] = {
	label = 'Chopped Potatoes',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		salt = 2,
		hunger = 3,
	},
},

['squash'] = {
	label = 'Squash',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['chopsquash'] = {
	label = 'Chopped Squash',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['spinach'] = {
	label = 'Spinach',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['chopspinach'] = {
	label = 'Chopped Spinach',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['celery'] = {
	label = 'Celery',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['chopcelery'] = {
	label = 'Chopped Celery',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['redpeppers'] = {
	label = 'Red Peppers',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['slicedredpepper'] = {
	label = 'Sliced Red Pepper',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['chopredpepper'] = {
	label = 'Chopped Red Pepper',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['greenpeppers'] = {
	label = 'Green Peppers',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['slicedgreenpepper'] = {
	label = 'Sliced Green Pepper',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['chopgreenpepper'] = {
	label = 'Chopped Green Pepper',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['hotpepper'] = {
	label = 'Jalapeno Peppers',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['chophotpepper'] = {
	label = 'Chopped Jalapeno Pepper',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['carrots'] = {
	label = 'Carrots',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['chopcarrots'] = {
	label = 'Chopped Carrots',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['cucumbers'] = {
	label = 'Cucumbers',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['chopcucumbers'] = {
	label = 'Chopped Cucumbers',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['peas'] = {
	label = 'Peas',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['greenbeans'] = {
	label = 'Grean Beans',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['corn'] = {
	label = 'Corn',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['cobcorn'] = {
	label = 'Corn on the Cob',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

['broccoli'] = {
	label = 'Broccoli',
	weight = 50,  
	shopType = 'farmers',
	price = 10, 
},

['chopbroccoli'] = {
	label = 'Chopped Broccoli',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		healthy = 3,
		hunger = 3,
	},
},

-- // Dairy // --

['milk'] = {
	label = 'Milk',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = {'food', 'drink'},
	nutrition = {
		dairy = 3,
		thirst = 3,
	},
},

['eggs'] = {
	label = 'Eggs',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
	nutrition = {
		dairy = 3,
		protein = 2,
		hunger = 3,
	},
},

['butter'] = {
	label = 'Butter',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['condensedmilk'] = {
	label = 'Condensed Milk',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['yogurt'] = {
	label = 'Yogurt',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = {'food', 'drink'},
	nutrition = {
		dairy = 3,
		hunger = 3,
		thirst = 2,
	},
},

['mozzarella'] = {
	label = 'Mozzarella Cheese',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
},

['cubemozzarella'] = {
	label = 'Cubbed Mozzarella Cheese',
	weight = 50,    
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['stringmozzarella'] = {
	label = 'String Mozzarella Cheese',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['provolone'] = {
	label = 'Provolone Cheese',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
},

['cubeprovolone'] = {
	label = 'Cubbed Provolone Cheese',
	weight = 50,    
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['stringprovolone'] = {
	label = 'String Provolone Cheese',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['cheddar'] = {
	label = 'Cheddar Cheese',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
},

['cubecheddar'] = {
	label = 'Cubbed Cheddar Cheese',
	weight = 50,    
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['stringcheddar'] = {
	label = 'String Cheddar Cheese',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['bluecheese'] = {
	label = 'Blue Cheese',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['parmesan'] = {
	label = 'Parmesan Cheese',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
},

['parmesanflakes'] = {
	label = 'Parmesan Flakes',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['ricotta'] = {
	label = 'Ricotta Cheese',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['creamcheese'] = {
	label = 'Cream Cheese',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['gouda'] = {
	label = 'Cream Cheese',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['cottagecheese'] = {
	label = 'Cottage Cheese',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['swiss'] = {
	label = 'Swiss Cheese',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = 'food',
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

['icecream'] = {
	label = 'Ice Cream',
	weight = 50,   
	shopType = 'dairy',
	price = 10, 
	foodType = {'food', 'drink'},
	nutrition = {
		dairy = 3,
		hunger = 3,
	},
},

-- // Meat // --


['bologna'] = {
	label = 'Bologna',
	weight = 50,   
	shopType = 'butcher',
	price = 10, 
	foodType = 'food',
},


['slicedbologna'] = {
	label = 'Sliced Bologna',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 5,
	},
},

['wholeham'] = {
	label = 'Whole Ham',
	weight = 50,   
	shopType = 'butcher',
	price = 10, 
	foodType = 'food',
},

['bacon'] = {
	label = 'Bacon Strips',
	weight = 50,   
	foodType = 'food',
	shopType = 'butcher',
	price = 10,
	nutrition = {
		protein = 3,
		hunger = 5,
	},
},

['baconbits'] = {
	label = 'Bacon Bits',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 5,
	},
},

['meatslab'] = {
	label = 'Slab of Meat',
	weight = 50,   
	shopType = 'butcher',
	price = 10, 
	foodType = 'food',
},

['nystrip'] = {
	label = 'Raw NY Stip',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 4,
		hunger = 8,
	},
},

['filet'] = {
	label = 'Raw Beef Tenderloin',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 7,
	},
},

['ribs'] = {
	label = 'Ribs',
	weight = 50,   
	shopType = 'butcher',
	price = 10, 
	foodType = 'food',
	nutrition = {
		protein = 4,
		hunger = 8,
	},
},

['hotdog'] = {
	label = 'Hotdogs',
	weight = 50,   
	shopType = 'butcher',
	price = 10, 
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 4,
	},
},

['roastbeef'] = {
	label = 'Roast Beef',
	weight = 50,   
	shopType = 'butcher',
	price = 10, 
	foodType = 'food',
	nutrition = {
		protein = 4,
		hunger = 6,
	},
},

['slicedham'] = {
	label = 'Sliced Ham',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 6,
	},
},

['dicedham'] = {
	label = 'Diced Ham',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 4,
	},
},

['frozennuggets'] = {
	label = 'Frozen Nuggets',
	weight = 50,  
	shopType = 'butcher',
	price = 10,  
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 6,
	},
},

['frozenchickenpatty'] = {
	label = 'Frozen Chicken Patty',
	weight = 50,  
	shopType = 'butcher',
	price = 10,  
	foodType = 'food',
	nutrition = {
		protein = 4,
		hunger = 5,
	},
},

['frozenbeefpatty'] = {
	label = 'Beef Patty',
	weight = 50,  
	shopType = 'butcher',
	price = 10,   
	foodType = 'food',
	nutrition = {
		protein = 4,
		hunger = 6,
	},
},

['pepperoni'] = {
	label = 'Pepperoni',
	weight = 50,  
	shopType = 'butcher',
	price = 10,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 4,
	},
},

['packagedchicken'] = {
	label = 'Packaged Chicken',
	weight = 50,  
	shopType = 'butcher',
	price = 10,   
	foodType = 'food',
},

['venison'] = {
	label = 'Hunting Meat',
	weight = 50,  
	foodType = 'food',
	nutrition = {
		protein = 6,
		hunger = 13,
	},
},

['chickenstrips'] = {
	label = 'Chicken Strips',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 4,
	},
},

['chickenwings'] = {
	label = 'Chicken Wings',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 4,
		hunger = 5,
	},
},

['catfishfilet'] = {
	label = 'Catfish Filet',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 7,
	},
},

['redfishfilet'] = {
	label = 'Redfish Filet',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 7,
	},
},

['salomfilet'] = {
	label = 'Salmon Filet',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 6,
	},
},

['tunafilet'] = {
	label = 'Tuna Filet',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 8,
	},
},

['stripedbassfilet'] = {
	label = 'Stripped Bass Filet',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 5,
	},
},

['rawsquid'] = {
	label = 'Raw Squid',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		protein = 3,
		hunger = 4,
	},
},

-- // Bread/Carbs  // -- 

['breadloaf'] = {
	label = 'Bread Loaf',
	weight = 50,   
	foodType = 'food',
	shopType = 'bakery',
	price = 10, 
},

['flour'] = {
	label = 'Flour',
	weight = 50,   
	foodType = 'food',
	shopType = 'bakery',
	price = 10, 
},

['hotdogbun'] = {
	label = 'Hot Dog Buns',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 4,
		hunger = 3,
	},
},

['burgerbuns'] = {
	label = 'Burger Buns',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 4,
		hunger = 4,
	},
},

['flatbread'] = {
	label = 'Flat Bread',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 4,
		hunger = 3,
	},
},

['bagel'] = {
	label = 'Bagel',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 4,
		hunger = 3,
	},
},

['pizzadough'] = {
	label = 'Yeast',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		carbs = 2,
		hunger = 6,
	}, 
},

['sandwichbread'] = {
	label = 'Sandwich Bread',
	weight = 50,   
	foodType = 'food',
	nutrition = {
		carbs = 3,
		hunger = 2,
	}, 
},

['fettuccine'] = {
	label = 'Fettuccine Noodles',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 5,
		hunger = 4,
	},
},

['spaghetti'] = {
	label = 'Spaghetti Noodles',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 5,
		hunger = 4,
	},
},

['tortellini'] = {
	label = 'Tortellini Noodles',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 5,
		hunger = 4,
	},
},

['linguine'] = {
	label = 'Linguine Noodles',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 5,
		hunger = 4,
	},
},

['lasagna'] = {
	label = 'Lasagna Noodles',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 5,
		hunger = 4,
	},
},

['macaroni'] = {
	label = 'Macaroni Noodles',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 4,
		hunger = 5,
	},
},

['rigatoni'] = {
	label = 'Macaroni Noodles',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 4,
		hunger = 5,
	},
},

['ramen'] = {
	label = 'Ramen Noodles',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 4,
		hunger = 3,
	},
},

['rice'] = {
	label = 'Rice',
	weight = 50,  
	shopType = 'bakery',
	price = 10,   
	foodType = 'food',
	nutrition = {
		carbs = 4,
		hunger = 4,
	},
},

-- // General Market // --

['coffeebean'] = {
	label = 'Coffee Beans',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		sugar = 4,
		thirst = 5,
		seasoning = 2,
	},
},

['ketchup'] = {
	label = 'Ketchup',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		hunger = 2,
		seasoning = 2,
	},
},

['mustard'] = {
	label = 'Mustard',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		hunger = 2,
		seasoning = 2,
	},
},

['bbqsauce'] = {
	label = 'BBQ Sauce',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		hunger = 2,
		seasoning = 4,
	},
},

['mint'] = {
	label = 'Mint',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		hunger = 2,
		seasoning = 3,
	},
},

['sauce'] = {
	label = 'Generic Sauce',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		hunger = 3,
		seasoning = 2,
	},
},

['chips'] = {
	label = 'Potato Chips',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		hunger = 3,
	},
},

['chocolatecandies'] = {
	label = 'Chocolate Candy',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		sugar = 3,
		seasoning = 1,
		hunger = 1,
	},
},

['chocolatesyrup'] = {
	label = 'Chocolate Syrup',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		sugar = 3,
		seasoning = 1,
		hunger = 1,
	},
},

['sprinkles'] = {
	label = 'Assorted Sprinkles',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		sugar = 2,
		seasoning = 1,
		hunger = 1,
	},
},

['candy'] = {
	label = 'Assorted Candies',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		sugar = 2,
		seasoning = 1,
		hunger = 1,
	},
},

['sugar'] = {
	label = 'Sugar',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		sugar = 2,
		seasoning = 2,
		hunger = 1,
	},
},

['brownsugar'] = {
	label = 'Brown Sugar',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		sugar = 2,
		seasoning = 2,
		hunger = 1,
	},
},


['salt'] = {
	label = 'Salt',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 2,
		hunger = 1,
	},
},

['pepper'] = {
	label = 'Pepper',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 2,
		hunger = 1,
	},
},

['basil'] = {
	label = 'Basil',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 2,
		hunger = 1,
	},
},

['chilipowder'] = {
	label = 'Chili Powder',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 3,
		hunger = 1,
	},
},

['cinnamon'] = {
	label = 'Cinnamon',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 3,
		hunger = 1,
	},
},

['garlicpowder'] = {
	label = 'Garlic Powder',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 3,
		hunger = 1,
	},
},

['lemonpeper'] = {
	label = 'Lemon Pepper',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 4,
		hunger = 1,
	},
},

['nutmeg'] = {
	label = 'Nutmeg',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 2,
		hunger = 1,
	},
},

['onionpowder'] = {
	label = 'Onion Powder',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 1,
		hunger = 1,
	},
},

['oregano'] = {
	label = 'Oregano',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 3,
		hunger = 1,
	},
},

['paprika'] = {
	label = 'Paprika',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 2,
		hunger = 1,
	},
},

['pepperflakes'] = {
	label = 'Red Pepper Flakes',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 3,
		hunger = 1,
	},
},

['thyme'] = {
	label = 'Thyme',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 1,
		hunger = 1,
	},
},

['curry'] = {
	label = 'Curry',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'food',
	nutrition = {
		seasoning = 2,
		hunger = 1,
	},
},



-- // Alchol // -- 

['gin'] = {
	label = 'Gin',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'drink',
	nutrition = {
		alcohol = 5,
		thirst = 3,
	},
},

['vodka'] = {
	label = 'Vodka',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'drink',
	nutrition = {
		alcohol = 5,
		thirst = 3,
	},
},

['whiskey'] = {
	label = 'Whiskey',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'drink',
	nutrition = {
		alcohol = 5,
		thirst = 3,
	},
},

['cognac'] = {
	label = 'Cognac',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'drink',
	nutrition = {
		alcohol = 5,
		thirst = 3,
	},
},

['rum'] = {
	label = 'Rum',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'drink',
	nutrition = {
		alcohol = 5,
		thirst = 3,
	},
},

['olives'] = {
	label = 'Olives',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = {'food', 'drink'},
	nutrition = {
		alcohol = 5,
		thirst = 3,
		hunger = 2
	},
},

['tonic'] = {
	label = 'Tonic',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'drink',
	nutrition = {
		alcohol = 5,
		thirst = 3,
	},
},

['carbonatedwater'] = {
	label = 'Cabonated Water',
	weight = 50,  
	shopType = 'general',
	price = 10,   
	foodType = 'drink',
	nutrition = {
		thirst = 7,
	},
},
```
