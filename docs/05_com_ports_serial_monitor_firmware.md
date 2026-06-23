\# COM Ports, Serial Monitor, and Firmware



This page explains a very common beginner problem:



The device is connected.



The computer shows a COM port.



But the software still does not record anything.



This can feel confusing at first.



The important lesson is:



> Seeing a COM port does not always mean that useful data is coming from the device.



It only means that the computer can see a serial device.



\---



\## What is a COM port?



On Windows, a COM port is a communication doorway between the computer and a connected device.



For example:



COM3



COM6



COM12



When NPG Lite is connected by USB, Windows may show it as a COM port.



Software can then try to open that COM port and read data from it.



\---



\## COM port detected does not mean signal detected



These are different things:



Device detected by Windows



Device sending text/data



Firmware running correctly



Software reading the correct data



Graph appearing on screen



A beginner may think these are the same, but they are separate steps.



A COM port only tells us that the computer sees something.



It does not prove that the device is sending biosignal samples.



\---



\## What is firmware?



Firmware is the small program running inside the board.



The board does not automatically know what to do.



Firmware tells it things like:



\* which channels to read

\* how fast to sample

\* what format to send data in

\* whether to wait for commands

\* whether to stream continuously



If the wrong firmware is loaded, the board may connect to the computer but still not send the expected data.



\---



\## What is baud rate?



Baud rate is the communication speed used by the device and the computer.



Both sides must use the same speed.



For example, if the firmware uses:



230400 baud



then Arduino Serial Monitor or Python software should also use:



230400 baud



If the baud rate is wrong, the output may be blank, unreadable, or meaningless.



\---



\## What is Arduino Serial Monitor?



Arduino Serial Monitor is a simple window that lets us talk to the board.



It is useful before opening larger software.



Before blaming recording software, first check whether the board responds in Serial Monitor.



For command-based firmware, try commands such as:



HELP



STATUS



START



If the board responds, communication is working.



If there is no response, the problem is earlier in the chain.



\---



\## Line ending matters



Some firmware waits until it receives a complete command.



In Arduino Serial Monitor, the line ending should often be set to:



Newline



or:



Both NL \& CR



If line ending is set to:



No line ending



then the board may not understand the command.



So typing HELP may appear to do nothing.



\---



\## Only one program can use the COM port



A COM port is usually used by only one program at a time.



If Arduino Serial Monitor is open, OpenPhysiologyLab may not be able to use the same COM port.



If Chords Web is using the device, another program may not be able to use it at the same time.



Before testing in another program, close the first one.



\---



\## A useful troubleshooting order



Use this order:



1\. Connect the NPG Lite.



2\. Check which COM port appears in Device Manager or Arduino IDE.



3\. Open Arduino Serial Monitor.



4\. Select the correct COM port.



5\. Set baud rate correctly.



6\. Set line ending to Newline.



7\. Type HELP and press Enter.



8\. Type STATUS and press Enter.



9\. Type START and press Enter.



10\. Look for sample data or firmware response.



Only after this should you open recording software.



\---



\## What does b'' mean in Python?



Sometimes Python shows:



b''



This means Python opened the port but received no bytes before the timeout.



In simple words:



The door opened, but nothing came through.



Possible reasons include:



\* wrong COM port

\* wrong baud rate

\* firmware not streaming

\* command not sent

\* wrong line ending

\* another program using the port

\* board waiting for START command

\* firmware upload problem



\---



\## Common beginner situations



\### Situation 1: COM port appears, but no graph



This means the computer sees the device, but useful data may not be reaching the software.



Check Serial Monitor first.



\### Situation 2: Serial Monitor is blank



Check baud rate, line ending, firmware, board selection, and USB cable.



\### Situation 3: HELP does not respond



Try changing line ending to Newline.



Also confirm the correct firmware is loaded.



\### Situation 4: START works in Serial Monitor but software fails



Close Serial Monitor first.



Then open the recording software.



Only one program should use the COM port at a time.



\---



\## Key idea



A biosignal recording is a chain.



COM port is only one link in the chain.



For successful recording, all these must work together:



device



firmware



USB connection



COM port



baud rate



line ending



software command



data format



graphing software



When you troubleshoot, test one link at a time.



\---



\## Good first success



A good first success is not a perfect ECG.



A good first success is:



The board responds to HELP.



The board responds to STATUS.



The board starts sending data after START.



Once this happens, software recording becomes much easier to understand.



