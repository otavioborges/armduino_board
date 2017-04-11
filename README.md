# ARMduino

ARMduino is an open-source + open-hardware project. Created to be a stepping stone from Arduino development boards to ARM development.

The board feature the same pinout as an Arduino UNO&trade; and same voltage levels on target.

## Board Description

### Power source

The board feature automatic source selection using a LM385 and P-MOSFET (same arrangement as Arduino UNO&trade;). External power range goes from 6~30VDC. Max current supported 0.5A.

### Programmer/Debugger

A MKL26Z32VFM4, using an adapted [DAPLink](https://github.com/mbedmicro/DAPLink) source-code (available on https://bitbucket.org/otavioborges/daplink-if, is used as programmer/debugger through openOCD interface.

### Target

The NXP's MKE02Z64VLD4 replaces the usual ATMEGA8U2 from Arduino. Providing:
 * Enhanced operation frequency (up to 20MHz Bus and core);
 * More flexibility on pin muxing (available on [KE02 Sub-family Data Sheet](http://www.nxp.com/assets/documents/data/en/data-sheets/MKE02P64M20SF0.pdf);
 * SPI, I2C, UART, PWM and ADC peripheral access through break-out connections;
 * I/O signal and periodic interrupts;
 * Debugging capabilities, using MKL26, GDB, DAPLink and openOCD;
 * Up to two breakpoints;
 
### Pinout

The same pin voltage and placement used in Arduino UNO&trade; is available. Furthermore, as NXP MCU provide a range of pin-multiplexing pin-assignment can be altered to fit user's desire.
