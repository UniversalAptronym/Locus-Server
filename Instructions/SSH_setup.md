to-do: Check if `pi` and `raspberry` are the default root username and password like this, and if there's a seperate `root` user by default, whose password needs to be changed.

# __SSH Setup__

To-do: Include instructions for Macs and Ubuntu.

SSH means "Secure Shell", referring to the Secure Shell Protocol. An SSH program (like PuTTY) lets you talk to your Pi from your computer in a secure way. If you are using Windows, download and install [PuTTY](../Software_Repository/SSH.md). Make sure to create a desktop shortcut for PuTTY, and open it up.

In a previous step you create a Pi hostname, Pi username, and Pi password. Make sure you have all three ready for this step.

<img src="../Media_Repository/Pi_Imager_OS_settings_1.png" alt="Previous screen where you entered your Pi hostname" title="Previous screen where you entered your Pi hostname" width="40%"/>

In the field for `Host Name (or IP address)`, enter your Pi hostname followed by ".local", like this `[exampleHostname].local`. This will take you to a mostly black window with only text saying `login as:`. This is known as the "Terminal" window. Enter your Pi username and press Enter. Enter your Pi password (no text will appear, this is a normal security measure) and press Enter. If this works, some more text will appear and the bottom line will read `[exampleHostame].[exampleUsername]:~ $`. This means your computer is speaking to a machine named `exampleHostname` (this is your Pi), and you are logged in as `[exampleUsername]`. Additionally, the `~` means you are accessing the home directory of your Pi, and the `$` means you are a normal user.

If this does not work you probably got your wifi details wrong in the previous step, or entered the password wrong. If this is the case and retrying your password more carefully does not work, you may have to repeat the previous step with the Raspberry Pi Imager.

<img src="../Media_Repository/PuTTY_username.png" alt="PuTTY username input" title="PuTTY username input" width="30%"/> <img src="../Media_Repository/PuTTY_password.png" alt="PuTTY password input" title="PuTTY password input" width="30%"/> <img src="../Media_Repository/PuTTY_terminal_input.png" alt="PuTTY terminal input" title="PuTTY terminal input" width="30%"/> 

If this works, you are ready for the next step. Follow the link below which matches the setup you want.

[Full Home Server](../Instructions/CasaOS_Setup.md) 

Secure Communication Only
