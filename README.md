# RaspberryPiPicoWM

### Reference Link
- [Raspberry Pi Documentation/ Microcontrollers / Raspberry Pi Pico](https://www.raspberrypi.com/documentation/microcontrollers/raspberry-pi-pico.html)

### [Raspberry Pi Pico W](https://www.raspberrypi.com/documentation/microcontrollers/raspberry-pi-pico.html#raspberry-pi-pico-w-and-pico-wh)
- Wireless(802.11n), single-band(2.4GHz) : infineno CYW43439
- WPA3
- Soft access point suporting up to four clients
- Bluetooth 5.2
  - Support for Bluetooth LE Central and Perpheral roles
  - Support for Bluetooth Classic
Onbard antenna licensed form ABRACON (formerly ProAnt)
Wireless interface is connected via SPI to the RP2040 microcontroller

- **Share Pin**
  - CLK : VSYS : only when there isn't an SPI transaction in progress can VSYS be read via the ADC
  - Infineon CYW43439 DIN/DOUT : IRQ : only when an SPI transaction isn't in progress is it suitable to check for IRQs.

**Adding grounded metal to the sides of the antenna can improve the antenna's bandwidth.**

**NOTE**
*CYW43439 -> SPI -> RP2040*
*CYW43439 supports both 802.11 wireless and Bluetooth over this interface.*

**IMPORTANT**
Default libcyw43: non-commercial use

### [Pinout](https://www.raspberrypi.com/documentation/microcontrollers/raspberry-pi-pico.html#pinout-and-design-files-2)
![image](https://github.com/ChungChiuHung/RaspberryPiPicoWM/assets/52248840/486cac1c-fb6f-4c7a-ae1b-ae290a20717b)

### Getting Started
- [C/C++](Notes_GettingStarted.md)
- [Prefer way: pico-setup-windows](https://github.com/raspberrypi/pico-setup-windows)
