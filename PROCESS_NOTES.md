# Process notes for tinkering on circuit playground

## Guide

Following along with [this tutorial](https://learn.adafruit.com/welcome-to-circuitpython?view=all#).

## Setting up the serial monitoring

Details from [this guide](https://learn.adafruit.com/welcome-to-circuitpython/advanced-serial-console-on-mac-and-linux).

Need the port. First:

```
ls /dev/tty.*
```

Looking for the `usbmodem` entry

Then:

```
screen /dev/tty.board_name 115200
```

Where `board_name` is the name listed in the `usbmodem` entry. For example:

```
screen /dev/tty.usbmodem1421 115200
```

## Update the library bundle

https://circuitpython.org/libraries

## Returning to work

Even though I can save directly to the Circuit Playground board, I'm going to work in this repo instead and copy the code to Circuit Playground whenever I want to run it.

This just fits my normal operating style and also keeps a current copy on my computer (and my Github repo).

Command to run:

```
cp -rf ./board_files/lib/ /Volumes/CIRCUITPY/lib/
cp ./board_files/code.py /Volumes/CIRCUITPY/code.py
```

