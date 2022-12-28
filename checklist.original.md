# End-of-life disaster response

Welp... Nic got ded and now someone has to clean up this tech stuff... I've
made an attempt to have this `TODO` list to help tie off the loose ends.


Contact the following friends and family directly before announcing it on
Twitter... 

* Signal: Basically all contacts who I have chats with 
> TODO: This
* Email: Contact list in Nextcloud

Then you can use my computer or phone to hit Twitter up a final tweet:

> Just died. See ya in Heaven or won't. Peace ✌️


Before you get started you'll need one of my YubiKeys... backup one is locked
in firebox if I didn't leave one out

## Tech

This section covers the topics that will help you access my emails and website
logins. It'll also let you know who to give my tech things to or who to ask for
help when something breaks.

### Emails

As you know, I SimpleLogin.io to alias most of my e-mails. Go to
[dashy.paynepride.com](dashy.paynepride.com) and follow a link to the
SimpleLogin dashboard. If you need to login you will need to check my 2FA app
on my phone (probably Microsoft Authenticator) for a code for simplelogin.

The SimpleLogin dashboard will show you all my email addresses - they all
funnel to my main emails which are logged in SimpleLogin `Mailboxes`

Add my ProtonMail account to your phone and you will get any emails to any
address in SimpleLogin

### Domains

