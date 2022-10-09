# 🪙 Crypto Exports

{% hint style="info" %}
Here you can find all exports related to Crypto within the phone!
{% endhint %}

### RemoveCrypto

```
This export can be used to remove crypto from an user.

-- STOCK EXPORT -- 
exports['qb-phone']:RemoveCrypto(src, type, amount)

-- USAGE --
local src = source
local success = exports['qb-phone']:RemoveCrypto(src, "gne", 50)
print(success)

If the export could remove the crypto then success will return true otherwise false
```

### hasEnough

```
This export is to check if a user has enough crypto for something

This one shouldnt really be used for that much since its build
into the remove crypto function but can be usefull for niché things

-- STOCK EXPORT -- 
exports['qb-phone']:hasEnough(src, type, amount)

-- USAGE --
local src = source
local success = exports['qb-phone']:hasEnough(src, "gne", 50)
print(success)

If you have enough crypto success will be true otherwise false
```

### AddCrypto

```
This export is used to add crypto to a player.

-- STOCK EXPORT -- 
exports['qb-phone']:AddCrypto(src, type, amount)

-- USAGE --
local src = source
exports['qb-phone']:AddCrypto(src, "gne", 50)
```
