# M68K-BUS-VOLTAGE-CONVERTER

A breakout board for the MC68010 that drops the 5V TTL bus voltages to a 3.3V CMOS bus you can use with an FPGA.

Licensed under CC-BY-SA 4.0

## Pins

All MC68010 signals are converted with the exception of the MC6800 peripheral interface pins. VMA and E are left floating, and VMA is tied to 5V through a 2K2 resistor, which does prevent the use of autovectored interrupts. However, considering it's attached to an FPGA, a proper interrupt controller is a simple thing to add.

The RESET and HALT pins are able to be driven by the M68K itself, or by the FPGA. There are "RESET_OUT" and "HALT_OUT" pins which output the converted state of the pins, and "RESET_IN" and "HALT_IN" which connect to an inverter with open-collector outputs, allowing the FPGA to drive them low.

### Assembled
![Assembled](/Assets/assembled.webp)

### PCB
![PCB](/Assets/pcb.webp)

### Schematic
![Schematic](/Assets/M68K-BUS-VOLTAGE-CONVERTER-SCH.pdf)	
