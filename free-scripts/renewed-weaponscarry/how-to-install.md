# 📄 How to Install

{% hint style="info" %}
Step 2 can be skipped if you do not use qb-apartments
{% endhint %}

### Step 1

Download the latest version of the script

and extract it to your servers root directory

### Step 2

Head over to your qb-apartments and add the following:

`exports['Renewed-Weaponscarry']:toggleProps()`&#x20;

to line 256 right under Wait(250) in the function EnterApartment

Now scroll down till you find `local function LeaveApartment`&#x20;

and paste the following under it (Around line 317)

`exports['Renewed-Weaponscarry']:toggleProps()`

### Step 3

Add the following line to your server.cfg file `ensure Renewed-Weaponscarry`





And that's it! I hope you enjoy the Script!
