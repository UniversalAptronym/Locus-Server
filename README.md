# __Secure Communication__

This is a guide for how to set up secure, self-hosted communication, including text, voice, and video chat, which is much more difficult\* for governments to surveil or for corporations to harvest data from than typical texts or social media (such as Facebook, Discord, Tumblr, etc). "Self-hosted" means that you physically own and operate the equipment which transmits and stores messages, and "secure" means the messages are encrypted - they cannot be read by anyone who intercepts the messages en-route. 

That said, the [Signal](https://signal.org/download/) app is a secure texting, voice, and video chat service, which is easier to use than self-hosting. We highly recommended using it. However, [China has blocked Signal](https://www.techradar.com/news/china-blocks-signal-heres-what-you-need-to-know), making impossible to access without a VPN (service which alters your apparent digital location) which [China has also been cracking down on](https://www.farwestchina.com/tips/best-vpn-for-china/). Such services can be interfered with and censored by governments.

A self-hosted communication system is much more difficult to interfere with or ban. It is the goal of this project to enable oppressed and at-risk groups, such as queer people and ethnic minorities, to communicate securely without fear of surveillance, censorship, or government violence. Spreading information about how to set up secure self-hosted communication is the best way we know to do this.

\*No form of communication, online or otherwise, is definitively secure. This will not protect you from the [FBI installing spyware onto your computer](https://www.nbcnews.com/id/wbna3341694) and using that to gain access to your passwords and communications. However it's infinitely more secure than communicating by text, or on Facebook, Discord, WhatsApp, etc, all of which can and do cooperate with government requests to access user messages and other data.

As a perk, the process to set up secure self-hosted communication overlaps very heavily with the process of setting up a full home server with self-hosted cloud storage, and this guide will show you how to do that as well. That is, you can have your own Google Drive / iCloud / DropBox without needing to pay exhorbitant monthly fees. This can save a good deal of money on cloud storage and avoids dependence on data-mining entities such as Google and Apple to store one's files. If you use this guide to do so, even if you yourself have no need for secure communication, please consider passing it on to those in your life who may be the targets of bigotry and institutional violence. 

Even if you don't think they will need it, gestures such as these, reaching out and affirming a desire to help, are never without merit or appreciation. 

### __How-To List__

 1. Decide what you're getting.
    1. [Full Home Server with Cloud Storage and Secure Communication](https://github.com/MythicAptronym/Locus-Server/blob/212890bef63c699d6c49c2edd7390ee65c048aed/Equipment_List/Description_Full_Home_Server) (~$200 + $10/yr)
    2. [Secure Communication Only](https://github.com/MythicAptronym/Locus-Server/blob/212890bef63c699d6c49c2edd7390ee65c048aed/Equipment_List/Description_Secure_Communication_Only) (~$50-70 + $10/yr)
 2. Buy the equipment you need. [Equipment List.md](https://github.com/MythicAptronym/Locus-Server/tree/d38cfb39f7593207ba383d74bd4478b6912eef67/Equipment_List)
 3. Get a domain name (web URL) and set it up. When you are finished, you and others will access your communication server by going to this URL. [Getting a Domain Name (Web URL).md](https://github.com/MythicAptronym/Locus-Server/blob/1f998997e4ccb97da92ac3ed4df4e2114b61cde0/Internet_Actions/Getting_a_Domain_Name_(Web_URL).md)
 4. Install the [imaging software](https://github.com/MythicAptronym/Locus-Server/blob/184a7ed74ee198dd9b6999579d1d71227d94f644/Software_Repository/README.md). This software lets you use your computer to install other software onto your equipment.
    DEV NOTE: (Beginner) is aspirational, for now we're just putting together the resources for (Advanced)
    1. (Beginner) There are prepared images (copies of everything needed to make your Pi a computer with software) and scripts (little programs which will ask you for your inputs) which will let you set everything up painlessly. You will only need to type in things like your wifi name and password, your desired usernames and passwords, your domain name, etc.
    2. (Advanced) There is a list of tools and instructions with which you can install a fresh Raspberry Pi OS and add everything you need.
 6. Image your Micro SD Card (Secure Communication Only) or your SSD (Full Home Server). These are the storage devices which will hold all the operational software for your equipment.
 7. Assemble your Raspberry Pi.
 8. Install the SSH software (this lets your computer talk to other computers).
 9. Log into your Pi and complete the installation.
 10. Set up your Databag server. 
 11. (For full home server users). Set up your Nextcloud system.
12. Talk to your friends and say hi to others.
