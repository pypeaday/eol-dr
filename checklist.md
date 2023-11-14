# End-of-life disaster response

Welp... Nic got ded and now someone has to clean up this tech stuff... I've
made an attempt to have this `TODO` list to help tie off the loose ends.

Contact the following friends and family directly before announcing it on
Twitter...

- Signal: Basically all contacts who I have chats with
- Email: Contact list in Nextcloud (TODO)

Then you can use my computer or phone to hit Twitter up a final tweet:

> Just died. See ya in Heaven or won't. Peace ✌️

Before you get started you'll need one of my YubiKeys... backup one is locked
in firebox if I didn't leave one out (TODO: these are not setup yet so make sure to have my phone with authenticator app on it)

## Tech

This section covers the topics that will help you access my emails and website
logins. It'll also let you know who to give my tech things to or who to ask for
help when something breaks.

### Emails

As you know, I use SimpleLogin.io to alias most of my e-mails. Go to
[dashy.paynepride.com](dashy.paynepride.com) and follow a link to the
SimpleLogin dashboard. If you need to login you will need to check my 2FA app
on my phone (Microsoft Authenticator or Aegis) for a code for simplelogin.

The SimpleLogin dashboard will show you all my email addresses - they all
funnel to my main emails which are logged in SimpleLogin `Mailboxes`

SimpleLogin is a service we use through Proton so you can continue to use it no problem. Proton has a subscription paid for through a Privacy.com card. As of April 2023 we have an organization subscription.

### Domains

- All of my domains are managed in Cloudflare right now. There is a link in dashy to cloudflare homepage. You only need to care about this if you're using `paynepride.com` for any email. For now, and for as long as you want, just keep the autorenewal going - it's like $10/year or something.
- My domains renew through Namecheap automatically via a card in [privacy.com](https://privacy.com).

### Password Managers

You know how to use this since we've incorporated it into our lives.

Note: There's a chance there's some logins owned by my user and not the home organization, my bitwarden login information is in bitwarden so you can find it there and login as me to double check

### Subscriptions

- Twitch.tv – Twitch Prime through Amazon Prime and I have 1 recurring subscription to ThePrimeagen's channel. Payment through Privacy.com card
- Amazon Prime - Autorenews on a privacy.com card
- Netflix - Blocks
- Spotify - Autorenews on a privacy.com card
  - This is a family account so convene with the other users about what to do
- Proton
  - I suggest keeping the Proton stuff. It's autorenewed on a privacy.com card.
- Playstation Plus - cancel this - login is in Bitwarden
- Instacart - Autorenews on a privacy.com card
- DoorDash - Autorenews through privacy.com card

### Homelabs

- DO NOT SELL WITHOUT FORMATTING OR DESTROYING DISKS. This could be an identity theft disaster.

Jeremy will be the biggest help here

1. All the services I run can be managed at portainer.paynepride.com. Remember that you have to be on our network (wireguard, local, or tailscale) to login.

   - Keep the Nextcloud, Dashy, Jellyfin, and Paperless containers up.
   - You'll want to move anything from Nextcloud probably to Proton Drive and use that like Google Drive. The Proton subscription autorenews on a privacy.com card so I'd say lean into it. You can keep Jellyfin up, maybe Hall will know enough to manage it after I died? You should login to paperless (link in Dashy, only available on network) and get all the documents out of it. @Jeremy - you could copy the raw pdfs from the filesystem over to nextcloud... maybe I'll have a python script to do that [here???](TODO)
   - Go through the other services one by one and turn them off (do this like at the end)

2. Church uses Nextcloud. The data is on 1 or 2 computers at church so they
   just need to pick another solution - Google Drive or something. Leave that
   up to them

3. Go through MonicaDB and save what you find relevant somewhere else

4. Most of our important documents are going to be in paperless-ngx. The link
   is on Dashy - follow it and save files as you need to.

### Wireless network

- Jeremy can help setup a regular ol' wifi router. Our Netgear Orbi is being used as Access Points right now, but you can just reset them and use it as the router like we did for a while.
- Otherwise you can keep the OPNSense router up, it's not hard to manage and everything is configured on it for the local network access. Link is on [dashy](dashy.paynepride.com)

### Restarting network services

- If the Internet goes out, restart the router. It's like a desktop pc so you can just hold down the power until it turns off (button's on the front), wait 10 seconds, and start it up again. It takes about 2 minutes to fully power back on.
- If that doesn't work there's probably an actual outage

# TODO: THIS

### Social Media accounts

- Everything can be logged in with Bitwarden + the multi-factor apps on my phone (Microsoft Authenticator or Yubi Authenticator, or Aegis) or my YubiKey
- Don’t close Twitter for a few years
  - If you sell my Twitter, make it worth your time, like 1 million then ask a friend to delete all my old posts

