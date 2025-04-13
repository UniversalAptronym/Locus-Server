To-do: 
Secure communication only section, with dietpi.

### __Surge Protection__

For the safety of your electronics, we highly recommend that all power outlets you plug your equipment to are part of surge-protector, or a power strip with surge protection, to avoid losing your equipment and data to a power surge.

# __Full Home Server (Advanced)__

Install the [Raspberry Pi Imager](../Software_Repository/Raspberry_Pi_Imager.md) on your computer. This lets you turn your Raspbbery Pi from a lump of silicon into a working computer you can talk to.

Slot your SSD into your external SSD enclosure, then plug the enclosure's power supply into a power outlet, then plug the enclosure's USB 3.0 cable into your computer. 

<img src="../Media_Repository/SSD_exposed.jpg" alt="SSD exposed" title="SSD exposed" width="30%"/> <img src="../Media_Repository/SSD_enclosed.jpg" alt="SSD enclosed" title="SSD enclosed" width="30%"/> 

Open up the Raspberry Pi Imager on your computer.

<img src="../Media_Repository/Pi_Imager_search.png" alt="Searching for Pi imager" title="Searching for Pi imager" width="30%"/> <img src="../Media_Repository/Pi_Imager_landing_page.png" alt="Pi imager landing page" title="Pi imager landing page" width="30%"/> 

For `Raspberry Pi Device` select 'Raspberry Pi 5'. For `Choose OS`, select 'Raspberry Pi OS (other)' and then 'Raspberry Pi OS Lite (64 bit)'. For 'Storage' select the SSD you have plugged in. This should be the only device which shows up unless you have other external storage devices plugged in.

<img src="../Media_Repository/Pi_Imager_OS_Other.png" alt="Pi imager OS other" alt="Pi imager OS other" title="Pi imager OS other" width="30%"/> <img src="../Media_Repository/Pi_Imager_OS_Lite.png" alt="Pi imager OS lite" title="Pi imager OS lite" width="30%"/> <img src="../Media_Repository/Pi_Imager_OS_Complete.png" alt="Pi imager OS complete" title="Pi imager OS complete" width="30%"/> 

Click `Next` and then `Edit Settings`. Fill in the settings. **Keep track of your Pi hostname, your Pi username (if different), and your Pi password!!!** These are very important. The Pi hostname will be used to connect to your Pi. The Pi username and password will be used to give commands to your Pi. **Be careful about entering your Pi password. There is no way to tell if you did this wrong.**

Under `Wireless LAN`, for `SSID`, enter the name of your wifi. Under `Wireless LAN`, for `SSID`, enter your wifi password. Click the `Services` tab and make sure you have 'Enable SSH' and 'Use password authentication' enabled. This will ensure you can talk to your Pi through your wifi. Click `Save`, `Yes`, and `Yes`. Wait for the Raspberry Pi Imager to finish writing the Pi OS to your SSD. If your computer asks you if you want to format your device when finished **do not say yes** (this will wipe your Pi device). 

<img src="../Media_Repository/Pi_Imager_OS_settings_1.png" alt="Pi imager OS other" alt="Pi imager OS settings" title="Pi imager OS settings" width="30%"/> <img src="../Media_Repository/Pi_Imager_OS_settings_2.png" alt="Pi imager OS settings" title="Pi imager OS settings" width="30%"/> 

Remove the USB plug of the SSD enclosure from your PC. Make sure your Pi is unplugged from any power outlet. Plug the USB plug of the SSD enclosure into the Pi. Plug your SSD enclosure's power outlet into a power outlet. Plug your Pi into a power outlet. Wait one minute while your Pi boots up. You now have a tiny functioning computer! 

Your next step, to talk to the Pi, is to [use SSH to connect to your Pi](../Instructions/SSH_setup.md).

# __Secure Communication Only (Advanced)__

Plug your micro SD card into your computer. You computer may have a micro SD card slot like this, in which case you can plug it in directly. 

<img src="../Media_Repository/micro_SD_Card_micro-SD-slot.jpeg" alt="micro SD card in slot" title="micro SD card in slot" width="30%"/> 

Your computer may have an SD card slot, in which case you need to put your micro SD card into an SC card adapter (this comes with the purchase of most micro SD cards), then plug that into your computer.

<img src="../Media_Repository/micro_SD_card_stuff.jpg" alt="micro SD card with SD card adapater and USB adapter" title="micro SD card with SD card adapater and USB adapter" width="30%"/> <img src="../Media_Repository/micro_SD_card_in_SD_card_adapter.jpg" alt="micro SD card in SD card adapter" title="micro SD card in SD card adapter" width="30%"/> <img src="../Media_Repository/micro_SD_card_SD-slot.jpg" alt="SD card adapter in slot" title="SD card adapter in slot" width="30%"/> 

If your computer does not have either of those slots, you may need to put your micro SD card in a USB adapter (found in [Equipment_List](../Equipment_List#optional-hardware)), then plug that into your computer.

<img src="../Media_Repository/micro_SD_card_stuff.jpg" alt="micro SD card with SD card adapater and USB adapter" title="micro SD card with SD card adapater and USB adapter" width="30%"/> <img src="../Media_Repository/micro_SD_card_in_USB_adapter.jpg" alt="micro SD card in USB adapter" title="micro SD card in USB adapter" width="30%"/> to-do: last image

to-do: SSH_setup for Secure Communications Only
