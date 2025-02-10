**==================================================**
# __About This Project__
**==================================================**

[Setup and Installation Guide](../../wiki/Setup-and-Installation)

Welcome to the Locus Server project. Our goal is to provide a fairly inexpensive method for oppressed and at-risk groups (such as the LGBT+ community and religious or ethnic minorities) to communicate securely without fear of surveillance, censorship, or government violence.

This guide will show you how to set up a secure, end-to-end encrypted, self-hosted communication server that includes text, voice, and video chat, and can be modified to include encrypted, remotely-accessible cloud storage as well. This server facilitates communication which is *more* difficult for governments or malicious actors to surveil than other methods, like texting, Facebook Messenger, Instagram, WhatsApp, or Discord. While the [Signal app](https://signal.org/#signal) is an easier-to-use alternative for secure, end-to-end encrypted communication, it's blocked in some countries (such as [Russia, Venezuela,](https://www.theverge.com/2024/8/9/24217008/signal-blocked-venezuela-russia) [China, and Iran](https://www.techradar.com/news/china-blocks-signal-heres-what-you-need-to-know). This can be circumvented by a VPN, but those services are often restricted by oppressive governments as well.

While no form of digital communication is definitively secure, encrypted self-hosted communication systems are far more difficult to usefully surveil, interfere with, or ban. The Locus Server is infinitely more secure than communicating with programs like WhatsApp or Discord, which can read every message you've ever sent and regularly cooperate with governments' requests to access users' messages and other data. However, the Locus Server will not protect you from [spyware installed directly on your computer](https://www.nbcnews.com/id/wbna334169) which gains access to your passwords and server account.

Should you build a Locus Server? It depends. If you're a member of an at-risk group or know people who are, this system could provide a substantial boost to your and/or their safety. If you pay monthly fees for cloud storage services such as Google Drive, iCloud, and Dropbox, or encrypted telecommunication services such as Doxy.me and Zoom Business, building a home server may save you money. If you're not paying for these services, you're not part of an at-risk group, and don't know anyone who is, then it depends on how much you value your privacy. Most major communication programs are neither secure nor private, and often sell your data or give it to the police without a warrant; most online file-storage programs (such as Google Drive, Microsoft OneDrive, and Adobe Creative Cloud storage) store your files unencrypted, and some even use the files you store on them to train AI models. If you, like us, consider this a gross invasion of privacy, then you should consider building a Locus.

*Author's note, 29 December 2024: This is a new project, and therefore a work in progress. Much of the content is missing from this guide. Please be patient while we fill it out.*

# __Instructions__

Follow these instructions step by step to make a secure communication hub / home server. Each step links to a detailed list of instructions. 

Also, please don't be intimidated if this seems like a lot; most of these steps are actually very simple. The reason there's so many lists of instructions is that we try to document each step in as much detail as possible. Most users will probably find themselves bored to tears and rolling their eyes over how much overexplaining is done in the Locus Server project. But our goal is to make it so that _anyone_ can make a home server. Whether because you're a novice with computers and need your hand held through each step, or because you trip over something specific, we don't want anyone to give up on making a home server because we didn't explain it carefully enough.

 1. Decide what you're getting.
    1. [Full Home Server with Cloud Storage and Secure Communication](Equipment_List/Description_Full_Home_Server) (~$200 + $10/yr)
    2. [Secure Communication Only](Equipment_List/Description_Secure_Communication_Only) (~$50-70 + $10/yr)
 2. Buy the equipment you need from [this list](Equipment_List).
 3. Get a domain name (web URL) and set it up. When you are finished, you and others will access your communication server by going to this URL. [Getting a Domain Name (Web URL).md](Internet_Actions/Getting_a_Domain_Name_(Web_URL).md)
 4. Install the imaging software. This software lets you use your computer to install other software onto your equipment.
    DEV NOTE: (Beginner) is aspirational, for now we're just putting together the resources for (Advanced)
    1. (Beginner) There are prepared images (copies of everything needed to make your Pi a computer with software) and scripts (little programs which will ask you for your inputs) which will let you set everything up painlessly. You will only need to type in things like your wifi name and password, your desired usernames and passwords, your domain name, etc.
    2. ([Advanced](Software_Repository/Raspberry_Pi_Imager.md)) There is a list of tools and instructions with which you can install a fresh Raspberry Pi OS and add everything you need.
5. [Assemble your Raspberry Pi](Instructions/Raspberry_Pi_Assembly).
6. Image your Micro SD Card (Secure Communication Only) or your SSD (Full Home Server). These are the storage devices which will hold all the operational software for your equipment.
7. Install SSH software (this lets your computer talk to your Raspberry Pi during the installation).
8. Log into your Pi and complete the installation.
9. Set up your Databag server. 
10. (For full home server users). Set up your Nextcloud system.
11. Talk to your friends and say hi to others.
