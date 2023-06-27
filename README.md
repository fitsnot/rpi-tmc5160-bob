# rpi-tmc5160-bob
Quick and dirty stepper motor controller based on Raspberry Pi Pico and Trinamic TMC5160-BOB [PCB] [ARDUINO]
The goal is to have either a potentiometer or magentic encoder as rotary input that controls the speed of a large stepper motor. SPI and the integrated motion controller of the Trinamic TMC5160 is used to reduce computational load on the MCU as low as possible.

## Code
The TMC5160_Arduino library by tommag https://github.com/tommag/TMC5160_Arduino is used.

TODO:
- [x] Initial test with RPI and TMC5160-BOB
- [ ] Integrate AS5600 as rotary encoder
- [ ] Tune for utilised MOSFETS


## PCB
FIrst draft uses Raspberry Pi Pico and either a TMC5160-BOB ("Breakout board") or a corresponding SilentStepstick. A AS5600 can be used as a rotary encoder via I2C protocol.

<img src="https://github.com/fitsnot/rpi-tmc5160-bob/blob/main/hw/rpi-pico_tmc5160_pcb/RPi-Pico_TMC5160.png?raw=true" alt="Rendering of the PCB" width="600" />

