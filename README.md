# NPG Lite for Physiology

A beginner-friendly guide to understanding biosignal recording with NPG Lite.

This repository is for physiology, biology, and medical learners who want to explore how body signals such as ECG, EMG, EOG, and EEG become graphs on a screen.

You do not need to be an engineer to begin.

You can start with one small question:

> Is my device sending data to the computer?

That question is already a good beginning.

## Why this repository exists

Physiology becomes more meaningful when learners can see, record, question, and understand signals for themselves.

A physiological signal has a journey:

```text
body -> electrode -> amplifier -> ADC -> firmware -> computer -> software -> graph -> interpretation
```

This repository explains that journey slowly and practically.

## Who this is for

This guide is for:

* physiology teachers and facilitators
* MBBS students
* MD Physiology residents
* biology students
* laboratory demonstrators
* beginners who feel intimidated by electronics or programming
* anyone who wants to understand biosignals one step at a time

The focus is especially on practical physiology learning in Indian classrooms and laboratories, but the ideas are useful anywhere.

## What you can learn here

You can learn:

* what NPG Lite is
* what a biosignal is
* how ECG, EMG, EOG, and EEG are related
* what electrodes, amplifiers, ADCs, firmware, and software do
* what a COM port is
* how to test communication using Arduino Serial Monitor
* why a device may be detected but still not send useful data
* how to begin with small safe experiments

## Start here

Begin with:

[START_HERE.md](START_HERE.md)

Then read:

* [What is NPG Lite?](docs/01_what_is_npg_lite.md)
* [What is a biosignal?](docs/02_what_is_a_biosignal.md)
* [ECG, EMG, EOG, and EEG without fear](docs/03_ecg_emg_eog_eeg_without_fear.md)
* [Electrodes, amplifier, ADC, firmware, and software](docs/04_electrodes_amplifier_adc_software.md)
* [COM ports, Serial Monitor, and firmware](docs/05_com_ports_serial_monitor_firmware.md)

Then try:

* [Lab 01: Find the COM port](labs/lab_01_find_the_com_port.md)
* [Lab 02: Serial Monitor, HELP, STATUS, and START](labs/lab_02_serial_monitor_help_status_start.md)

## Link with OpenPhysiologyLab

This repository explains beginner concepts around NPG Lite and biosignal recording.

OpenPhysiologyLab is a separate open-source physiology recording and analysis project:

https://github.com/drdeepaksatheesh/OPL

The two projects are related, but they serve different purposes:

* **NPG Lite for Physiology** explains the ideas.
* **OpenPhysiologyLab** provides software for recording, analysis, comparison, and documentation.

## A note for facilitators

This project is not asking anyone to change everything overnight.

It can begin gently.

One small demonstration.

One student-led session.

One 60-second ECG recording.

One discussion about where a signal came from.

One moment where a learner says, “I think I understand what the machine is doing.”

That is enough to start.

A facilitator may be a teacher, postgraduate resident, lab demonstrator, student mentor, or anyone who helps others learn.

The goal is simple:

Help learners move from only seeing a trace to understanding the journey of that trace.

## Safety

Do not use this repository or NPG Lite recordings for diagnosis, treatment, emergency decisions, or replacing certified medical equipment.

Use these materials for learning, teaching, experimentation, and understanding physiological signals.

Always follow electrical safety, electrode safety, institutional ethics requirements, and local laboratory rules.

## License

Educational material in this repository is licensed under Creative Commons Attribution-ShareAlike 4.0 International.

See [LICENSE](LICENSE).

## Independence statement

This is an independent educational repository.

It is not officially affiliated with, sponsored by, or endorsed by Upside Down Labs unless explicitly stated.

NPG Lite, BioAmp, Chords, and related names belong to their respective creators.
