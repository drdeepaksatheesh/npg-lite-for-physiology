\# Start Here



Welcome to \*\*NPG Lite for Physiology\*\*.



This repository is for people who want to understand biosignals slowly, practically, and without fear.



You do not need to know electronics before starting.



You do not need to know programming before starting.



You only need to begin carefully.



\---



\## The first idea



A biosignal does not appear on the screen by magic.



It travels through a chain:



```text

body → electrode → amplifier → ADC → firmware → computer → software → graph

```



This repository helps you understand that chain one step at a time.



\---



\## Your first goal



Your first goal is not to record a perfect ECG.



Your first goal is simpler:



> Check whether the NPG Lite is communicating with the computer.



That means learning how to identify the COM port, open Arduino Serial Monitor, set the correct baud rate, and confirm that data is coming from the device.



\---



\## Suggested path



\### Step 1: Understand what NPG Lite is



Read:



```text

docs/01\_what\_is\_npg\_lite.md

```



\### Step 2: Understand what a biosignal is



Read:



```text

docs/02\_what\_is\_a\_biosignal.md

```



\### Step 3: Learn the signal chain



Read:



```text

docs/04\_electrodes\_amplifier\_adc\_software.md

```



\### Step 4: Learn COM ports and Serial Monitor



Read:



```text

docs/05\_com\_ports\_serial\_monitor\_firmware.md

```



\### Step 5: Try the first practical lab



Start with:



```text

labs/lab\_01\_find\_the\_com\_port.md

```



Then:



```text

labs/lab\_02\_serial\_monitor\_help\_status\_start.md

```



Only after this should you try longer recordings.



\---



\## What to expect



Real signals are not always clean.



You may see:



\* no COM port

\* wrong COM port

\* blank Serial Monitor

\* noisy signal

\* loose electrode contact

\* confusing first graphs

\* software that opens but does not record



These are not failures.



They are part of learning how the recording chain works.



\---



\## A good first success



A good first success is:



\* the computer detects the NPG Lite

\* you identify the correct COM port

\* Serial Monitor opens at the correct baud rate

\* the firmware responds to a command

\* you understand one reason why a graph may be blank



That is enough for day one.



\---



\## Safety



Do not use NPG Lite or this repository for diagnosis, treatment, emergency decisions, or replacing certified medical equipment.



Use it for learning, teaching, experimentation, and understanding physiology.



\---



\## Begin gently



Do one step.



Observe.



Write down what happened.



Then do the next step.



That is how experimental physiology begins.



