## [Getting started with Raspberry Pi Pico C/C++](https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf)

## Ref:
- [robotdad/picontoes: Pi Pico projects in VS Code from WSL](https://github.com/robotdad/piconotes)
- Get the SDK
```
git clone -b master --recursive https://github.com/raspberrypi/pico-sdk.git
```
- Get the Samples
```
git clone -b master https://github.com/raspberrypi/pico-examples.git
```
- Install tools
```
sudo apt install cmake gcc-arm-none-eabi libnewlib-arm-none-eabi build-essential
```
## The problem you might get
- [SDK location was not specified.](https://forums.raspberrypi.com/viewtopic.php?t=332016)

## Install usbipd-win (PowerShell)
- [usbipd-win](https://github.com/dorssel/usbipd-win)
```
winget install usbipd
```

## Share a device, allowing it to be attaced to WSL2
- [WSL support](https://github.com/dorssel/usbipd-win/wiki/WSL-support)
```
usbipd --help
usbipd list
usbipd bind --busid=<BUSID>
```
