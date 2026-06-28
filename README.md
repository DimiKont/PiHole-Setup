
# PiHole-Setup
A guide on how to setup PiHole at home and host it on your Raspberry Pi. It also showcases my own journey with the mistakes I made (breaking stuff is the way. By the way) so that they can hopefully be avoided.

### What is PiHole ?
PiHole is a software that sits on top of a network and basically filters ads. It is a **network-wide ad blocker**. It uses **lists of domains** that download or are related with ads so it can block them. There are some default lists but you can also add custom lists containing other domains.

### How to get started

* First you are going to need a **Raspberry Pi (obviously)**. Anything from as old as a Model 2b (which is what I have) up to a Model 5 will do. PiHole itself and the overall process is not heavy at all so even that 1GB of RAM that the Model 2b has is sufficient. 
* You obviously need **connection** to the **internet** either via WiFi Antenna (Model 2b does not a WiFi module so you will need an antenna) of the good old reliable Ethernet.
* In terms of power supply, a 20W phone charger should be enough to power it on, but if you want you can also use the old-fashioned DC power supply with the little circular cord thing (you know what I mean).
* An **SD Card** to write the operating system to. There might be ways to do it with a live USB stick, but with the SD card you can just write it once, insert it in the slot and just leave it there ( that does not apply if you break the system multiple times like I did and need to literally reinstall it because it is irreversible :( )
* If your laptop or computer that you use to flash the SD does not have a reader by itself, you will need an **SD Reader**.
* **Raspberry Pi Imager software** to write the Raspberry Pi OS into the SD Card.

Lets now look at the process regarding **Raspberry Pi Imager** to flash it.




### Extra
When you connect to a device through SSH and you exchange the ED25519 key/fingerprint, it saves it to `~/.ssh/known_hosts`. If for some reason (definitely did not forgot my old password) you have to reinstall the whole operating system and try to connect to it provided that the IP stays the same, then the ssh will block you thinking that something malicious will happen. You have to edit `~/.ssh/known_hosts` and delete the line that contains the hostname and the IP pair. Then SSH to it and get the new fingerprint. 
