---
title: Mac Installation Guide
description: Instructions on how to Install THJ on a Mac
published: true
date: 2025-03-05T19:28:37.788Z
tags: 
editor: markdown
dateCreated: 2025-03-03T12:14:49.040Z
---

![gettingstartedbanner.webp](/gettingstartedbanner.webp){.align-center}

# Mac Installation Guide

Everquest does not natively run on a Mac, and depending on the type of Mac that you have, there are different ways to install and play The Heroes Journey.

<br>

## Recomendations
<br>
 It is recommended that you use a Virtual Machine(VM) when trying to install / run THJ on a M series Mac. While you can use bottle / Wine containers similar to Linux, the packages make it difficult to contain.  
 
> Crossover and other such programs are basically UI skins for Wine and you will run into a lot of potential future problems that it will make it difficult to troublshoot / support. 
 
 If you are on an older Intel Mac, it is recommended that you use boot camp and natively install Windows and run the installer through the bootcamp partition.
 
 ### Recomended VMs
 - By far the best VM for the Mac is [Parallels](https://www.parallels.com/). This is a highly optimzed VM for Macs and runs fully isolated, along with Coherance mode which allows the app to run natively though the Mac and maximize resources.
 	Parallels does cost with a monthly / year subscription, but if you need a Windows resource this is the abxolute best option out there.
  
  - Your next option is [VM Ware Fusion Pro](https://knowledge.broadcom.com/external/article/315638/download-and-install-vmware-fusion.html). While this is free, it has its drawbacks and limitations and is more resource intensive. I would not receommend this if you are not on a Pro or Max series model.
  
  - Final optoin is [Virtual Box](https://www.virtualbox.org/), If your a lover of Oracle products then you can use this. It is the slowest VM in this list, but it works very well on Intel Macs.
  <br>
  ## Prerequisites
 Before you begin, ensure you have the following:
- A Mac running macOS Monterey or later
- A valid Windows ISO file
- Sufficient disk space and RAM for virtualization

## Installing on Parallels
- Create a Windows VM
- Click + New to create a new virtual machine.
- Select Install Windows from image file.Ensure you are using the ARM version of Windows
- Choose your Windows ISO file and follow the installation prompts.
- Configure VM settings (CPU, RAM, Storage) as needed.
- Complete installation and install Parallels Tools.
- It is recommended that you install in the VM like you would any windows application and not in Coherance mode.
- [Install DirectX 9](https://www.microsoft.com/en-us/download/details.aspx?id=8109)
- [Install Steam](https://store.steampowered.com/about/)
- Add Everquest to your Steam Game Library (Do Not Install it)
- [Use the Installer to Install THJ ](https://github.com/The-Heroes-Journey-EQEMU/thj-launcher/releases/download/v1.0.5/THJInstaller-1.0.5.zip) - You will right-click and unzip the file, and then run the .exe in the folder. Allow it, if windows asks if you're sure.
- The patcher should automatically be placed as a shortcut on your dekstop. Run it and it should provide all the needed packages.
- Click play after the patch and enjoy!

 ---

![pagebreak6.webp](/pagebreak6.webp){.align-center}