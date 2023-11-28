# 👩‍💼👨‍💼 Employment Exports (Server Side)

{% hint style="info" %}
Here you can find exports related to employment for the phone.
{% endhint %}

### hireUser

```
This export is used to hire a user in the phone.

-- stock export --
exports['qb-phone']:hireUser(job, citizenId, grade)

-- PARAMETERS --
- job (string): The job or organization to which the user will be hired.
- citizenId (string): The Citizen ID of the player to be hired.
- grade (number): The job grade or position to assign to the user.

-- USAGE --
local citizenId = QBCore.Functions.GetPlayer(source).PlayerData.citizenid
local job = 'taxi'
local grade = 0
exports['qb-phone']:hireUser(job, citizenId, grade)
```

### fireUser

```
This export is used to fire a user in the phone.

-- stock export --
exports['qb-phone']:fireUser(job, citizenId)

-- PARAMETERS --
- job (string): The job or organization from which the user will be fired.
- citizenId (string): The Citizen ID of the player to be fired.

-- USAGE --
local citizenId = QBCore.Functions.GetPlayer(source).PlayerData.citizenid
local job = 'taxi'
exports['qb-phone']:fireUser(job, citizenId)
```
