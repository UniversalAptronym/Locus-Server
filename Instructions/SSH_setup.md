to-do: 
- Check if `pi` and `raspberry` are the default root username and password like this, and if there's a seperate `root` user by default, whose password needs to be changed.
- Add a section about how to change your wifi name and password if those change.
- Include instructions for Macs and Ubuntu.

# __SSH Setup__

SSH means "Secure Shell", referring to the Secure Shell Protocol. An SSH program (like PuTTY) lets you talk to your Pi from your computer in a secure way.

0. In a previous step you created a Pi hostname, Pi username, and Pi password. Make sure you have all three ready for this step.

1. If you are using Windows, download and install [PuTTY](../Software_Repository/SSH.md). Make sure to create a desktop shortcut for PuTTY, and open it up.

<img src="../Media_Repository/Pi_Imager_OS_settings_1.png" alt="Previous screen where you entered your Pi hostname" title="Previous screen where you entered your Pi hostname" width="40%"/>

2. In the field for `Host Name (or IP address)`, enter your Pi hostname followed by ".local", like this `[exampleHostname].local`. This will take you to a mostly black window with only text saying `login as:`. This is known as the "terminal" window. Enter your Pi username and press Enter. Enter your Pi password (no text will appear, this is a normal security measure) and press Enter.
  - If this works, some more text will appear and the bottom line will read `[exampleHostame].[exampleUsername]:~ $`. This means your computer is speaking to a machine named `exampleHostname` (this is your Pi), and you are logged in as `[exampleUsername]`. Additionally, the `~` means you are accessing the home directory of your Pi, and the `$` means you are a normal user.

  - If this does not work you probably got your wifi details wrong in the previous step, or entered the password wrong. If this is the case and retrying your password more carefully does not work, you may have to repeat the previous step with the Raspberry Pi Imager.

<img src="../Media_Repository/PuTTY_username.png" alt="PuTTY username input" title="PuTTY username input" width="30%"/> <img src="../Media_Repository/PuTTY_password.png" alt="PuTTY password input" title="PuTTY password input" width="30%"/> <img src="../Media_Repository/PuTTY_terminal_input.png" alt="PuTTY terminal input" title="PuTTY terminal input" width="30%"/>

3. Next we need to update your Raspberry Pi. Type `sudo apt update` and hit enter. This tells your Pi's Advanced Package Tool (APT) to run an update. `sudo` indicates that you are using administrator privileges to do so (you are telling it to update very sternly). Some text will scroll across your screen, about what is getting updated. When that is finished, type `sudo apt upgrade -y`. This tells your Pi's Advanced Package Tool (APT) to upgrade all of the underlying code packages and modules, and `-y` tells it to say yes to any "are you sure you want to upgrade this?" questions. More text will scroll across your screen, about what is getting updated.

<img src="../Media_Repository/PuTTY_terminal_update_1.png" alt="PuTTY update 1" title="PuTTY update 1" width="40%"/> <img src="../Media_Repository/PuTTY_terminal_update_2.png" alt="PuTTY update 2" title="PuTTY update 2" width="40%"/>

4. Next we need to get your internet router's **local IP address**. If your router's **global IP address** is the mailing address for your piece of the internet, this is the personal name of the doorkeeper who brings the mail in. Type `ip -br route` and press Enter. One of the lines which pops up will say **default via XXX.XXX.XXX.XXX**, where each **XXX** can be 1, 2, or 3 digits. This is your internet router's **local IP address**, record it.

 

5. Finally, we need to give your Raspberry Pi a static **local IP address**. If your router's **global IP address** is the mailing address for your piece of the internet, this is the room your Pi lives in. Normally devices connected to your internet are free to change addresses as needed (crash in whatever room is available), but we need a permanent home for your Pi.
  - First we need to start by getting the **local IP address** for your internet router. Your router is like the doorkeeper who will deliver the letter to the your 
  - Type `sudo nmtui`. 



If all this works, you are ready for the next step. Follow the link below which matches the setup you want.

[Full Home Server](../Instructions/CasaOS_Setup.md) 

Secure Communication Only
