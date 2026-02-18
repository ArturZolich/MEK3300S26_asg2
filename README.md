"# MEK3300S26_asg2" 

To program the device use, e.g. 
    nrfjprog -f nrf52 --program merged.hex --chiperase --reset

The I2C transactions between the BMI160 and NRF52DK completes within 3 seconds from the NRF652DK reset.
INT1 and INT2 signals may occur at any time, triggered by the events defined in the transactions mentioned above.
The connection lines between NRF52DK (USB powered) and BMI160 are: 
BMI160  - NRF52DK
VDD -    VIN
GND -    GND
P0.27   -   SCL
P0.26   -   SDA