# Tinkercad_Projects

## Soil Moisture Monitoring System Using Arduino

#### Introduction
This project involves the development of a soil moisture monitoring system using an Arduino, a soil moisture sensor, and an LCD display. The system reads the moisture level from the sensor, calculates the moisture percentage, and displays it both on an LCD and via the serial monitor. This project is useful for applications in agriculture and gardening, where maintaining optimal soil moisture levels is crucial.

#### Components Used
1. Arduino Board: The main microcontroller used to interface with the sensor and the LCD.
2. Soil Moisture Sensor: A sensor used to measure the moisture level in the soil.
3. LCD Display: A 16x2 character LCD used to display the moisture percentage.
4. Connecting Wires: Used to connect the components.

#### Working Principle
1. Sensor Reading: The soil moisture sensor measures the moisture level in the soil and outputs an analog signal proportional to the moisture content.
2. Data Processing: The Arduino reads the analog signal and maps it to a percentage value representing the moisture level.
3. Display Output: The moisture percentage is displayed on both the LCD and the serial monitor.

### Explanation of the Code

1. Library Inclusion:
   - The code includes a library to control the LCD display easily. This library provides functions to manage the LCD using the I2C communication protocol.

2. LCD Initialization:
   - An object is created to represent the LCD display, specifying its I2C address. This object is used to interact with the LCD.

3. Pin and Variable Declarations:
   - The analog pin connected to the soil moisture sensor is defined.
   - Variables are declared to store the raw sensor reading and the calculated moisture percentage.

4. Setup Function:
   - Serial communication is initialized for debugging purposes, allowing data to be sent to the serial monitor.
   - The LCD is initialized with the specified number of columns and rows.
   - A static label "Moisture :" is printed on the LCD to indicate where the moisture percentage will be displayed.

5. Loop Function:
   - The soil moisture sensor's analog value is read continuously.
   - The raw sensor value is mapped to a percentage value representing the soil moisture level.
   - The moisture percentage is printed to the serial monitor for debugging.
   - The LCD cursor is set to a specific position where the moisture percentage will be displayed.
   - The moisture percentage and a percentage symbol are printed on the LCD.
   - Delays are added to control the update rate of the readings, allowing the system to update the displayed values without flickering.

#### Conclusion
This soil moisture monitoring system provides a simple and effective way to monitor soil moisture levels. It can be extended to include features like automated irrigation control, data logging, and remote monitoring. Such systems are beneficial in agriculture and gardening to maintain optimal soil conditions and improve crop yield.