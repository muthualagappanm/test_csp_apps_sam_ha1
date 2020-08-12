[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# TCC PWM generation

This example application shows how to use the TCC to generate a 2 or 3 phase PWM signals for motor control with dead time.

## Description

TCC module is configured to generate synchronous 2 or 3 phase PWM signals with dead time. The duty cycle of the PWM signals is updated in the period interrupt handler.

## Downloading and building the application

To download or clone this application from Github, go to the [top level of the repository](https://github.com/Microchip-MPLAB-Harmony/csp_apps_sam_ha1) and click

![clone](../../../docs/images/clone.png)

Path of the application within the repository is **apps/tcc/tcc_synchronous_pwm_channels/firmware** .

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| sam_ha1_xpro.X | MPLABX project for [SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO) |
|||

## Setting up the hardware

The following table shows the target hardware for the application projects.

| Project Name| Board|
|:---------|:---------:|
| sam_ha1_xpro.X | [SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO)
|||

### Setting up [SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO)

- Connect the Debug USB port on the board to the computer using a micro USB cable

### Note:
*ATSAMHA1G16A device in SAM HA1G16A Xplained Pro board is not recommended for new design, hence replace the device with ATSAMHA1G16AB device. Connect the supported external debugger to Cortex Debug Port*

## Running the Application

1. Build and Program the application using its IDE
2. Observe the high-side and low-side PWM waveforms on oscilloscope
3. Observe the dead time between the high side and the low side
4. Observe the pwm frequency to be 10 KHz

[SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO) pin details:

|Signal Name| Pad   | Pin |
|-----------|-------|-----|
| CH0-PWMH  | PA04  | Pin 16 of EXT1 connector |
| CH0-PWML  | PB10  | Pin 14 of EXT1 connector  |
| CH1-PWMH  | PA05  | Pin 18 of EXT1 connector |
| CH1-PWML  | PB11  | Pin 13 of EXT1 connector |
| CH2-PWMH  | PA10  | Pin 15 of EXT1 connector |
| CH2-PWML  | PA16  | Pin 10 of EXT1 connector |
||||

[SAM HA1G16A Xplained Pro Evaluation Kit](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO) waveforms:

  ![output](images/output_tcc_synchronous_pwm_channels.png)
