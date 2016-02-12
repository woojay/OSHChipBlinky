---
layout: home_no_recents
excerpt: "OSHChip Blinky Tutorial"
tags: [OSHChip, nRF51822, BLE, Bluetooth Low Energy, Bluetooth Smart, Blinky, Tutorial]
categories: [Electronics]
comments: false
modified: 2016-02-09
---

# OSHChip: The Blinky Tutorial

**This short guide will walk you through the toolchain set up and installation of LED blink software on OSHChip**

## Tools you need
- Browser with internet connection
- Computer with MS Windows
- OSHChip


## Tools you will install
- KEIL-MDK 5
- nRF5 SDK Packed version
- nRF5 SDK Zipped version




## 1.  Search for 'KEIL MDK' on a browser.
<BR>
![Googling KEIL MDK](images/1-google-click.PNG)




## 2.  Click on 'MDK Version 5 - Keil'
<BR>
![Selecting MDK Version 5](images/1-1-google-click.PNG)




## 3.  Click on 'Download & Install'
<BR>
![Selecting Download & Install](images/2-keil-click.PNG)




## 4.  Click on 'Download MDK-Core'
<BR>
![Selecting Download MDK-Core](images/2-1-keil-click.PNG)


## 5.  Supply contact information and click on 'Submit'
![Supplying information and selecting Download](images/2-2-keil-click.PNG)


## 5.  Click on '   ' to finally download the latest KEIL-MDK.
<BR>




## 6.  Point your browser to 'http://developer.nordicsemi.com' and click on 'nRF5_SDK' location.
<BR>
![Selecting nRF5_SDK at http://developer.nordicsemi.com](images/3-nordic-dev-click.PNG)




## 7.  Select the latest version of nRF5_SDK (11.x.x in this case)
<BR>
![Selecting nRF5_SDK_v11.x.x](images/3-1-nordic-dev-click.png)




## 8.  Select the Zip file version and then click on 'packs' for packs version. <BR> 
We need both packs and zip versions for this tutorial. <BR>

![Selecting nRF5_SDK .zip file and then packs folder](images/3-2-nordic-dev-click.PNG)




## 9.  Select the packs Zip file
<BR>
![Selecting nRF5_SDK _packs.zip file](images/3-3-nordic-dev-click.PNG)




## 10. Unzip both fils in a directory/folder.  Each file will create its own subdirectory.  The picture shows the installation help for installing Packs (CMSIS Packs).
<BR>
![Installation steps for Packs and Zip file versions](images/3-0-nordic-dev-click.PNG)




## 11.  Connect the hardware.  The BLE radio is connected to a USB power and J-Link adapter is plugged into the programming port.  It may install additional drivers at this point.
<BR>
![Connecting J-Link and radio](images/4-0-HW setup.jpg)





## 12.  Navigate through the Zip file version of the SDK to find the blink program.  It's hidden in examples\peripheral\blinky\pca10028\blank\arm5_no_packs directory.
<BR>
![Selecting blinky program directory](images/4-3-arm5_no_packs.png)





## 13.  Select the blink project file for Keil 5 named 'blinky_blank_pca10028.uvprojx'
<BR>
![Selecting blinky project file](images/4-4-arm5_no_packs.png)




## 14.  Select the main.c file to reveal the main code.
<BR>
![Selecting main.c file](images/4-5-arm5_no_packs.png)
![Selecting main.c file](images/4-6-arm5_no_packs.png)




## 15.  Select 'Configure Flash Tools' under 'Flash' option.
<BR>
![Selecting Configure Flash Tools under Flash option](images/4-7-arm5_no_packs.png)




## 16.  Here's the window that opens for configuration.
<BR>
![A view of the configuration window](images/4-8-arm5_no_packs.png)




## 17.  Select 'Debug' tab.
<BR>
![Selecting Debug Tab or Utilities Tab](images/4-9-arm5_no_packs.png)




## 18.  Select 'J-Link / J-Trace Cortex' on the top right pull-down list.  And then select 'Settings' button.
<BR>
![Selecting J-Link / J-Trace Cortex option and Settings button](images/4-9-arm5_no_packs.png)




## 19.  Select the Debug tab.
<BR>
![Selecting Debug Tab](images/4-11-arm5_no_packs.png)




## 20.  Select the 'Auto Clk' button.
<BR>
![Selecting Auto Clk button](images/4-12-arm5_no_packs.png)




## 21.  Click 'OK' to continue
<BR>
![Selecting OK](images/4-13-arm5_no_packs.png)




## 22.  Exit the configuration and select 'Project' and 'Build Target' (or hit F7) to compile the blinky program
<BR>
![Building / Compiling blinky program](images/4-14-arm5_no_packs.png)




## 23.  No errors or warning shows on the bottom window.
<BR>
![Build Output window](images/4-15-arm5_no_packs.png)




## 24.  Select 'Flash' and 'Download' from the menu (or hit F8).
<BR>
![Selecting Flash and Download options](images/4-16-arm5_no_packs.png)




## 25.  The programmer should send the program hex file to the radio.
<BR>
![Build Output window](images/4-17-arm5_no_packs.png)




## 26.  It works!
<BR>
![Picture of the LED blinking](images/4-18-arm5_no_packs.png)




