
# MEK3300S26 assignment 2 

### Assignment hex file
See **merged.hex** in this repository  

### Programming


To program the device use, e.g.

**nrfjprog -f nrf52 --program merged.hex --chiperase --reset**

Expected command output is presented in **output.png** file in this repository.

### Notes

The I2C transactions between the BMI160 and NRF52DK completes within 3 seconds from the NRF52DK reset.

INT1 and INT2 signals may occur at any time, triggered by events defined in the I2C transactions mentioned above.

  

### Wiring

The connection lines between NRF52DK (USB powered) and BMI160 are:

 - BMI160 - NRF52DK
 - VDD - VIN
 - GND - GND
 - P0.27 - SCL
 - P0.26 - SDA
