# Basic Home Lab Running Active Directory

This repository contains steps on how i set up a basic home lab running Active Directory

## Diagram
![Diagram](https://i.imgur.com/DuZohlX.png)

## Download and install Oracle VirtualBox from the official website.
[Oracle Virtual Box](https://www.virtualbox.org/)

## Download the Windows 10 and Server 2019 ISO files.
[Windows 10 iso](https://www.microsoft.com/en-us/software-download/windows10ISO)
[Windows Server 2019](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)

## Create a new virtual machine by clicking on "New" in VirtualBox, naming it "Domain Controller," and selecting the "Windows Server 2019" ISO file as the boot media.

![](https://i.imgur.com/pBfdTVs.png)

![](https://i.imgur.com/Gnw6NCM.png)

##  Configure the virtual machine by giving it two network adapters: one for connecting to the internet and the other for the private network.

![](https://i.imgur.com/9YkM5O3.png)

![](https://i.imgur.com/UJXFUmo.png)

##  Install Server 2019 on the virtual machine and assign IP addressing for the internal network.

![](https://i.imgur.com/yyG9DZv.png)

![](https://i.imgur.com/TvpEAer.png)
##  Name the server and install Active Directory to create the domain.
![](https://i.imgur.com/eduYSoW.png)

![](https://i.imgur.com/kj3qur5.png)

##  Configure routing so that clients on the private network can access the internet through the domain controller.

![](https://i.imgur.com/5SzRiHd.png)

![](https://i.imgur.com/5bIfLgn.png)

![](https://i.imgur.com/WeLJqg5.png)

##  Set up DHCP on the domain controller.
![](https://i.imgur.com/m4xFQKl.png)

![](https://i.imgur.com/WpjjWBU.png)

![](https://i.imgur.com/Tz93rfA.png)


##  Run the PowerShell script to create 1000 users in Active Directory.

[Power Shell script for creating users](https://github.com/joshmadakor1/AD_PS)

##  Create a new virtual machine named "Client1" and install Windows 10 on it.

![](https://i.imgur.com/LFazRDt.png)


##  Connect the client machine to the private network and join it to the domain.

![](https://i.imgur.com/W6ig3tj.png)

![](https://i.imgur.com/f7C5crq.png)

##  Log into the client machine with a domain account.

![](https://i.imgur.com/zIL4wuF.png)

![](https://i.imgur.com/7N0cAhi.png)
