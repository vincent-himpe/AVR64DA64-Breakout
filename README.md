# AVR64Dx64 Breakout

This is a breakout board for the Atmel (microchip) AVR64Dx64 processor. You can use either the DA or DB version as they are pin compatible. Only the peripheral mappings are a bit different.
The board was made out of necessity to have a simple development board for this processor and there are no real boards out there (yet).

## Features:

UPDI programmer and UART.
It has an on-board UPDI programmer with HV capability to reset a bricked processor. The programmer has an auto-switch between Programming and UART mode. It uses a standard UDB connector and a CH340 type USB<>UART converter. Switching between UART and UPDI is controlled by the D

## I/O 

- Every pin of the processor is brought out to at least 3 test pins. 2 to hook up your stuff and a "third + ground" to easily hook up a logic analyzer or oscilloscope probe.
- All I/O ports have the capability of switching-in a button (active low ) or LED (active high) using banks of dip-switches.
- The two I2C busses are brought out on dedicated connectors.
- Besides the I/O pin headers , one of the I/O ports is brought out to an extra header for a character LCD interface (HD44780 type in 4-bit mode) on a 2x8 boxheader. This mates directly with the pinout of the classic 2x40 LCD display modules.
- There is provision for a 16 bit I/O expander in the form of a PCA9555 or PCAL9555A , each pin with the same button/led setup as the processor I/O pins.

Additional placeholders are on board for:

- 24cXX type EEprom or FRAM,
- An I2C DAC
- I2C Potentiometer.
- Voltage reference Diode (LM4040 with a voltage of your choice. I use 2.048 volt)

## Layout

The Board is a 2 layer PCB that can easily be produced by the likes of JLCPCB or PCBway.  A full production pack (Gerber / NCdrill, BOM , Pick and place ) is available. The production pack includes all the base parts like programmer, LED, resistors, Buttons and switches. It does not include the thru-hole parts or the DAC/ EEprom / potmeter. They add to the cost and you may not need those.

## Assembly

The Bom and pick and place is included for assembly using LCSC parts at JLCPCB

## Source Files

All source files are available in Altium Format. That's what i know, have and use. Other CAD programs most likely can import those. So you can modify.

## License

The project is PUBLIC DOMAIN. Do as you please. No warranties, As-Is
Creative Commons Zero.

