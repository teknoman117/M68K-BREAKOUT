# M68K-BUS-VOLTAGE-CONVERTER

A breakout board for the MC68010 that drops the 5V TTL bus voltages to a 3.3V CMOS bus you can use with an FPGA.

Licensed under CC-BY-SA 4.0

## Pins

All MC68010 signals are brought out to header with the exception of the MC6800 peripheral interface pins. VMA and E are left floating, and VMA is tied to 5V through a 2K2 resistor. This does prevent the use of autovectored interrupts, bus considering it's attached to an FPGA, a proper interrupt controller is a simple thing to add.

### Assembled
![Assembled](/Assets/assembled.webp)

### PCB
![PCB](/Assets/pcb.webp)

### Schematic
![SCH](/Assets/M68K-BUS-VOLTAGE-CONVERTER-SCH.pdf)
