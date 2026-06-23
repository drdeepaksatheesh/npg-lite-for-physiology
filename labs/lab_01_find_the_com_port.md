\# Lab 01: Find the COM Port



\## Aim



To identify the COM port used by NPG Lite on a Windows computer.



\---



\## Why this lab matters



Before recording any biosignal, the computer must first detect the device.



On Windows, USB serial devices usually appear as COM ports.



For example:



COM3



COM6



COM12



If the wrong COM port is selected, the software will not receive data from the device.



So the first practical skill is simple:



Find the correct COM port.



\---



\## What you need



\* NPG Lite

\* USB cable

\* Windows computer

\* Arduino IDE or Windows Device Manager

\* Optional: OpenPhysiologyLab



\---



\## Step 1: Disconnect the NPG Lite



First, disconnect the NPG Lite from the computer.



This helps you notice which COM port appears later.



\---



\## Step 2: Open Device Manager



On Windows:



1\. Right-click the Start button.

2\. Click Device Manager.

3\. Look for Ports (COM \& LPT).



If you do not see Ports (COM \& LPT), do not worry.



It may appear after connecting the device.



\---



\## Step 3: Connect the NPG Lite



Now connect the NPG Lite using the USB cable.



Wait a few seconds.



Look again in Device Manager.



A new COM port may appear.



Example:



USB Serial Device (COM6)



or:



USB JTAG/serial debug unit (COM6)



The number may be different on your computer.



\---



\## Step 4: Note the COM port number



Write down the COM port.



Example:



COM6



This is the port you will use in Arduino Serial Monitor or recording software.



\---



\## Step 5: Confirm using Arduino IDE



Open Arduino IDE.



Go to:



Tools → Port



Look for the same COM port.



If the same port appears in Arduino IDE, that is a good sign.



\---



\## Step 6: Disconnect and reconnect test



To confirm, disconnect the NPG Lite.



The COM port should disappear.



Reconnect the NPG Lite.



The COM port should appear again.



This confirms that the COM port belongs to the NPG Lite.



\---



\## Common observations



\### No COM port appears



Possible reasons:



\* USB cable is charge-only

\* driver issue

\* board not powered

\* wrong USB port

\* faulty cable

\* device not recognized

\* board settings issue



Try another USB cable first.



\### Many COM ports appear



Disconnect the NPG Lite and see which port disappears.



Reconnect and see which port returns.



That is usually the correct one.



\### COM port appears but no data comes later



That is a different problem.



A COM port only means the computer sees the device.



It does not prove that the firmware is sending data.



For that, do Lab 02.



\---



\## Record your result



Write down:



Date:



Computer used:



Device used:



COM port detected:



How you confirmed it:



Any problem noticed:



\---



\## Good first success



You have completed this lab if you can say:



The NPG Lite appears as COM\_\_\_ on my computer.



This is enough for Lab 01.



