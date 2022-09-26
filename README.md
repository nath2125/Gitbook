---
description: Overview/Guide/Implementation
---

# Unraid OS

## <mark style="color:red;">Overview:</mark>

Unraid is a Linux based operating system created for media aficionados, gamers, data pursuers, and other intensive data-users to have the ultimate control over their data, media, applications and desktops whilst using any sort of hardware combination.

<figure><img src=".gitbook/assets/111111 (1) (2).PNG" alt=""><figcaption><p>Unraid Product Page</p></figcaption></figure>

## <mark style="color:red;">Unraid Home Page</mark>

<figure><img src=".gitbook/assets/111111 (1) (1).PNG" alt=""><figcaption><p>Unraid Homepage</p></figcaption></figure>

Unraid Home page is where most of the performance, monitoring and general overview of your unraid server can be seen.

You can see your CPU, Motherboard, Ram and Storage usages and monitoring here on the left and right.&#x20;

Unraid uses something called an "array" where it puts all the storage disks into type of raid where it becomes depenant on each other and writes everything to the parity drive. Array works little different to your typical raid in which it will also write everything thats on the array to the parity drive to almost mirror every other drive in case of an instance that one drive fails that drive can rebuild that drive or become in replace of the failed drive.

Cache drive can also be used, normally done with an ssd to help transfer speeds of data coming on and off the array and sometimes also hold data in its self for usage.

In the middle column you will find all the containers, virtual machines and shares that have been created. Most of these windows/widgets can be customised and moved around to your likeing.

## <mark style="color:red;">Main</mark>

<figure><img src=".gitbook/assets/111111 (2).PNG" alt=""><figcaption><p>Unraid Main Page</p></figcaption></figure>

This page will consist of the "array" devices, like spoken about be for except this is where you will find most information about your disks and where you will be able to have the most control and modification of them.

In here you can:

* Rename, monitor reading and writing, and storage used for each of the disks
* Stop and Start the array
* Slow and speed up disks
* Reboot, shutdown and sleep the server/drives
* Access to all disks, caches and drive pools

## <mark style="color:red;">Shares</mark>

<figure><img src=".gitbook/assets/111111.PNG" alt=""><figcaption><p>Unraid Shares Page</p></figcaption></figure>

The shares page will consist of your shares. These are almost like folders in a way that are created within the unraid server. These can then either be: NFS, SMB or FTP exported out to then access it accordingly to the support devices of these formats. Then you can access, copy or move files around into these folder like "shares" to your likeing and have them stored on your server.

Other information is here also like what format the share is currently being exported out too, if its using a cache drive, how much space from the disks is being allocated to that share and as well as what is actually consisting in those shares in real time using the view option on the ride side of the share.

## <mark style="color:red;">Users</mark>

<figure><img src=".gitbook/assets/111111 (8).PNG" alt=""><figcaption><p>Unraid Users Page</p></figcaption></figure>

In here will consist of any user accounts you create for unraid, these account will be able to access the unraid webgui and also can be adjusted to allow certain users to have access to shares and for transfers and read and write privileges within those shares.

## <mark style="color:red;">Settings</mark>

<figure><img src=".gitbook/assets/111111 (7).PNG" alt=""><figcaption><p>Unraid Settings Page</p></figcaption></figure>

Within the settings page a lot of things can be access and probably way to much to cover, but il cover the basic needs.

Settings its sorted into 4 categorys:

* System Settings
* Network Settings
* User Preferences
* User Utilities

System Settings you will find most things related to the unraid server system its self like: clock, disk settings, performance adjustments, management acess and other things related to the machine and os itself.

Network Settings will consist of more things on the network side like export settings of shares and vpn managers (if one has been setup)

User Preferences is more about how the os looks, how tasks/events are scheduled, how the display looks, etc.&#x20;

User Utilities will show things that can help improve or use the OS better. Like auto app updates, backup/restore, stats, etc. Most plugins that you may install could leave a icon in here as a quick short cut for access.

## <mark style="color:red;">Plugins</mark>

<figure><img src=".gitbook/assets/111111 (4).PNG" alt=""><figcaption><p>Unraid Plugins Page</p></figcaption></figure>

Plugins page will consist of installed plugins that would have installed via apps, updates will also happen here for the plugins.

This tab is pretty self-explainitory :smile:.

## <mark style="color:red;">Docker</mark>

<figure><img src=".gitbook/assets/111111 (1).PNG" alt=""><figcaption><p>Unraid Docker Tab</p></figcaption></figure>

In here all your containers that have been installed via apps just like plugins, will be shown.

It will display information like name, the port number its on, the amount of cpu and ram power being used per container, enabling autostartup upon start up of array, application uptime, etc.

Any configuration, information or monitoring of your containers will most likely be done in here.

## <mark style="color:red;">VMS</mark>

<figure><img src=".gitbook/assets/111111 (6).PNG" alt=""><figcaption><p>Unraid VMs Page</p></figcaption></figure>

VMs page quite self-explainitory also in that this is where you will create, modify and delete any virtual machines you create.

## <mark style="color:red;">Apps</mark>

<figure><img src=".gitbook/assets/111111 (5).PNG" alt=""><figcaption><p>Unraid Apps Page</p></figcaption></figure>

Apps page this is the big marketplace where you can search and install application/containers into your docker.&#x20;

Once installed you will then be able to configure the presettings of the container before it makes the full install onto your machine!

## <mark style="color:red;">Tools</mark>

<figure><img src=".gitbook/assets/111111 (3).PNG" alt=""><figcaption><p>Unraid Tools Page</p></figcaption></figure>

Tools Tab is almost the same as settings but focuses on more utilties tools.&#x20;

Things like:

* Unraid Os (Eg: Diagnostics, config files, processes and system logs)
* Webgui (Eg: Language Change)
* About (Eg: Updating Os, Prechecks)
* System Information (Eg: system info, stats)

Tools for each of these will be found below the according category.

## <mark style="color:red;">Download Link:</mark>

If you are interested in downloading you can download [here](https://unraid.net/download)! and follow the guide to instal!
