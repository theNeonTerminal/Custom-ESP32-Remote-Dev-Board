# ESP32 Based RC dev board

A project I made to experiment more with custom ESP32 dev boards and PCBs 100% suited to specific project needs

---

## About this project

This project features 2 PCBs each running its own ESP32 chip. The first board is small in size and is the receiver board - this will go into the device you are trying to control wirelessly. It has an ESP32 Chip (with its PCB Antenna) 2 TB6612FNG Motor drivers, capable of driving upto 4 motors individually in both directions along with PWM speed control, extra headers to attack servos, extra GPIO in the form of header to connects LEDs and other peripherals as needed. The second board contains another ESP32 chip, an ADS1115 ADC connected to 2 joysticks and few push buttons for various other tasks.

From the firmware side, this runs an ESP NOW script allowing seamless and easy wireless control over both. They run a 2 way communication script

> [!NOTE]
> Both boards have a type C port for programming along, the receiver board has an extra 2 pin terminal block for external power to motors, along with a jumper that allows the ESP32 to be powered via external soruce or USB, useful for debugging.
