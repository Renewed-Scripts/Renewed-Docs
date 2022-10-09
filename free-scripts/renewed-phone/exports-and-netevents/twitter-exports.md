# 🌀 Twitter Exports

{% hint style="info" %}
Here you can find exports related to twitter for the phone.
{% endhint %}

### AddNewTweet

```
This export can be used for scripts to add announcements into twitter.

Use cases here would be a weather station, or scripts announcing special events?

-- stock export --
exports['qb-phone']:AddNewTweet(TweetData)

-- USAGE --

local TweetData = {
    citizenid = "Fisherman32"
    firstName = "Fisherman",
    lastName = "Paul",
    message = "I like to eat fish every whensday",
    url = "",
    picture = "default",
}

exports['qb-phone']:AddNewTweet(TweetData)
```
