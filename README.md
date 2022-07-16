# Welcome to Rubber Ducky! <img src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" width="30px">

# Rasberry Pi Rubber Ducky

This repo is for rubber ducky exploration and proof of concepts around this type of tool.

### What is a Rubber Ducky?

A Rubber Ducky is a keystroke injection tool that is often disguised as a USB flash drive to trick an unsuspecting victim into plugging it into their computer. The computer recognizes the Rubber Ducky as a USB keyboard (and mouse if required), and when it is plugged in, it executes a sequence of pre-programmed keystrokes, which will be executed against the target computer, as if the user did it. This attack thus exploits the security roles and permissions assigned to the user logged in at the time.

### What are Key Stroke Injection attacks?

[Read about Keystroke injections attacks here](https://docs.hak5.org/usb-rubber-ducky-1/getting-started/keystroke-injection-attacks)

## Installation

To create the Pico Rubber Ducky, you will need four things:

```bash
1. A Rasberry Pico
2. A Micro USB Cable
3. CircuitPython
4. The Adafruit HID Library of CircuitPython
```

Full Instructions for how to set up a rasberry pi pico as a rubber ducky: [Read Here](https://www.instructables.com/Rickroll-People-With-a-Raspberry-Pi-Pico/)

## Usage

Once your pico rubber ducky is set up you can now config the the tool to run a series os scripts. There is a library that has a plethora of pre-written scripts to get jump started.

[Payload Scripts are here](https://github.com/hak5darren/USB-Rubber-Ducky/wiki/Payloads)

### Example

Example from the above link:
[Payload - Fake Update screen](https://github.com/hak5darren/USB-Rubber-Ducky/wiki/Payload---Fake-Update-screen)

_Script_

```bash
REM fake update LUL
REM author: Judge2020 https://judge2020.com
REM edited by: DanielL99 on github (thanks!)
REM
REM let the ducky HID enumerate
DELAY 3000
GUI r
DELAY 500
STRING iexplore -k http://fakeupdate.net/win10/index.html
ENTER
```

## Caveats

Please note that using a Rubber Ducky for dubious intents is illegal and a terrible idea, and I take no responsibility for the consequences if anyone chooses to use what they learn here to commit such acts.
