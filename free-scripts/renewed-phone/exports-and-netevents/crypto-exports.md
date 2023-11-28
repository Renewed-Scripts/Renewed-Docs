# 🪙 Crypto Exports (Server Side)

{% hint style="info" %}
Here you can find all exports related to Crypto within the phone!
{% endhint %}

### RemoveCrypto

```
This export is used to remove crypto from a user.

-- STOCK EXPORT -- 
exports['qb-phone']:RemoveCrypto(source, type, amount)

-- PARAMETERS --
- source (number): The player source ID.
- type (string): The type of crypto to be removed.
- amount (number): The amount of crypto to be removed.

-- USAGE --
local source = source
local success = exports['qb-phone']:RemoveCrypto(source, "gne", 50)
print(success)

If the export successfully removes the crypto, the `success` variable will be true; otherwise, it will be false.
```

### hasEnough

```
This export is used to check if a user has enough crypto for a specific purpose.

Note: This function is mainly for niche use cases, as the removal function already includes this check.

-- STOCK EXPORT -- 
exports['qb-phone']:hasEnough(source, type, amount)

-- PARAMETERS --
- source (number): The player source ID.
- type (string): The type of crypto to check.
- amount (number): The amount of crypto needed.

-- USAGE --
local source = source
local success = exports['qb-phone']:hasEnough(source, "gne", 50)
print(success)

If the user has enough crypto, the `success` variable will be true; otherwise, it will be false.
```

### AddCrypto

```
This export is used to add crypto to a player.

-- STOCK EXPORT -- 
exports['qb-phone']:AddCrypto(source, type, amount)

-- PARAMETERS --
- source (number): The player source ID.
- type (string): The type of crypto to be added.
- amount (number): The amount of crypto to be added.

-- USAGE --
local source = source
exports['qb-phone']:AddCrypto(source, "gne", 50)
```
