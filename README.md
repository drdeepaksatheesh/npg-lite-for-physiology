# \# NPG Lite for Physiology

# 

# A beginner-friendly guide to understanding biosignal recording with NPG Lite.

# 

# This repository is for physiologists, medical teachers, biology students, MBBS students, postgraduate residents, and curious learners who want to explore ECG, EMG, EOG, EEG, and other physiological signals using accessible tools.

# 

# It is written for people who may not have formally studied electronics, computer science, biomedical engineering, or advanced mathematics.

# 

# That is completely okay.

# 

# You can begin with curiosity.

# 

# You can begin with one small experiment.

# 

# You can begin by asking:

# 

# > “Is my device sending a signal to my computer?”

# 

# That question is already a good beginning.

# 

# \---

# 

# \## Why this repository exists

# 

# Physiology becomes more meaningful when students can see, record, question, and understand signals for themselves.

# 

# Many of us first meet physiology instruments as ready-made systems. We connect electrodes, press buttons, and see a trace on a screen.

# 

# That is useful.

# 

# But there is another layer of learning waiting underneath.

# 

# A physiological signal has a journey:

# 

# ```text

# body → electrode → amplifier → ADC → firmware → computer → software → graph → interpretation

# ```

# 

# When we understand this journey, the machine becomes less mysterious.

# 

# The graph becomes more meaningful.

# 

# The practical becomes more alive.

# 

# This repository is an invitation to explore that journey slowly, safely, and together.

# 

# \---

# 

# \## What is NPG Lite?

# 

# NPG Lite, or Neuro PlayGround Lite, is a compact biosignal acquisition board developed by Upside Down Labs.

# 

# It can be used to explore physiological signals such as:

# 

# \* \*\*ECG\*\*: electrical activity related to the heart

# \* \*\*EMG\*\*: electrical activity from muscle

# \* \*\*EOG\*\*: electrical activity related to eye movement

# \* \*\*EEG\*\*: electrical activity related to the brain

# 

# This repository does not replace the official NPG Lite documentation.

# 

# Instead, it acts as a physiology-first companion for learners who want to understand what the device is doing, how signals reach the computer, and how small experiments can be built around it.

# 

# \---

# 

# \## The spirit of this repository

# 

# This repository is built around a simple idea:

# 

# > Good physiology learning should not require expensive machines before curiosity can begin.

# 

# Accessible tools do not replace careful science.

# 

# They help more people participate in it.

# 

# They allow students and facilitators to ask small, testable questions:

# 

# \* Can I detect a heartbeat?

# \* Can I see muscle activity change during contraction?

# \* Can I understand why a signal is noisy?

# \* Can I compare raw and filtered data?

# \* Can I explain where the graph came from?

# 

# These are not small questions.

# 

# They are the beginning of experimental thinking.

# 

# \---

# 

# \## Who this is for

# 

# This repository is for:

# 

# \* physiology teachers

# \* MBBS students

# \* MD Physiology residents

# \* BSc and MSc biology students

# \* medical researchers

# \* laboratory demonstrators

# \* students who feel intimidated by electronics

# \* teachers who want practical physiology to feel more hands-on

# \* anyone who wants to understand biosignals one step at a time

# 

# The focus is especially on Indian classrooms and laboratories, but the ideas are useful anywhere.

# 

# \---

# 

# \## What this repository is

# 

# This repository is:

# 

# \* a beginner guide

# \* a physiology-first explanation of biosignal recording

# \* a bridge between classical practical physiology and digital recording

# \* a collection of small experiments

# \* a place to document common mistakes and fixes

# \* a learning path for people starting from biology or medicine

# \* a companion to open-source physiology tools such as OpenPhysiologyLab

# 

# \---

# 

# \## What this repository is not

# 

# This repository is not:

# 

# \* an official Upside Down Labs repository

# \* a diagnostic medical guide

# \* a replacement for certified ECG, EMG, EOG, or EEG equipment

# \* a regulatory medical device document

# \* an advanced electronics textbook

# \* a promise that every experiment will work perfectly on the first try

# 

# Learning with real signals includes noise, errors, loose wires, wrong COM ports, blank graphs, and confusing first attempts.

# 

# That is part of the learning process.

# 

# \---

# 

# \## The basic idea

# 

# A biosignal recording system is not magic.

# 

# It is a chain.

# 

# ```text

# human body

# &#x20;  ↓

# electrodes

# &#x20;  ↓