* All of my domains are managed in CloudFlare right now
* My domains renew through Namecheap automatically via a card in [privacy.com](https://privacy.com)

### Password Managers

You know how to use this since we've incorporated it into our lives.

Bitwarden is however still self-hosted, so you should sign up for the hosted
service at www.bitwarden.com and migrate our data over there - there should be
a simple way to export our vault to JSON and just upload it to Bitwarden
proper. Jeremy can help with this


### Subscriptions

* Twitch.tv – Nothing autorenews, my Twitch Prime is connected to Amazon 
* Amazon Prime - Autorenews on a privacy.com card
* Netflix - Blocks
* Spotify - Autorenews on a privacy.com card
  * Just keep this account since it’s a family account
* Proton
  * I suggest keeping the Proton stuff. It's autorenewed on a privacy.com card. 
  * If I remembered to do it I put all of our non-media stuff in Proton Drive just like Nextcloud
* Playstation Plus - cancel this - login is in Bitwarden

### Homelabs

* DO NOT SELL WITHOUT FORMATTING OR DESTROYING DISKS. This could be an identity theft disaster.

Jeremy will be the biggest help here

1. All the services I run can be managed at portainer.paynepride.com. Remember that you have to be on our network (wireguard, local, or tailscale) to login.

    * Keep the Nextcloud, Dashy, and Bitwarden containers up until Jeremy says they can go down
    * Go through the other services one by one and turn them off (do this like at the end)

2. Church uses Nextcloud. The data is on 1 or 2 computers at church so they
   just need to pick another solution - Google Drive or something. Leave that
   up to them

3. Go through MonicaDB and save what you find relevant somewhere else

4. Most of our important documents are going to be in paperless-ngx. The link
   is on Dashy - follow it and save files as you need to

### Wireless network

* Jeremy can help setup a regular ol' wifi router. Our Netgear Orbi is being used as Access Points right now, but you can just reset them and use it as the router like we did for a while.


### Restarting network services

* If the Internet goes out, restart the black modem by unplugging it, waiting 10 seconds, plugging it back in.
* If that doesn't work, unplug the router, which is probably at this point going to be the Netgear Orbi, and plug it back in.
* If that doesn't work there's probably an actual outage

### Home automation / IoT (Hue, etc)

If you change the name of the wifi (like if you move and use the ISP's built-in wifi), then you will have to reconnect...

# TODO: THIS


### Social Media accounts

* Everything can be logged in with Bitwarden + the multi-factor apps on my phone (Microsoft Authenticator or Yubi Authenticator) or my YubiKey
* Don’t close Twitter for a few years
  * If you sell my Twitter, make it worth your time, like 1 million then ask a friend to delete all my old posts
  * This will probably require some sort of service because Twitter makes things hard
* Double check that my Facebook is 100% deactivated (login in Bitwarden) 

### 2FA

Fortunately, you're familiar with this because I require you to be :blush:.
This is "Two factor authentication" or "2FA" or "Multi factor authentication"
or "MFA". They all mean the same thing.

* I use two MFA apps on my phone
  * YubiAuthenticator 
  * Microsoft Authenticator
* Remember to avoid using SMS for 2FA if it's possible, because it's less safe

### Cloud Subscriptions

SUPER IMPORTANT because these bills can get big quickly


### Online Storage & Photo Backups

**Photo Backups**

* All our photos are in Nextcloud. You'll probably want to move them to something easier like Amazon or something. I'll leave that up to you 
* You can/should copy all those photos to an external hard drive too and plan to keep that updated if you want to maintain storing new photos

**Cloud Storage** 

# TODO: Regularly tarball or something my paperless-ngx stack and data

# TODO: figure out cloud storage for what makes sense, like docs

We have some documents stored on [cloud storage provider], I also have lots of things stored there that you might want to view, TV License receipts, renewal documents for the car things like that. 

* You can login to the web version [here]() details are in KeePass
* From here you can download individual files, change the password etc. 
* Even if you don't use this it is a good idea to keep it as some of the files you might need in the future.

### Local Storage & Backups 

Like the above online storage and backups we have a NAS, which is the cube-looking black computer in my closet.

This little black box stores all of our backups that we don't want going to the
internet, all of our electronic documents, our films our digital life is on
here so it is **IMPORTANT** that If you decide that you don't want to keep it
contact Jeremy who will help you wipe it (delete everything), whatever you do
don't just throw it in the bin.

* There isn't a specific web portal - but you'll want portainer.paynepride.com, and nextcloud.paynepride.com for most everything. 
* The "nas" folder in Nextcloud is everything _not_ in Nextcloud (media/tv/movies, downloads, etc.)
    * There is a `photos` directory in .../nas/media but you can basically ignore it. Everything you care about is in Nextcloud Photos folder.

### Websites


### Tech Tips

* Do not EVER sell anything with a hard drive without formatting the hard drives first. Ask any of our tech friends to help.
  * Or just destroy, like with a drill or saw, all the hard drives that you want to get rid of... seriously... physical destruction

## Input

This is the section where money lands or exists.

### Bank Accounts and Virtual Currency

All login info will be in Bitwarden

* CEFCU 
  * uses SMS for 2FA so you'll need my phone
  * Checking and Savings accounts
  * Auto loan
  * Job payroll goes here
* Mortage
  * With Finance Of America Mortgage
  * Auto payments are through CEFCU
* Crypto
  * Just call it a loss... 
  * Sell everything in crypto.com and Voyager app then transfer USD to the linked bank account - probably CEFU
* Privacy cards
  * Most of our bills and such are handled with privacy.com cards. 
  * Login to https://www.privacy.com (see Bitwarden) and you'll see a dashboard with all the cards. Remember that they are single-merchant only... so the Twitch card is literally only for Twitch and in fact any card will be declined if it's ran with a merchant that it wasnt' setup to be for
* Venmo
  * On my phone - you can transfer all the money to an account and close my venmo
* PayPal
  * Login in Bitwarden 

### Life Insurance

We have Life Insurance with Northwestern, but just ask Zack and he'll tell you what you need


### Investments

Literally just call Zack

## Output

# TODO:

This is the section with bills and things you gotta pay. Everything is on auto-pay so no stress. Just keep money in Fak Bank and United States Bank.

### Ongoing Insurance Accounts

* Auto insurance technically with Traveler's, through Mercer via my work
* Health insurance was through work - hopefully an attorney can help you with this

### Credit Cards and Loans

# TODO

### Cell Phone & Internet

* Verizon (login in Bitwarden)
* Privacy.com card that autopays

### Bill Auto Pay


## Misc

### Financial Advisor

Zack.


### Answers to common security questions

Any security question/identity challenge should be documented in Bitwarden alongside the account

### Physical Security

* Firebox in my office, keys.... somewhere?
