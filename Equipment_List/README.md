Note: In addition to this, you will need a web URL, which as of 2024 costs \~$10/yr.

## __Full Home Server with Cloud Storage and Secure Communication__

Note to self: SSD enclosure needs to be powered

## __Secure Communication Only__

As of 2024, the following will cost $50-70. 

#### __Critical Hardware (\~$50)__

Buy a [Raspberry Pi Zero 2 W](https://www.raspberrypi.com/products/raspberry-pi-zero-2-w/) with 

- A case (like [this](https://www.pishop.us/product/aluminum-alloy-protection-case-for-raspberry-pi-zero-series-fits-zero-zero-2-w/))
  - You may also need an extra [heatsink](https://www.pishop.us/product/aluminum-heatsink-for-raspberry-pi-zero/) if your case does not have metal heatsink ridges (rectangular ridges which dissipate heat) and come with thermal putty contacts. (The case above does not need an extra heatsink.)
- A compatible power supply (like [this](https://www.pishop.us/product/wall-adapter-power-supply-micro-usb-2-4a-5-25v/))
- A high quality micro SD card with at least 8 GB of space (the [official Raspberry Pi Micro SD cards with 32 GB](https://www.pishop.us/product/raspberry-pi-sd-card-32gb/) are high quality and will serve well, note that it also comes with a Micro SD to SD card adapter)
  - Note: Do not get a very large SD Card (256+ GB) for more storage. SD Cards do not survive constant file transfers the way SSDs (solid state drives) do and using massive ones for moving and storing many files is prone to failure.

Raspberry Pi Zero 2 W. (left) Bare motherboard. (Middle) Motherboard with thermal putty contacts, which help conduct heat away from the board and into the case. (Right) Pi Zero 2 W fully enclosed in case, with an extra unneeded aluminum heatsink on top. 

<img src="https://github.com/MythicAptronym/Locus-Server/blob/1f74da379c967ed8d3db54ce35241509a0cc6845/Media_Repository/Raspberry_Pi_Zero_2_W_0-Bare.jpg" alt="Bare Raspberry Pi Zero 2 W motherboard" title="Bare Raspberry Pi Zero 2 W motherboard" width="30%"/> <img src="https://github.com/MythicAptronym/Locus-Server/blob/192cb7fa16d6826c81baeb14fbd5af65b4366dee/Media_Repository/Raspberry_Pi_Zero_2_W_1-With-Thermal-Patches.jpg" alt="Raspberry Pi Zero 2 W motherboard and thermal putty contacts" title="Raspberry Pi Zero 2 W motherboard and thermal putty contacts" width="30%"/> <img src="https://github.com/MythicAptronym/Locus-Server/blob/192cb7fa16d6826c81baeb14fbd5af65b4366dee/Media_Repository/Raspberry_Pi_Zero_2_W_2-With-Case.jpg" alt="Raspberry Pi Zero 2 W in case" title="Raspberry Pi Zero 2 W in case" width="30%"/>

#### __Optional Hardware__

- Ethernet to micro USB port (like [this](https://www.amazon.com/Smays-Micro-B-Ethernet-compatible-Raspberry/dp/B01AT4C3KQ?crid=3AITNRWE6DGYE&dib=eyJ2IjoiMSJ9.KXW0YZSm4KBDiJpLS1LFfViXX6o3TTg5mdgEXWTEZ4qTRkA2jV-w-8Bx7lHOZ0At0wyXFVhcq0NoPSvGX_2wdWqYXnCEv9ObFBiP_ovwDuXYuvlW1Zu0FtcqczaHHuVRpWynr9E74ust47HeoQvIIu69XAdwhg1H3z9Ys6lzyTzVcfWmvdBuX7MNudDKbHA2uERN6PgAmEI1y_E81G7Hrh4pkOqZAUq2ppIGxMw5RGY.3yQedQZ0pa9bDT9W7dbYzCo6XzTGR4fYM0f84HP51_A&dib_tag=se&keywords=ethernet+to+micro+usb+adapter&qid=1734673136&sprefix=ethernet+to+mic%2Caps%2C132&sr=8-2)) ($15)
  - This will allow you to use wired ethernet rather than wireless wifi. This allows for faster and more consistent connection.
- SD Card USB Adapter (like [this](https://www.amazon.com/Reader-Adapter-Camera-Memory-Wansurs/dp/B0B9QZ4W4Y?crid=3UGPJK6DS6ZDK&dib=eyJ2IjoiMSJ9.OP-goGzbVTBErEAb5KAgGCjBKA-u0HiCypmciWXnCRgmRE5ZhWDvwdAi_2XUcK0jL_SFjQ4MZWhqaqWC8kp3wYdJ1e6p75mvBgBMb91yRA6v73oRnv2FNBMINxGLaSHPoB8Lsy-aHlXIVakZkXW6UUyA4iiWEqsUIvrpOTs5NKxYXa5HTfle6cKL7AInHXQmJYmBoxLW0MV9AXg7qCqNJ6Y0euFFmyIU_ONiIANMR-0.Y2-4F1iyV_KvIv3bcPtFNsjz4sYLBWfq465lF-pqZ5A&dib_tag=se&keywords=sd+card+usb+adapter&qid=1734674535&sprefix=sd+card+usb%2Caps%2C139&sr=8-3)) ($5)
  - If your computer does not have an SD card or micro SD card reader, you will need one of these.
 
## __Full Home Server__

As of 2024, the following will cost ~$200. 

#### __Critical Hardware (\~$200)__

Buy a [Raspberry Pi 5](https://www.raspberrypi.com/products/raspberry-pi-5/) with at least [4 GB of RAM](https://www.pishop.us/product/raspberry-pi-5-4gb/)

- A case (like [this](https://www.pishop.us/product/raspberry-pi-case-for-pi-5-red-white/), which includes a cooling fan)
  - You should also get extra [heatsinks](https://www.pishop.us/product/set-of-heatsinks-for-raspberry-pi-5-4-pack-copper/)
- A compatible power supply (like [this](https://www.pishop.us/product/raspberry-pi-27w-usb-c-power-supply-white-us/))
- A good quality SSD (solid state drive) with at least 1 TB of space [I (Sengachi) personally use this SSD and it's worked well so far](https://www.amazon.com/Silicon-Power-Performance-Internal-SP002TBSS3A55S25/dp/B07Q37V1C9). High transfer speeds are a plus when considering what SSD card to get, but reliability is the most important thing. Always look up customer reviews from somewhere other than the major sites (like Amazon), which are sometimes faked.
- An [external SSD enclosure](https://www.amazon.com/UGREEN-External-Enclosure-Housing-Adapter/dp/B076WQHK2G) to connect your SSD to your Pi, with a USB 3.0 connector, and which **runs off its own power adapter**. This is very important. Your enclosure should have power adapter with an outlet plug. Many external SSD enclosures operate off of power from their USB 3.0 port; the pi 5 **does not have enough power** to do this.

Raspberry Pi 5 and SSD in an external enclosure. (left) Exposed Pi 5 and SSD. (Right) Enclosed Pi 5 and SSD.
<img src="
https://github.com/MythicAptronym/Locus-Server/blob/8085d56783c51a567b81cf351e39e5aba3026f01/Media_Repository/Raspberry_Pi_5_and_SSD_enclosed.jpg" alt="Exposed Pi 5 and SSD" title="Exposed Pi 5 and SSD" width="40%"/> <img src="https://github.com/MythicAptronym/Locus-Server/blob/bf0e2ada85ff6c71767ff4623db80f89bbf1b27b/Media_Repository/Raspberry_Pi_5_and_SSD_enclosed.jpg" alt="Enclosed Pi 5 and SSD" title="Enclosed Pi 5 and SSD" width="40%"/> 

