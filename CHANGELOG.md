# SVM40 Firmware Changelog

## v2.2 (2020-12-14)

- SGP40: Turn heater off when returning to idle mode
- Bugfix for corrupted CRC calculation on sensor I2C bus

## v2.1 (2020-12-11)

- Add error handling for SHT and SGP communication errors: Old sensor values
  are taken for further processing of the current cycle and the sensor is reset
  for the next read cycle (SHT40: Send soft reset, SGP40: Assert reset pin)

## v2.0 (2020-12-02)

- Update VOC algorithm to version 2.0.0
- Add SHDLC and I2C commands for tuning the VOC algorithm
- Add SHDLC and I2C commands for getting and setting the state of the VOC
  algorithm
- Setting the temperature offset parameter on the SHDLC interface is supported
  as float or int16 value
- Breaking change: Getting the temperature offset parameter on the SHDLC
  interface returns an int16 instead of a float value

## v1.1 (2020-08-19)

