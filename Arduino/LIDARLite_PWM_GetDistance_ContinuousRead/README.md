# LIDARLite_PWM_GetDistance_ContinuousRead

Demonstrates taking a distance reading using Pulse-Width Modulation (PWM), does not require/use I2C

## Dependencies
1. Arduino Uno compatible Board
2. Arduino IDE (1.0.6 or newer)
3. USB Cable
4. LIDAR-Lite Sensor

## Installation
1. Download Repository and open with Arduino IDE

## Arduino Setup

Note: the current picture is wrong with regards to SDA, SCL pin
location on the Arduino boards.  This table is correct.

Arduino Board | SDA, SCL Pins
:--------------|:--------------
Uno, Pro Mini | A4 (SDA), A5 (SCL)
Mega2560      | 20 (SDA), 21 (SCL)
Leonardo      | 2 (SDA), 3 (SCL)
Due           |20 (SDA), 21 (SCL), SDA1, SCL1

![arduino-screenshot](http://pulsedlight3d.com/pl3d/wp-content/uploads/2014/11/arduino-pwm-setup2.png)

### LIDARLite I2C Connection Setup
LIDARLite Cable | Arduino Pins
:---|:---
5V | 5V
PWR EN | _(Unused)_
MODE | Connect to 1kΩ Resistor and Pin #3
SCL | _(Unused)_
SDA | _(Unused)_
GND | GND

*Connect the other side of the resistor to Pin #2.*

## Usage

1. [Connect an Arduino](#arduino-setup) and upload code
2. Open the serial monitor (Make sure baud rate is set to 9600)
3. The distance measured in centimeters (cm) will print to the serial monitor



