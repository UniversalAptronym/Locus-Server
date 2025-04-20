
# __CasaOS Setup__

If typing into the terminal window was intimidating, don't worry! We exactly have one more line to enter. Type the following line into terminal and press Enter. A lot of text will start scrolling. Wait for this to finish.

Note: Terminal windows often do not accept `ctrl+v` commands to paste content. If you want to paste the following command, you may have to right-click in the terminal window (on some systems this automatically pastes text) or right-click and select paste.

1. `curl -fsSL https://get.casaos.io | sudo bash`

<img src="../Media_Repository/PuTTY_casaos.png" alt="PuTTY CasaOS Install" title="PuTTY CasaOS Install" width="40%"/>

  - This commands installs [CasaOS](https://casaos.io/) from an online repository, and a lot of text will scroll by while it installs. CasaOS is an operating system which will let you operate your Pi through a graphics-based desktop like an ordinary computer, rather than through a terminal, and lets you make use of many programs written by open-source programmers. And speaking of open-source programmers, we have a [list of open-source programers whose work we'd like you to consider supporting](../donations_list.md). Their hard work makes all of this and so much more possible, and they rely on donations to keep the lights on. The whole world benefits from the labor of open source programmers and they deserve all the support we can give them. (The comic below is not a joke. It is stone-cold reality.)

<img src="https://imgs.xkcd.com/comics/dependency.png" alt="XKCD 2347: Dependency" title="XKCD 2347: Dependency" width="40%"/>

2. This is the end of your time with terminal! In the final lines of CasaOS's installation output, you should see `- http://XXX.XXX.XXX.XXX (eth0)`. The **XXX.XXX.XXX.XXX** should be the same as the **local IP address** you gave to your Pi and recorded in the previous section. (Remember that **XXX** represents 1-3 digits, and **(eth0)** may be **(wlan0)** if you opted for a non-ethernet connection.)

<img src="../Media_Repository/CasaOS_Terminal_IP_Address.png" alt="CasaOS Local IP Address" title="CasaOS Local IP Address" width="40%"/> 

