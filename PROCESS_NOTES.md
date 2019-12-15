# Process notes for tinkering on circuit playground

## Guide

Following along with [this tutorial](https://learn.adafruit.com/welcome-to-circuitpython?view=all#).

## Getting Started

- Plug Circuit Playground Express into computer (make sure it's a *DATA* USB cable)
- `CIRCUITPY` will appear as a drive on the desktop.

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