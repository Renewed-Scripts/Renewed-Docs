# 🔔 Notifications Exports (Client Side)

{% hint style="info" %}
Here you can find exports related to notifications for the phone.
{% endhint %}

### PhoneNotification

```
This export can be used to send a notification to the phone of a player

-- stock export --
local success = exports['qb-phone']:PhoneNotification(title, text, icon, color, timeout, accept, deny)

-- PARAMETERS --
- title (string): The title of the notification.
- text (string): The main text content of the notification.
- icon (string): The icon to be displayed with the notification (FontAwesome icon class).
- color (string): The color of the notification.
- timeout (string or number): The duration for which the notification will be displayed. It can be a string like "short" or "long," or a specific time in milliseconds.
- acceptIcon (string): The icon for the accept action (FontAwesome icon class).
- denyIcon (string): The icon for the deny action (FontAwesome icon class).

-- USAGE --
local title = 'PING'
local text = info.Name .. ' Incoming Ping'
local icon = 'fas fa-map-pin'
local color = '#b3e0f2'
local timeout = 'NONE'  -- Can be 'short', 'long', or a specific duration in milliseconds
local acceptIcon = 'fas fa-check-circle'
local denyIcon = 'fas fa-times-circle'

local success = exports['qb-phone']:PhoneNotification(title, text, icon, color, timeout, acceptIcon, denyIcon)
```
