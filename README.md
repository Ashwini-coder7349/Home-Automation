# Home-Automation

COMANY:CODTECH IT SOLUTIONS

NAME:ASHWINI NAIK

INTERN ID:CT12009

DOMAIN: EMBEDDED SYSTEM

DURATION:4 WEEKS

MENTOR:NEELA SANTHOSH KUMAR

**Components Required:

Arduino (e.g., Arduino Uno)
Bluetooth Module (HC-05 or HC-06)
Relay Module
Appliance (e.g., Light or Fan)
Jumper wires
Power Supply for Arduino and Appliance

**Circuit Diagram
Here’s the connection layout:
*Bluetooth Module (HC-05/HC-06):

VCC → 5V (Arduino)
GND → GND (Arduino)
TX → Pin 10 (Arduino RX)
RX → Pin 11 (Arduino TX)

*Relay Module:

VCC → 5V (Arduino)
GND → GND (Arduino)
IN1 → Pin 7 (Arduino digital pin)
NO (Normally Open) → One side of the appliance (Live wire)
COM (Common) → Other side of the appliance (Neutral wire)
Note: The appliance (light or fan) should be connected to the relay correctly, as you are switching high voltage using the relay.

**Working Demo:
*Wiring Setup:

Connect the HC-05 Bluetooth module to Arduino (TX to RX and RX to TX).
Connect the Relay Module to the digital pin 7 on Arduino and the appliance.
Make sure the appliance (light or fan) is properly connected to the relay to handle high voltage safely.

*Pair the Bluetooth Module:

Pair your smartphone with the HC-05 Bluetooth module using the default password 1234.
Open a Bluetooth terminal app on your smartphone (e.g., Bluetooth Terminal for Android).

*Send Commands:

In the Bluetooth terminal app, type 1 and send it to turn the appliance ON.
Type 0 and send it to turn the appliance OFF.


**Working Principle:
When you send the command 1 from your smartphone, the Bluetooth module communicates with the Arduino. The Arduino then sends a HIGH signal to the relay pin, activating the relay and turning the appliance ON.
When you send the command 0, the Arduino sends a LOW signal to the relay, turning the appliance OFF.
You can add additional commands to control multiple appliances or devices.

**OUTPUT:

![Image](https://github.com/user-attachments/assets/62c69189-a67c-4601-ad57-a853855cb440)
