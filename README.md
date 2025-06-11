![Static Badge](https://img.shields.io/badge/CPU-MC6809-green "CPU:MC6809")
![Static Badge](https://img.shields.io/badge/CAD-KiCAD_8-green "CAD:KiCAD 8")

# Octuplex #

A 6502/6809 microcomputer in the shape of an octagon.

## Microprocessor ##

A choice of two classic 8-bit CPUs, the 6502 or the 6809.
The two chips have similar pinouts and are placed on the PCB overlapping.
Only one chip may be installed at a time.
Clock speed 2MHz in both cases,
with the 68B09 requiring a 4x clock input,
i.e. 8MHz.
The Hitachi 63B09 may also be fitted.

## Timer ##

The standard Motorola MC6840 timer chip.
Can generate interrupts and/or PWM signals.

## Parallel I/O ##

The standard 6522 parallel port chip.
Can generate interrupts.

Two handy little circuits for additional 8-bit I/O with minimal pin count: 74LS259 and 74LS251.
The 74LS259 is an unusual chip, an addressable latch.
It takes three address input pins and a single data input pin,
and has eight output pins.
The 74LS251 is an eight-input multiplexer with tri-state output.
The selector inputs are connected to three address pins,
while the output is connected to data bit D7.
The 6502's BIT instruction can read D7 directly into the sign flag,
which can be followed by BMI or BPL.

## Analog I/O ##

The classic Ferranti ZN428 8-bit DAC chip.

The classic Ferranti ZN448 b-bit ADC chip.
Although I'm not sure about this one due to its need for a negative supply rail.

## I2C Bus ##

Classic Philips PCF8584 I2C bus controller.
Can generate interrupts.

## Async Serial I/O ##

Rockwell R65C52 dual ACIA.
Can generate interrupts.

Motorola MC6850 with optocoupler for MIDI.
Can generate interrupts.

## Display ##

TBD, most likely an LED starburst display of some kind.

