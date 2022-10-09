# 📄 How to Install

{% hint style="info" %}
Make sure to follow all steps step by step, if you encounter errors please recheck that you've completed step 1-5 correctly.
{% endhint %}

### Step 1

* Open Renewed-Fuel folder and run the SQL on your database.

### Step 2

* Remove LegacyFuel or any other Fuel Script you used prior
* Insert Renewed-Fuel into your server
* Remember to Ensure Renewed-Fuel in your server.cfg

### Step 3

* Open your Entire server in Visual Studio Code
* Now do a folder search for LegacyFuel (Or any other fuel script you used prior)
* Now Replace it with **Renewed-Fuel**

### Step 4

* Head over to your qb-core folder inside your resources
* Here headover to the shared folder and find items.lua
* Paste following code whereever you like within the QBCore.Shared table

```
['oil_barrel'] 	 = {['name'] = 'oil_barrel', 	['label'] = 'Oil Barrel', 	['weight'] = 80000, 	['type'] = 'item', 	['image'] = 'oil_barrel.png', 	['unique'] = true, 	['useable'] = false, 	['shouldClose'] = false,   ['combinable'] = nil,   ['description'] = 'A barrel used to store types of oil'},
```

### Step 5

* Head over to your qb-inventory (Or any other inventory)
* Paste the oil\_barrel.png into your html/images

### Step 6 (Optional)

These steps is needed if you want the oil barrel to show the current Gasoline inside them

* Headover to your qb-inventory/html/js/app.js
* Now search for harness and it should look like

```
else if (itemData.name == "harness") {
    $(".item-info-title").html("<p>" + itemData.label + "</p>");
    $(".item-info-description").html(
        "<p>" + itemData.info.uses + " uses left.</p>"
    );
}
```

* now replace that code with this

```
else if (itemData.name == "harness") {
    $(".item-info-title").html("<p>" + itemData.label + "</p>");
    $(".item-info-description").html(
        "<p>" + itemData.info.uses + " uses left.</p>"
    );
} else if (itemData.name == "oil_barrel") {
    $(".item-info-title").html('<p>' + itemData.label + '</p>')
    $(".item-info-description").html('<p>' + itemData.info.gas + ' / 5000 Gallons left.</p>');
}
```
