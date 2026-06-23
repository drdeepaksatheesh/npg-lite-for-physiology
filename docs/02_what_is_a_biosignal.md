\# What is a Biosignal?



A biosignal is a signal produced by the body that can be measured, recorded, and studied.



Some biosignals are electrical.



Some are mechanical.



Some are chemical.



Some are pressure-related.



Some are related to movement, temperature, or sound.



In this repository, we mostly focus on \*\*electrical biosignals\*\* because NPG Lite is used to record small voltage changes from the body.



\---



\## Simple examples



Here are some common physiological signals:



\* \*\*ECG\*\*: electrical activity related to the heart

\* \*\*EMG\*\*: electrical activity from muscle

\* \*\*EOG\*\*: electrical activity related to eye movement

\* \*\*EEG\*\*: electrical activity related to the brain

\* \*\*PPG\*\*: light-based signal related to blood volume changes

\* \*\*Respiration signal\*\*: movement or flow related to breathing

\* \*\*Blood pressure signal\*\*: pressure changes in blood vessels



All of these are biosignals, but they are not measured in the same way.



Different signals need different sensors, amplifiers, settings, and interpretation.



\---



\## Electrical biosignals



Cells in the body maintain electrical differences across their membranes.



When groups of cells become active, small electrical changes can spread through tissues.



Electrodes placed on the body surface can detect some of these changes.



The voltage changes are usually very small.



That is why we need an amplifier.



\---



\## Why the signal is small



The body is not like a wire carrying a large current.



The electrical activity from the heart, muscles, eyes, or brain becomes weaker by the time it reaches the skin surface.



The signal is also mixed with:



\* skin-electrode contact effects

\* movement artifacts

\* power-line noise

\* muscle noise

\* cable movement

\* sweat

\* loose electrodes

\* environmental electrical interference



So the signal we record is not pure physiology.



It is physiology plus recording conditions.



Understanding this is very important.



\---



\## Signal and noise



A useful biosignal recording contains both:



```text

signal + noise

```



The \*\*signal\*\* is the part we are interested in.



The \*\*noise\*\* is unwanted activity or interference.



For example, during ECG recording:



\* heart-related activity is the main signal

\* muscle tension may add noise

\* loose electrodes may add artifacts

\* mains electricity may add 50 Hz noise in India



A good recording setup tries to improve the signal and reduce the noise.



\---



\## Raw signal and processed signal



A raw signal is the data recorded before much cleaning or filtering.



A processed signal may be filtered, smoothed, scaled, inverted, or transformed.



Both are useful.



The raw signal helps us understand what the device actually recorded.



The processed signal helps us see the pattern more clearly.



A good learner should ask:



\* Am I looking at raw data or filtered data?

\* Was the signal inverted?

\* Was the baseline removed?

\* Was the signal scaled?

\* Were noisy parts hidden?



This habit prevents blind trust in the graph.



\---



\## Biosignal recording is a chain



A biosignal becomes a graph through a chain:



```text

body → sensor/electrode → amplifier → ADC → firmware → computer → software → graph

```



If the graph looks wrong, the problem may be anywhere in the chain.



It may not be the body.



It may be:



\* electrode placement

\* loose contact

\* wrong channel

\* wrong COM port

\* wrong firmware

\* wrong baud rate

\* wrong software setting

\* poor filtering

\* movement artifact



This is why troubleshooting is part of physiology learning.



\---



\## ECG as a beginner example



ECG is often a good first biosignal because:



\* the heart produces a relatively strong electrical signal

\* the pattern is familiar

\* the rhythm can be seen clearly when recording is good

\* students already learn ECG in physiology



But for this repository, the first ECG recording is not mainly about diagnosis.



It is about understanding how a body signal becomes digital data.



\---



\## A useful way to think



Do not ask only:



> Is the graph correct?



Also ask:



> How did this graph come into existence?



That second question is where experimental physiology begins.



\---



\## Next step



After this, read:



\* docs/04\_electrodes\_amplifier\_adc\_software.md

\* docs/05\_com\_ports\_serial\_monitor\_firmware.md



Then try:



\* labs/lab\_01\_find\_the\_com\_port.md

\* labs/lab\_02\_serial\_monitor\_help\_status\_start.md



