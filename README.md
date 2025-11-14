# H22R2x-Hardware

Hexabitz LTE/GNSS Module Hardware Design.



Design this module using the STM32G0B1CEU6 MCU and NRF9160-SICA-R7. Include connectors 734120110 and SIM8050-6-0-14-01-A.



This design must use two hexagons with a 4-layer PCB stack-up.

## Design Notes

1. Could not find the correct NRF9160-SICA-R7 component with the schematic file and pcb footprint inside of Altium Designer, so I referenced imported this one: https://www.digikey.com/en/models/10242085?tab=ultralibrarian
2. Referenced page 395 of the [nRF9160 datasheet](https://octopart.com/datasheet/nrf9160-sica-r7-nordic+semiconductor-102775108) for the schematic layout.
3. I could not find the capacitor in Altium Designer for capacitor C2, so I used this one: https://www.digikey.com/en/products/detail/samsung-electro-mechanics/CL10A475KQ8NNNC/3886703
4. I could not find the resistor that the datasheet referenced, so I used this one: https://www.digikey.com/en/products/detail/vishay-dale/CRCW020110K0FNED/1178493
5. Since P0.00 - P0.31 are multiplexed for the NRF9160-SICA-R7 I can choose any GPIO pin to act as UART0_TX and UART0_RX. I chose P0.28 to be UART0_TX and P0.29 to be UART0_RX.
6. Refer to this site for more data on the NRF9160-SICA-R7: https://docs.nordicsemi.com/
7. 

