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

-- PARAMETERS --
- TweetData (table): A table containing the following information for the new tweet:
  - citizenid (string): The Citizen ID or identifier of the tweet author.
  - firstName (string): The first name of the tweet author.
  - lastName (string): The last name of the tweet author.
  - message (string): The content of the tweet message.
  - url (string): A URL associated with the tweet (optional).
  - picture (string): The picture associated with the tweet. Use "default" for the default Twitter profile picture (optional).

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