# biopotential amplifier

# &#x20;  ↓

# analog-to-digital converter

# &#x20;  ↓

# firmware

# &#x20;  ↓

# USB / serial / BLE / Wi-Fi

# &#x20;  ↓

# computer software

# &#x20;  ↓

# plot

# &#x20;  ↓

# analysis

# &#x20;  ↓

# interpretation

# ```

# 

# If one part of the chain fails, the signal may disappear, become noisy, or look wrong.

# 

# This repository teaches the chain slowly.

# 

# The aim is not to make everyone an engineer.

# 

# The aim is to help physiology learners understand enough to ask better questions, troubleshoot basic problems, and design better practicals.

# 

# \---

# 

# \## First learning goal

# 

# The first goal is not to record a perfect ECG.

# 

# The first goal is to understand whether the device is communicating with the computer.

# 

# That means learning:

# 

# \* what a COM port is

# \* what firmware is

# \* what Arduino Serial Monitor does

# \* what baud rate means

# \* why a graph can be blank even when a device is connected

# \* why `b''` in Python means no bytes were received

# \* why line endings such as `Newline` can matter

# \* why only one program should use a COM port at a time

# 

# Once communication works, recording becomes much easier to understand.

# 

# \---

# 

# \## Suggested learning order

# 

# Start here:

# 

# ```text

# START\_HERE.md

# ```

# 

# Then read:

# 

# ```text

# docs/01\_what\_is\_npg\_lite.md

# docs/02\_what\_is\_a\_biosignal.md

# docs/03\_ecg\_emg\_eog\_eeg\_without\_fear.md

# docs/04\_electrodes\_amplifier\_adc\_software.md

# docs/05\_com\_ports\_serial\_monitor\_firmware.md

# ```

# 

# Then try the first labs:

# 

# ```text

# labs/lab\_01\_find\_the\_com\_port.md

# labs/lab\_02\_serial\_monitor\_help\_status\_start.md

# labs/lab\_03\_first\_ecg\_headroom\_test.md

# ```

# 

# The order matters.

# 

# Do not begin with complicated recordings.

# 

# Begin by confirming that the device and computer can talk to each other.

# 

# \---

# 

# \## Link with OpenPhysiologyLab

# 

# OpenPhysiologyLab is an open-source physiology recording and analysis application.

# 

# This repository explains the beginner concepts around NPG Lite and biosignal recording.

# 

# OpenPhysiologyLab provides one possible software workflow for recording and analysing signals.

# 

# The two projects are related, but they serve different purposes:

# 

# \* \*\*NPG Lite for Physiology\*\* explains the ideas.

# \* \*\*OpenPhysiologyLab\*\* provides software for recording, analysis, comparison, and documentation.

# 

# \---

# 

# \## A note for facilitators

# 

# This project is not to change everything overnight.

# 

# It can begin gently.

# 

# One small demonstration.

# 

# One student-led session.

# 

# One 60-second ECG recording.

# 

# One discussion about where a signal came from.

# 

# One moment where a learner says, “I think I understand what the machine is doing.”

# 

# That is enough to start.

# 

# A facilitator may be a teacher, postgraduate resident, lab demonstrator, student mentor, or anyone who helps others learn.

# 

# The goal is not to make every physiology lab look like an engineering lab.

# 

# The goal is simpler:

# 

# Help learners move from only seeing a trace to understanding the journey of that trace.

# 

# When students understand the signal chain, practical physiology becomes more active, more honest, and more memorable.

# 

# \---

# 

# \## Safety warning

# 

# Do not use this repository or NPG Lite recordings for diagnosis, treatment, emergency medical decisions, or replacing certified medical equipment.

# 

# Use these materials for:

# 

# \* teaching

# \* learning

# \* experimentation

# \* validation

# \* understanding physiological signals

# 

# Always follow electrical safety, electrode safety, institutional ethics requirements, and local laboratory rules.

# 

# \---

# 

# \## Independence statement

# 

# This is an independent educational repository.

# 

# It is not officially affiliated with, sponsored by, or endorsed by Upside Down Labs unless explicitly stated.

# 

# NPG Lite, BioAmp, Chords, and related names belong to their respective creators.

# 

# Links to official documentation are provided so learners can find the original hardware information.

# 

# \---

# 

# \## Closing thought

# 

# You do not need to understand everything before beginning.

# 

# Start with one signal.

# 

# Start with one wire.

# 

# Start with one question.

# 

# Then build from there.



