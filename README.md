# smart-vehicle-can
Smart Vehicle Communication System using CAN protocol (Arduino + MCP2515)

This project demonstrates a **Smart Vehicle Communication System** using the **Controller Area Network (CAN)** protocol. It simulates real-world automotive subsystems communicating through a CAN bus network using Arduino and ESP32 microcontrollers.

  Project Highlights
- Implements CAN-based communication between multiple Electronic Control Units (ECUs)
- Uses MCP2515 CAN modules for reliable SPI-based CAN bus communication
- Integrates various sensors: DHT11, Gas sensor, Ultrasonic, LDR, and Water Level Sensor
- Displays sensor data on a 16x2 LCD via the master ESP32 node
- Controls actuators like motors, LEDs, buzzers, and relays

  Components Used
 - Arduino Uno: Microcontroller for controlling the project.
 - MCP2515 CAN Bus Module: CAN transceiver to send and receive CAN messages.
 - DHT11 or DHT22 Sensor: Measures temperature and humidity.
 - I2C LCD Display: Displays the temperature and humidity readings.
 - Jumper Wires: For connections.
 - Breadboard: For connecting components.
 - Power Supply: Typically USB power for Arduino Uno.

 Wiring

 1. MCP2515 CAN Bus Module to Arduino Uno

 -VCC -> 5V (Arduino Uno)
 -GND -> GND (Arduino Uno)
 -CS -> Pin 10 (Arduino Uno)
 -SCK -> Pin 13 (Arduino Uno)
 -MOSI -> Pin 11 (Arduino Uno)
 -MISO -> Pin 12 (Arduino Uno)
 -INT -> Pin 2 (Arduino Uno)
 
 2. DHT11/DHT22 Sensor to Arduino Uno

 -VCC -> 5V (Arduino Uno)
 -GND -> GND (Arduino Uno)
 -Data -> Pin 8 (Arduino Uno)
 
 3. I2C LCD to Arduino Uno

 -VCC -> 5V (Arduino Uno)
 -GND -> GND (Arduino Uno)
 -SDA -> SDA (Arduino Uno)
 -SCL -> SCL (Arduino Uno)
 
 Libraries Used

 -mcp2515: For interfacing with the MCP2515 CAN Bus module.
 -DHT Sensor Library: For reading data from the DHT sensor.
 -LiquidCrystal_I2C: For controlling the I2C LCD display.



