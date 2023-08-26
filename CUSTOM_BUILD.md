# Setup Mini Drone

## Drone Setup
- Drone: Brushless FPV Mini 130
- Board: Afroflight Naze32 Rev 6
- Reciever:
- Transmitter:
- ESC:
- CAM:
- CAM Transmitter:
- CAM Antenna:

## Betaflight:
- [Firmware Release v.3.2.5](https://github.com/betaflight/betaflight/releases/tag/v3.2.5)
- [Betaflight Configurator v10.7.0](https://github.com/betaflight/betaflight-configurator/releases/tag/10.7.0)


## Resources
- Betaflight on NAZE32
    - Betaflight is support until v3.2.5 for NAZE32
    - [Instructions](https://www.youtube.com/watch?v=XA5r_HbI__g) for Firmware Upgrade with newer Betaflight-Configurator Version
- [STM32CubeProgrammer](https://www.st.com/en/development-tools/stm32cubeprog.html) to alternatively flash firmware.
- [Issue](https://github.com/betaflight/betaflight/issues/2165) with disabled features on NAZE32 due to memory limitation.



## Custom Build
- ASSUPTION: Working on Windows 10 and Docker Desktop is installed.
1. Clone docker [betaflight build repo](https://github.com/betaflight/docker-betaflight-build)
2. Open terminal in cloned repo directoy
3. RUN `docker run -e "TARGET=NAZE" --rm -it -v C:/Users/patri/Documents/Development/GitHub/betaflight:/opt/betaflight betaflight/betaflight-build`
4. Flash Firmware