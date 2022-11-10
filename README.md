---
description: Overview/Guide
---

# Omada Controller with Ubuntu

## <mark style="color:red;">Overview:</mark>

Omada Controller is a management software for TP-Link EAP devices. With this software, you can use a web browser to centrally manage your EAP devices, such as **configure EAPs in batches and conduct real-time monitoring of EAPs**.

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption><p>Overview Dashboard</p></figcaption></figure>

<mark style="color:purple;">For this example, we are installing this on an instance of Ubuntu.</mark>

## <mark style="color:red;">Guide:</mark>

You will need to start by opening your ubuntu os or instance, and continue over on the terminal window.

Type this in the terminal window:&#x20;

```
sudo apt update && sudo apt install openjdk-8-jre-headless jsvc curl -y
```

This will install the dependencies required for the Omada software

Next type this followed by enter:

```
curl -fsSL https://www.mongodb.org/static/pgp/server-4.4.asc | sudo apt-key add -
```

```
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/4.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.4.list
```

```
sudo apt update && sudo apt install mongodb-org
```

All of these commands will install the necessary MongoDB database required for Omada management software.

### <mark style="color:purple;">Possible Error:</mark>

<mark style="color:purple;">At this point you may fall into an error if you're running an instance, which I am for this example.</mark>

<mark style="color:purple;">Where you may need to type in these commands in order for it to let you to continue your mongodb install.</mark>

```
echo "deb http://security.ubuntu.com/ubuntu focal-security main" | sudo tee /etc/apt/sources.list.d/focal-security.list
```

```
sudo apt-get update
```

```
sudo apt-get install libssl1.1
```

<mark style="color:purple;">Once you have done these continue back to the previous step and reattempt the command and it should let you install with no issues.</mark>

```
sudo apt update && sudo apt install mongodb-org
```

<mark style="color:purple;">Once it has worked successfully you can run this command to remove what we did 2 steps ago to get rid of that error wall.</mark>

```
sudo rm /etc/apt/sources.list.d/focal-security.list
```

Once the installation has worked we need to start the service and also check that its running:

```
sudo systemctl start mongod.service
```

```
sudo systemctl status mongod
```

After the last command, it should give you a status of whether the service is active or not. If you followed the steps correctly it should be listed as active service.

This next command will make sure mongodb is running on start up everytime when this instance or os is booted up. Which will make the process smoother if you going to be regularly using this to host your omada controller.

```
sudo systemctl enable mongod
```

These next command are required for the actual omada tp link software:

```
sudo wget https://static.tp-link.com/upload/software/2022/202203/20220322/Omada_SDN_Controller_v5.1.7_Linux_x64.tar.gz
```

```
tar zxvf Omada_SDN_Controller_v5.1.7_Linux_x64.tar.gz
```

```
cd Omada_SDN_Controller_v5.1.7_Linux_x64/
```

```
sudo bash ./install.sh
```

Once these all have been done and processed you should be good to go!

It will list somewhere after the last command has been processed that you can access the webpage via "localhost:8088" for me that wasn't the case and probably changed due to conflict issues if so if you highlight the link in the terminal it should take you to the browser and automatically redirect you to the correct port number created for the webpage.
