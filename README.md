# SysMonTask  <img align="right" width="100" height="100" src="https://user-images.githubusercontent.com/48773008/108200308-4d170080-7144-11eb-8354-0c528c7b1ac2.png">
[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

<p align="left">
<a href="https://github.com/KrispyCamel4u/SysMonTask/commit-activity">
    <img src="https://img.shields.io/badge/Maintained%3F-yes-green.svg">
</a>

<a href="https://github.com/KrispyCamel4u/SysMonTask/tags/">
    <img src="https://img.shields.io/github/v/tag/KrispyCamel4u/SysMonTask.svg">
</a>
<a href="https://github.com/KrispyCamel4u/SysMonTask/master/LICENSE">
    <img src="https://img.shields.io/github/license/KrispyCamel4u/SysMonTask.svg">
</a>

<a href="https://github.com/KrispyCamel4u">
    <img src="https://img.shields.io/badge/Need%20help%3F-Ask-27B89C">
</a>
</p>

Linux system monitor with the compactness and usefulness of windows task manager to allow higher control and monitoring.

## Installation
To install the binary for ubuntu and its family members **(only for: 16.04,18.04,20.04 and 20.10 and equivalent)**, run: 

***[Need help for packaging for other distros]***

*Note: The process tab works well only for the systems using gnome desktop environment type as of now(support for Mate,Xfce,cinnamon will be added soon)*
```
$ sudo add-apt-repository ppa:camel-neeraj/sysmontask
  ....
$ sudo apt install sysmontask
  ....
$ sysmontask   // optional to run via terminal but recommended for the first time 
```
**If you get the warning about psutil module version(require >=5.7.3) then install the newest one(system-wide) by running:**

```
$ sudo pip3 install -U psutil
  ....
```
**[for Ubuntu<=20.04, the python3-psutil comes with <=5.5.1, hence it is highly recommended to install to the newest one(system-wide)]**

*Note: For Nvidia GPU, nvidia-smi needs to be installed. Check if nvidia-smi is installed by running:*
```
$ nvidia-smi
  ...
```
If not then install it for your system(generally it is automatically installed with nvidia proprietary drivers).

---
Alternatively, if you don't want to add ppa(Personal Package Archives) then download the binaries from releases. And install by double clicking on it.

Then start application from menu or by command "sysmontask"(recommended only in case of error/crashed) on terminal.

Hurray, You're good to go in understanding capabilities of your system:)


## What's New: [![Generic badge](https://img.shields.io/badge/What's_New-History-red.svg)](https://github.com/KrispyCamel4u/SysMonTask/blob/master/HISTORY.md) [![Generic badge](https://img.shields.io/badge/Read_More-Docs-blueviolet.svg)](https://github.com/KrispyCamel4u/SysMonTask/blob/master/DOCS.md)

### v1.1.1-beta
**[Update]**
  * Added support for multiple users processes.
  * About logo icon fixed.
  * Back to zenity for privilege uplifting.
  * Removed auto installing of psutil.
  * hardcode path removed when running from source 
---
- Logical and Overall CPU Utilisation.
- Option to change graph movement(Newer on Left/Newer on Right).
- Icons on Menu.
- Mac Address on Network tab.
- Resident and Shared Memory Columns on performance tab.
- Show/Hide process tab columns(click on column headers).
- [Bug Fix] optimised code.
- [Bug Fix] Refresh not working after Adding a process tab. 
- [Bug Fix] Update speed not working after Adding a process tab.
- [Bug Fix] Graph resizing on full screen.
- [Bug Fix [#2](https://github.com/KrispyCamel4u/SysMonTask/issues/2)] Application crashes start after adding process tab. 
 
**Previous highlight:**
- Processes filtering for user for fast look-ups. ([Read More](https://github.com/KrispyCamel4u/SysMonTask/blob/master/DOCS.md))
- rCPU, rMemory (recursive-CPU,recursive-Memery) columns. ([Read More](https://github.com/KrispyCamel4u/SysMonTask/blob/master/DOCS.md)).


**To set theme, Run:**

By Default sysmontask will use the system-wide setting for themes. If you use any of dark theme(dark mode), that dark theme(dark mode) will be applied to sysmontask. If you use any of light theme(default/light mode), that light theme(default/light mode) will be used by sysmontask. 

To Force apply a particular available theme(light or dark) regardless of system-wide theme, use the below commands:
```
$ sudo sysmontask.set_light
  0 : Raleigh
  1 : HighContrast
  2 : Pop
  3 : Default
  4 : Adwaita
  5 : Emacs
  Index for Corresponding Theme that you want to apply?:2
  Setting of Light Theme Done:)
$ sudo sysmontask.set_dark
  0 : Pop-dark
  1 : Adwaita-dark
  Index for Corresponding Theme that you want to apply?:0
  Setting of Dark Theme Done:)
  ```
This setting will be permanent. If you want to revert back to system-wide theme settings for sysmontask, run:
```
$ sudo sysmontask.set_default
  Setting done:)
```

#### Highlights
![Screenshot from 2021-02-17 17-54-27](https://user-images.githubusercontent.com/48773008/108204170-79814b80-7149-11eb-8b1f-843a1efa8d42.png)

![Screenshot from 2021-02-21 22-06-32](https://user-images.githubusercontent.com/48773008/108631693-1bc66980-7491-11eb-8b1e-59df9622bd32.png)

![Screenshot from 2021-01-24 11-00-18](https://user-images.githubusercontent.com/48773008/105622210-7ab6a580-5e35-11eb-9a43-8f09c0efbdb2.png)

![Screenshot from 2021-02-17 18-09-43](https://user-images.githubusercontent.com/48773008/108212228-a33f7000-7153-11eb-9d3d-2c56d411efc7.png)


### v1.1.0

- User Processess Tab
    * Processes filtering for user for fast look-ups. ([Read More](https://github.com/KrispyCamel4u/SysMonTask/blob/master/DOCS.md))
    * rCPU, rMemory (recursive-CPU,recursive-Memery) columns. ([Read More](https://github.com/KrispyCamel4u/SysMonTask/blob/master/DOCS.md)).
    * Support for aggregate values on coloumn headers.
    * Icon support, Available Killer. 
- Mounted Disk List  
- Can start with different system themes 

### v1.0.0 
- Performance monitoring graphs
- Devices supported:
  * CPU
  * Memory
  * Disks
  * Network adapters
  * only single Nvidia GPU