### 2FA

Fortunately, you're familiar with this because I require you to be :blush:.
This is "Two factor authentication" or "2FA" or "Multi factor authentication"
or "MFA". They all mean the same thing.

- I use two MFA apps on my phone
  - Microsoft Authenticator (slowly moving everything over to Aegis)
  - Aegis
  - YubiAuthenticator (TODO: not yet)
- Remember to avoid using SMS for 2FA if it's possible, because it's less safe

### Online Storage & Photo Backups

**Photo Backups**

- All our photos are in Nextcloud. I recommend keeping them there since your phone auto backs up to it. This is dependent on the server though. If you want to move them somewhere then I recommend ProtonDrive.

**Cloud Storage**

# TODO: Regularly tarball or something my paperless-ngx stack and data

# TODO: figure out cloud storage for what makes sense, like docs

### Local Storage & Backups

Like the above online storage and backups we have a NAS, which is the cube-looking black computer in my closet.

This little black box stores all of our backups that we don't want going to the
internet, all of our electronic documents, our films our digital life is on
here so it is **IMPORTANT** that If you decide that you don't want to keep it
contact Jeremy who will help you wipe it (delete everything), whatever you do
don't just throw it in the bin.

- There isn't a specific web portal - but you'll want portainer.paynepride.com, and nextcloud.paynepride.com for most everything.
- The "nas" folder in Nextcloud is everything _not_ in Nextcloud (media/tv/movies, downloads, etc.)
  - There is a `photos` directory in .../nas/media but you can basically ignore it. Everything you care about is in Nextcloud Photos folder.

### Websites

### Tech Tips

- Do not EVER sell anything with a hard drive without formatting the hard drives first. Ask any of our tech friends to help.
  - Or just destroy, like with a drill or saw, all the hard drives that you want to get rid of... seriously... physical destruction

## Input

This is the section where money lands or exists.

### YNAB

1. YNAB is on a Windows Virtual Machine hosted on the NAS. Jeremy can help with moving the VM somewhere (ZFS dataset /tank/encrypted/vms/), or you can just stop using YNAB all together... it's old and installing it anywhere new is tough.
2. YNAB allows 1 desktop install and 2 connected device via Dropbox for automatic syncing. If you want to just install it on a laptop or the regular desktop you use then you'll find the installer on the NAS in /tank/encrypted/nas/dump and the product key is in Bitwarden. Remember that we use an ancient version of YNAB so the installer isn't available anywhere else. Also for the app if you need to reinstall it you have to use the .apk that's also on the NAS which has updated support from the community for Dropbox syncing.
3. I access the windows VM through remmina, username is just `nic`, no password

### Bank Accounts and Virtual Currency

All login info will be in Bitwarden

- CEFCU
  - uses SMS for 2FA so you'll need my phone
  - Checking and Savings accounts
  - Auto loan
  - Job payroll goes here
- Mortage
  - With Finance Of America Mortgage
  - Auto payments are through CEFCU
- Crypto
  - Just call it a loss...
- Privacy cards
  - Most of our bills and such are handled with privacy.com cards.
  - Login to <https://www.privacy.com> (see Bitwarden) and you'll see a dashboard with all the cards. Remember that they are single-merchant only... so the Twitch card is literally only for Twitch and in fact any card will be declined if it's ran with a merchant that it wasnt' setup to be for
- Venmo
  - On my phone - you can transfer all the money to an account and close my venmo
- PayPal
  - Login in Bitwarden
- Fox Communities Credit Union
  - Login in Bitwarden

There's links in Dashy for the girl's 529 plans and all our stuff with Zack. Obviously he/Abri will be the most help here.

### Life Insurance

We have Life Insurance with Northwestern, but just ask Zack and he'll tell you what you need

### Investments

Literally just call Zack

## Output

# TODO

### Ongoing Insurance Accounts

- Auto insurance technically with Traveler's, through Mercer via my work
- Health insurance was through work - hopefully an attorney can help you with this

### Credit Cards

- YNAB has each of our cards with all the scheduled transactions on each one. Logins in Bitwarden
- We pay our credit card balance every month so since there's no real debt there isn't much to worry about, just keep doing what we're doing...

### Cell Phone & Internet

- Verizon (login in Bitwarden)
- Privacy.com card that autopays
- Internet Service Provider is TDS (login in Bitwarden)

### Bill Auto Pay

## Misc

### Financial Advisor

Zack.

### Answers to common security questions

Any security question/identity challenge should be documented in Bitwarden alongside the account

### Physical Security

- Firebox in my office, keys.... somewhere?
