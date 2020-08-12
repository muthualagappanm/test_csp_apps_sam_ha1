[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# DSU compute CRC32

This example application demonstrates how to use the DSU Peripheral library to compute 32-bit Cyclic Redundancy Checksum (CRC).

## Description

The DSU unit provides support for calculating a 32-bit CRC value for a memory area. This example application computes the 32-bit hardware CRC value using the DSU Peripheral and validates it using a software-calculated CRC value.

## Downloading and building the application

To download or clone this application from Github, go to the [top level of the repository](https://github.com/Microchip-MPLAB-Harmony/csp_apps_sam_ha1) and click

![clone](../../../docs/images/clone.png)

Path of the application within the repository is **apps/dsu/dsu_crc32_generate/firmware** .

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| sam_ha1_xpro.X | MPLABX project for [SAM HA1G16A Xplained Pro](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO) |
|||

## Setting up the hardware

The following table shows the target hardware for the application projects.

| Project Name| Board|
|:---------|:---------:|
| sam_ha1_xpro.X | [SAM HA1G16A Xplained Pro](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO)
|||

### Setting up [SAM HA1G16A Xplained Pro](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO)

- Connect the Debug USB port on the board to the computer using a micro USB cable

### Note:
*ATSAMHA1G16A device in SAM HA1G16A Xplained Pro board is not recommended for new design, hence replace the device with ATSAMHA1G16AB device. Connect the supported external debugger to Cortex Debug Port*

## Running the Application

1. Build and Program the application using its IDE
2. The LED indicates the success or failure:
    - LED is turned ON when the hardware CRC value matched with the software calculated CRC value
    - LED is turned OFF when the hardware CRC value did not match with the software calculated CRC value

The following table provides the LED name

| Board      | LED Name |
| ---------- | ---------|
| [SAM HA1G16A Xplained Pro](https://www.microchip.com/DevelopmentTools/ProductDetails/PartNO/ATSAMHA1G16A-XPRO) | LED0 |
|||
