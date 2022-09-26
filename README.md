---
description: Overview/Guide/Implementation
---

# Unraid OS

## Overview:

Unraid is a Linux based operating system created for media aficionados, gamers, data pursuers, and other intensive data-users to have the ultimate control over their data, media, applications and desktops whilst using any sort of hardware combination.

<figure><img src=".gitbook/assets/111111 (1).PNG" alt=""><figcaption><p>Unraid Product Page</p></figcaption></figure>

## Unraid Home Page

<figure><img src=".gitbook/assets/111111 (1) (1).PNG" alt=""><figcaption><p>Unraid Homepage</p></figcaption></figure>

Unraid Home page is where most of the performance, monitoring and general overview of your unraid server can be seen.

You can see your CPU, Motherboard, Ram and Storage usages and monitoring here on the left and right.&#x20;

Unraid uses something called an "array" where it puts all the storage disks into type of raid where it becomes depenant on each other and writes everything to the parity drive. Array works little different to your typical raid in which it will also write everything thats on the array to the parity drive to almost mirror every other drive in case of an instance that one drive fails that drive can rebuild that drive or become in replace of the failed drive.

Cache drive can also be used, normally done with an ssd to help transfer speeds of data coming on and off the array and sometimes also hold data in its self for usage.

In the middle column you will find all the containers, virtual machines and shares that have been created. Most of these windows/widgets can be customised and moved around to your likeing.

## Main

<figure><img src=".gitbook/assets/111111 (2).PNG" alt=""><figcaption><p>Unraid Main Page</p></figcaption></figure>

This page will consist of the "array" devices, like spoken about be for except this is where you will find most information about your disks and where you will be able to have the most control and modification of them.

In here you can:

* Rename, monitor reading and writing, and storage used for each of the disks
* Stop and Start the array
* Slow and speed up disks
* Reboot, shutdown and sleep the server/drives
* Access to all disks, caches and drive pools

## Shares

<figure><img src=".gitbook/assets/111111.PNG" alt=""><figcaption><p>Unraid Shares Page</p></figcaption></figure>

The shares page will consist of your shares. These are almost like folders in a way that are created within the unraid server. These can then either be: NFS, SMB or FTP exported out to then access it accordingly to the support devices of these formats. Then you can access, copy or move files around into these folder like "shares" to your likeing and have them stored on your server.

Other information is here also like what format the share is currently being exported out too, if its using a cache drive, how much space from the disks is being allocated to that share and as well as what is actually consisting in those shares in real time using the view option on the ride side of the share.

## Users

If you are interested in downloading you can download [here](https://unraid.net/download)! and follow the guide to install!
