# PiHole-Setup
A guide on how to setup PiHole at home and host it on your Raspberry Pi. It also showcases my own journey with the mistakes I made (breaking stuff is the way. By the way) so that they can hopefully be avoided.

### What is PiHole ?
PiHole is a software that sits on top of a network and basically filters ads. It is a n**etwork-wide ad blocker**. It uses l**ists of domains** that download or are related with ads so it can block them. There are some default lists but you can also add custom lists containing other domains.

### How to get started
First you are going to need a Raspberry Pi (obviously). Anything from as old as a Model 2b (which is what I have) up to a Model 5 will do. PiHole itself and the overall process is not heavy at all so even that 1GB of RAM that the Model 2b has is sufficient. You obviously need connection to the internet either via WiFi Antenna (Model 2b does not a WiFi module so you will need an antenna) of the good old reliable Ethernet. In terms of power supply, a 20W phone charger should be enough to power it on, but if you want you can also 
