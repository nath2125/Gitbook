---
description: Overview/Install Guide/Usage Guide
---

# HTTrack Website Archiver

Welcome back to another documentation article.

This one will cover HTTrack Website Copier.

<mark style="color:purple;">Note: This software is available for Windows, Mac, Linux, docker and other platforms via their website:</mark> [<mark style="color:purple;">https://www.httrack.com/</mark>](https://www.httrack.com/)<mark style="color:purple;"></mark>

## <mark style="color:red;">Overview:</mark>

This open-source software is used to crawl the web and in an offline browser allows you to download the HTML page of that website link, for purposes of archiving or downloading an article off the internet for offline usage.

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption><p>Website Homepage</p></figcaption></figure>

## <mark style="color:red;">Installation Guide via Unraid:</mark>

For this installation process, it will be quite easy since its already ready with an installation template within the community AppStore. Note: if you would like to use something like portainer with docker instead and use docker-compose I'm pretty sure they have the link to those files on their website.

Firstly, you want to access the community appstore within unraid and search for Httrack and should look something like this.

<figure><img src=".gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

Once here you can hit action and then install and you will be brought to an installation template page.

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption><p>Installation Template via unraid</p></figcaption></figure>

Here you can keep it pretty default in terms of settings other than inputting where you want the website archives to be stored which will need to be up to you. After that, you are all done and ready to install let the program install and open the WebUI and start archiving.&#x20;

If you have issues which you will see below keep reading otherwise you can skip ahead where i explain how to actually use the program

### <mark style="color:red;">If you have port number issues or the webpage won't load:</mark>

Another critical thing I should mention is that if you run multiple containers within unraid like I do and have a port confliction where another container is using the port this new application is going to use you will run into issues and probably need to redirect which il show how to do here.

since this runs off port 8080 you will need to redirect what port this goes to.

whilst still, in the install template, you want to click the basic view slider and it will go into advanced view. Heading down to the extra parameter section you will already see something there. You want to add "-p 3000:8080" and replace "3000" with another port you don't currently use with another container and then " " (spacebar gap) and paste "-p 3000:8080" this in after you have made those port number small adjustments.

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Probably best also to put that number you replace "3000" within with the WebUI address and replace that default port number in case there's any confusion from the application. After that, you are all done and ready to install let the program install and open the WebUI and start archiving.

## <mark style="color:red;">Usage Guide:</mark>

This is your Starting Page. Following through this guide is pretty easy and will get you on your way to start achieving websites.

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

You want to either create or select an existing project your want these html webpages to be saved in.

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

After this, you will be given a page to attach the links to the website and then will start the process as seen below. Once this is done you will be at the end and you will be able to go now access your offline website HTML via an index link that is attached to the HTTack container.

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption><p>Copier In Progress</p></figcaption></figure>
