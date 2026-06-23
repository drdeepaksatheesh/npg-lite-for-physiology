# Electrodes, Amplifier, ADC, Firmware, and Software

This page explains the signal chain in simple language.

A biosignal does not jump directly from the body to the graph.

It passes through several steps.

Each step matters.

Body

\-> Electrode

\-> Amplifier

\-> ADC

\-> Firmware

\-> Computer

\-> Software

\-> Graph

\-> Interpretation

If the final graph looks wrong, the problem may be anywhere in this chain.

---

## 1. Body

The signal begins in the body.

For example:

- the heart produces electrical activity related to ECG

- muscles produce electrical activity related to EMG

- eye movements produce signals used in EOG

- brain activity contributes to EEG

But these signals are very small at the skin surface.

They need careful recording.

---

## 2. Electrodes

Electrodes are the contact points between the body and the recording system.

They do not create the physiology.

They help detect voltage differences from the body surface.

Electrode quality matters.

A poor electrode contact can cause:

- noise

- baseline wandering

- sudden jumps

- unstable recordings

- no useful signal

Before blaming the software, always check the electrodes.

---

## 3. Skin-electrode contact

The skin-electrode junction is very important.

Good contact helps the signal enter the recording system more reliably.

Poor contact can happen because of:

- dry skin

- loose electrode

- old gel

- hair

- movement

- sweat

- cable pulling

- wrong placement

Many “bad signal” problems are actually contact problems.

---

## 4. Amplifier

Physiological electrical signals are small.

An amplifier makes these small signals large enough to be measured.

But amplification must be done carefully.

If the signal is too small, it may be lost in noise.

If the signal is too large, it may clip.

Clipping means the top or bottom of the signal is cut off because the recording range is exceeded.

A good amplifier helps the signal become visible without distorting it.

---

## 5. Analog signal

Before digital recording, the biosignal is analog.

Analog means it changes continuously with time.

The body does not produce neat rows of numbers.

The board must convert the continuously changing voltage into digital numbers.

That is the role of the ADC.

---

## 6. ADC

ADC means analog-to-digital converter.

It converts the analog voltage into numbers.

For example, instead of saying:

“the voltage is continuously changing”

the ADC gives a stream of digital values such as:

1023

1027

1031

1028

1025

These numbers can be saved, plotted, filtered, and analysed.

---

## 7. Sampling rate

The ADC does not measure the signal continuously.

It samples the signal many times per second.

This is called the sampling rate.

For example:

250 samples per second

500 samples per second

1000 samples per second

A higher sampling rate gives more points per second, but also creates more data.

The required sampling rate depends on the signal and the experiment.

---

## 8. Firmware

Firmware is the small program running inside the board.

Firmware tells the board what to do.

It may control:

- which channels are read

- how fast data is sampled

- whether data streams continuously

- whether the board waits for commands

- what text format is sent to the computer

- how START, STOP, HELP, or STATUS commands behave

If the firmware is wrong, the computer may still show a COM port, but useful data may not appear.

---

## 9. Communication

After the board creates digital data, it must send that data to another device.

This may happen through:

- USB serial

- Bluetooth

- Wi-Fi

Each method has its own behavior.

For beginner troubleshooting, USB serial is often easier to understand because we can test it using Arduino Serial Monitor.

---

## 10. Computer software

Computer software receives the data.

Software may:

- open the COM port

- send commands

- read incoming values

- check data format

- save CSV files

- plot the signal

- filter the signal

- calculate measurements

If the software expects one data format but the firmware sends another, recording may fail.

So firmware and software must speak the same “language.”

---

## 11. Graph

The graph is the final visual result.

But the graph is not the whole story.

A graph may look clean because it has been filtered.

A graph may look noisy because the raw signal is noisy.

A graph may be blank because data never reached the software.

A graph may be inverted because electrode polarity or software display settings changed.

A graph should always be interpreted with knowledge of the recording chain.

---

## 12. Interpretation

Interpretation is the physiology part.

After seeing the graph, we ask:

- What physiological event may have produced this?

- Is the signal expected?

- Is this real activity or artifact?

- Does the signal change with posture, contraction, breathing, or movement?

- Could the recording setup explain the finding?

- Do we need to repeat the experiment?

The machine gives data.

The learner must think.

---

## A simple example: ECG

In ECG recording:

Body: heart electrical activity

Electrodes: placed on body surface

Amplifier: enlarges the small voltage difference

ADC: converts voltage into numbers

Firmware: sends numbers to the computer

Software: plots the waveform

Learner: interprets rhythm, shape, noise, and limitations

This is why ECG is not just a trace.

It is a complete recording chain.

---

## Key idea

Do not trust a graph blindly.

Ask:

How did this graph come into existence?

That question connects physiology, instrumentation, software, and experimental thinking.

---

## Next step

After this, read:

- docs/05\_com\_ports\_serial\_monitor\_firmware.md

Then try:

- labs/lab\_01\_find\_the\_com\_port.md

- labs/lab\_02\_serial\_monitor\_help\_status\_start.md

