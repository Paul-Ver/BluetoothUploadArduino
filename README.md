# BluetoothUploadArduino
Project page on wirelessly (bluetooth) uploading&amp;communication with Arduino

# Why this GIT page?

Lately I've been scratching my hairs out over trying to get "Bluetooth uploading" to work.
This page combines the sources I found on the internet with the experiences I've had, to aid others who try to achieve the same.

I think bluetooth uploading to a regular Arduino is quite interesting, it's much like an FTDI cable, but the wirelessly.
Especially since the bluetooth versions of Arduino are not as common a homebrew alternative is very effective.

I'll be using this solution in my "LED Table", an LED matrix that can be controlled by a phone. Since there is need for a connection to a phone and the Arduino will be nicely tucked away, it's convenient to use bluetooth.
I'll also use this in a future project, where I make a bluetooth controllable car, which you can leave on the ground withouth having to plug in a cable for reprogramming (which is very convenient for testing purposes).

# Biggest issues:

The bootloader baudrates aren't very well documented on Arduino.
The Atmega168 based boards commonly use 19200 baud, while the Atmega328P based boards commonly use 57600 baud!

The bluetooth module has a fixed baudrate for the setup (through AT commands) and can be configured to use a different baudrate for communication.

Also, the bluetooth modules are 3.3V, so care should be taken when connecting these.

I also found that my bluetooth module can use it's "State" pin to trigger a reset (instead of having to solder a wire to the board itself).

Connecting the bluetooth device to a Windows PC can be quite bothersome.

# Tutorial:

Coming soon...

I'll re-evaluate my steps and share these.

## Configure the bluetooth module

## Make the hardware

## Upload code

## Connect to windows

## Upload a program!
