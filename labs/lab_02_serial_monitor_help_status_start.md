# Lab 02: Serial Monitor, HELP, STATUS, and START

## Aim

To check whether NPG Lite is communicating with the computer through Arduino Serial Monitor.

---

## Why this lab matters

In Lab 01, we found the COM port.

That only proves that the computer can see the device.

It does not prove that the board is sending useful data.

In this lab, we ask a better question:

> Is the board responding to commands?

This is an important step before using recording software.

---

## What you need

- NPG Lite

- USB cable

- Windows computer

- Arduino IDE

- COM port found in Lab 01

---

## Step 1: Close other programs

Before opening Arduino Serial Monitor, close any other program that may be using the NPG Lite.

Close:

- OpenPhysiologyLab

- Chords Web

- any other serial monitor

- any Python script reading the COM port

Only one program should use the COM port at a time.

---

## Step 2: Open Arduino IDE

Open Arduino IDE.

Go to:

Tools → Port

Select the COM port found in Lab 01.

Example:

COM6

Your COM port may be different.

---

## Step 3: Open Serial Monitor

In Arduino IDE, open Serial Monitor.

Set the baud rate to:

230400

This number must match the firmware.

If the baud rate is wrong, the output may be blank or unreadable.

---

## Step 4: Set line ending

In Serial Monitor, set line ending to:

Newline

or:

Both NL & CR

Do not use:

No line ending

Some firmware waits for a complete command. Without the correct line ending, the board may not understand the command.

---

## Step 5: Send HELP

Type:

HELP

Then press Enter.

A working command-based firmware should respond with a list of commands or help text.

If there is no response, do not move to recording software yet.

First fix communication.

---

## Step 6: Send STATUS

Type:

STATUS

Then press Enter.

The board may respond with information about its current state.

This can help confirm that the firmware is alive and responding.

---

## Step 7: Send START

Type:

START

Then press Enter.

If the firmware is working and streaming is enabled, sample data may begin to appear.

The data may look like rows of numbers.

That is a good sign.

It means the board is sending data to the computer.

---

## Step 8: Stop if needed

If the firmware supports a stop command, type:

STOP

Then press Enter.

If not, close Serial Monitor or disconnect the board safely.

---

## What a good result looks like

A good result is:

- Serial Monitor opens

- correct COM port is selected

- baud rate is set correctly

- line ending is set correctly

- HELP gives a response

- STATUS gives a response

- START begins data streaming

This means the computer and board are communicating.

---

## If Serial Monitor is blank

Check these one by one:

- Is the correct COM port selected?

- Is the baud rate correct?

- Is line ending set to Newline?

- Is another program already using the COM port?

- Is the USB cable working?

- Is the correct firmware uploaded?

- Is the board selected correctly in Arduino IDE?

- Does the board need to be reset?

Do not guess many things at once.

Change one thing, then test again.

---

## If COM port opens but no data appears

This means the computer may see the board, but the firmware may not be sending data.

Possible reasons:

- firmware is waiting for START

- wrong firmware is loaded

- wrong baud rate

- wrong line ending

- board needs reset

- another program is using the port

- firmware upload did not happen correctly

---

## If data appears after START

That is a useful success.

Now close Serial Monitor before opening recording software.

If Serial Monitor remains open, recording software may not be able to use the COM port.

---

## Record your result

Write down:

Date:

Computer used:

NPG Lite used:

COM port:

Baud rate:

Line ending:

Did HELP respond?

Did STATUS respond?

Did START produce data?

Problems noticed:

---

## Good first success

You have completed this lab if you can say:

The board responded in Serial Monitor.

or:

The board started sending data after START.

That is enough for Lab 02.

The next step is to use this same communication chain inside recording software.

