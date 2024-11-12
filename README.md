# LPE_Fall2024
Low Power Embedded Gaming Application using Blue Gecko
ECEN 5833 Low Power Embedded Design Techniques
Team Members: Jayash Raulkar, Unmesh Phaterpekar & Tirth Patel
Started: 07.09.2024

**Overview**: //
This project aims to design and develop a low-power gaming application using two Blue Gecko microcontrollers (MCUs) from Silicon Labs, leveraging Bluetooth Low Energy (BLE) communication. The project will involve creating a complete gaming system, where one microcontroller (Stick Gecko) acts as the BLE transmitter interfaced with various sensors and input devices, and the other microcontroller (Screen Gecko) acts as the BLE receiver, interfaced with a display to run the game application.

**System Description**
1. Stick Gecko (BLE Transmitter)
Microcontroller: ARM Cortex-M4 core
Components:
- Joystick: Interfaced using an ADC to capture user input for controlling the game.

- Buttons: Connected via GPIO for additional control functions.

- Gyro Sensor: Interfaced via I2C to detect motion, enhancing game interactivity.

- Temperature Sensor: Monitors device temperature, ensuring it operates within safe thermal limits.

- Power Supply: Battery powered with integrated energy harvesting, such as a solar panel, for extended operation.

- Communication: Sends sensor data and user inputs via BLE to the Screen Gecko.


2. Screen Gecko (BLE Receiver)
Microcontroller: ARM Cortex-M4 core
Components:

- LCD/OLED Display: Connected via SPI to display the game interface.

- Power Supply: Battery powered

- BLE Communication: Receives data from the Stick Gecko and processes it to update the game display.

