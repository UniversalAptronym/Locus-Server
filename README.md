**==================================================**
# __About This Project__
**==================================================**

[Setup and Installation Guide](../../wiki/Setup-and-Installation)

Welcome to the Locus Server project. Our primary goal is to provide an easy to use and affordable method for oppressed and at-risk groups (such as the LGBT+ community and religious or ethnic minorities) to communicate securely without fear of surveillance, censorship, or government violence. Our secondary goal is to make it easier for people to manage and store their own data online, without relying on expensive, intrusive tech monopolies.

This guide will show you how to set up a secure, end-to-end encrypted, self-hosted communication server which includes text, voice, and video chat, and which can be modified to include encrypted, remotely-accessible cloud storage and ad-blocking. In simple terms: You will have a small box. You will plug that box into your house and your wifi. This box will host a website which you can access from anywhere in the world with a web browser or mobile app. This website lets you communicate with other people in a secure, encrypted manner which cannot be intercepted and read en-route. It can also host a website where you can store your data, just like Google Drive, iCloud, or Dropbox. Finally, as a bonus, it can block many advertisers and trackers before they even load on your internet. 

This server facilitates communication which is much more difficult for governments or malicious actors to surveil than other methods, like texting, Facebook Messenger, Instagram, WhatsApp, or Discord. While we suggest the [Signal app](https://signal.org/#signal) as an easier-to-use alternative for secure, end-to-end encrypted communication, it is blocked in some countries (such as [Russia, Venezuela,](https://www.theverge.com/2024/8/9/24217008/signal-blocked-venezuela-russia) [China, and Iran](https://www.techradar.com/news/china-blocks-signal-heres-what-you-need-to-know)). This can be circumvented by a virtual private network (VPN), but those services are often restricted by oppressive governments as well.

While no form of digital communication is definitively secure, encrypted self-hosted communication systems are far more difficult to usefully surveil, interfere with, or ban. Self-hosted servers are infinitely more secure than communicating with programs like WhatsApp or Discord, which can read your messages and regularly cooperate with governments' requests to access users' messages and other data. However, a self-hosted server will not protect you from [FBI spyware installed directly on your computer](https://www.nbcnews.com/id/wbna3341694), if that is used to gain access to your usernames and passwords. The best security is always caution and nothing is foolproof.

Should you build a self-hosted server? It depends. If you're a member of an at-risk group or know people who are, this system could provide a substantial boost to your and/or their safety. If you dislike internet ads, or you pay monthly fees for cloud storage services such as Google Drive, iCloud, and Dropbox, or for encrypted telecommunication services such as Doxy.me and Zoom Business, building a home server may be useful for you.

If you are not part of an at-risk group and don't know anyone who is, you don't care about ads, and you are not paying for cloud or communication services, you may still want to consider self-hosting on privacy grounds. Most major communication programs are neither secure nor private, and often sell your data or give it to the police without a warrant; most online file-storage programs (such as Google Drive, Microsoft OneDrive, and Adobe Creative Cloud storage) store your files unencrypted, and some even use the files you store on them to train AI models. If you, like us, consider this a gross invasion of privacy, then you should consider building a self-hosted server.

*Authors' note, 16 April 2025: This is a new project, and therefore a work in progress. Much of the content is missing from this guide. Please be patient while we fill it out.*

# __Instructions__

Follow these instructions step by step to make a secure communication hub / home server. Each step links to a detailed list of instructions.

Don't be intimidated if this seems like a lot; most of these steps are actually very simple. The reason there's so many lists of instructions is that we try to document each step in as much detail as possible. Most users will probably find themselves bored to tears and rolling their eyes over how much overexplaining is done in the Locus Server project. But our goal is to make it so that _anyone_ can make a home server. Whether you are a novice with computers and need your hand held through each step, or if you're an IT expert who happens to trip over some particular pain point, we don't want anyone to give up on making a home server because we didn't explain it carefully enough.

 1. Decide what you're getting.
    1. [Full Home Server with Cloud Storage and Secure Communication](Equipment_List/Description_Full_Home_Server.md) (~$150-200 + $10/yr)
    2. [Secure Communication Only](Equipment_List/Description_Secure_Communication_Only.md) (~$50-70 + $10/yr)
 2. Buy the equipment you need from [this list](Equipment_List/README.md).
 3. Get a domain name (web URL) and set it up. When you are finished, you and others will access your communication server by going to this URL. [Getting a Domain Name (Web URL).md](Instructions/Getting_a_Domain_Name_(Web_URL).md)
 4. Install the imaging software. This software lets you use your computer to install other software onto your equipment.
    DEV NOTE: (Beginner) is aspirational, for now we're just putting together the resources for (Advanced)
    1. (Beginner) There are prepared images (copies of everything needed to make your Pi a computer with software) and scripts (little programs which will ask you for your inputs) which will let you set everything up painlessly. You will only need to type in things like your wifi name and password, your desired usernames and passwords, your domain name, etc.
    2. ([Advanced](Instructions/Raspberry_Pi_Image_Setup.md)) There is a list of tools and instructions with which you can install a fresh Raspberry Pi OS and add everything you need.
5. [Assemble your Raspberry Pi](Instructions/Raspberry_Pi_Assembly.md).
6. [Image an operating system](Instructions/Raspberry_Pi_Image_Setup.md) onto your Micro SD Card (Secure Communication Only) or your SSD (Full Home Server). These are the storage devices which will hold all the operational software for your equipment.
7. [Install SSH software](Instructions/SSH_setup.md) (this lets your computer talk to your Raspberry Pi during the installation).
8. Log into your Pi and complete the installation.
9. Set up your Databag server. 
10. (For full home server users). Set up your Nextcloud system.
11. Talk to your friends and say hi to others.

# __Usernames and Passwords__

Before we start, you should to decide on certain usernames, passcodes, etc. You will need these later, and they are very important for your security. **Make sure these are usernames and passwords you can remember, which do not rely on simple patterns. If you absolutely must write them down, store them in a secure *offline* location. None of these passwords should be a copy of other passwords you use.** You will need:

## __For regular use__
- **Web URL** (this is the URL you and others will use to access your Pi's services) **(IMPORTANT: This is publically visible and SHOULD NOT MATCH ANY USERNAMES BELOW)**
- **Databag username** (this is your username for the secure communication app) (Important: Do not ever set your browser to autocomplete this username)
- **Databag password** (this is your password for the secure communication app) (Important: Do not ever set your browser to autocomplete this password)
#### __For regular use - Full Home Server Only__
- **CasaOS username** (this is the username you use to log into your Pi through a web browser)
- **CasaOS password** (this is the password you use to log into your Pi through a web browser)
- **Nextcloud username** (this is the username you use to log into your home server storage, and an alternative secure communication service)
- **Nextcloud password** (this is the password you use to log into your home server storage, and an alternative secure communication service)
## __Usernames and passwords you'll need during installation or for changing your system later__
- **Raspberry Pi hostname** (`hostname`.local is the name your Pi goes by when your computer talks to it) 
- **Raspberry Pi username** (this is the username you use to log into your Pi through the terminal) (if you don't know what that is yet, don't worry)
- **Raspberry Pi password** (this is the password you use to log into your Pi through the terminal)
- **Cloudflare email** (this is the email you use for a free account with a service which lets you receive and manage your web URL)
- **Cloudflare password** (this is the password you use to receive and manage your web URL)
- **Nginx email** (this is the email you use for a free account with a service which lets you send your computer passwords without other people intercepting them) 
- **Databag admin password** (this is your administrator password for the secure communication app) **(IMPORTANT: None of these passwords should be the same as the others, but this one MUST BE DIFFERENT THAN THE OTHERS! DO NOT EVER SET YOUR BROWSER TO AUTOCOMPLETE THIS PASSWORD!)**
## __Recorded information__
You will also learn the following information during this installation. You should record this somewhere offline, where you won't lose it.
- Your Raspberry **Pi's local IP address**
- Your network **router's local IP address**
- Your network **router's global IP address**

# __Let's Get Started!__

Click [here](Equipment_List/README.md) to begin your self-hosting journey!
