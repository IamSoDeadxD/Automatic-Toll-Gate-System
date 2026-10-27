# Automatic Toll Gate System

An Arduino-based automatic toll gate system built as a college project using RFID, IR sensors, and a servo motor.

## About the Project

The aim of this project is to build a simple toll gate prototype that can authenticate RFID cards and control a gate automatically. An Arduino Uno handles the main logic, while IR sensors detect vehicle movement.

The system also uses an LCD to display messages and LEDs and a buzzer to provide feedback during authentication.

## Features

- RFID card authentication using the MFRC522 module
- Vehicle detection using FC-51 IR sensors
- Automatic gate control using an SG90 servo motor
- LCD messages for system status
- LED and buzzer feedback for accepted and denied cards

## Components Used

- Arduino Uno R3
- MFRC522 RFID reader and RFID card
- FC-51 IR sensors
- SG90 servo motor
- 16x2 LCD with I2C module
- Buzzer
- Red and green LEDs
- Breadboard and jumper wires

## Software and Libraries

- Arduino IDE
- Arduino C/C++
- MFRC522
- LiquidCrystal_I2C
- SPI
- Wire

## How It Works

1. The system waits for an RFID card to be scanned.
2. The Arduino checks whether the card is authorized.
3. If the card is accepted, the system gives feedback and starts the gate-opening sequence.
4. IR sensors detect the vehicle as it passes through the gate.
5. The servo motor closes the gate according to the programmed sensor sequence.
6. The LCD, LEDs, and buzzer indicate the system status.

## How to Run

1. Download or clone this repository.
2. Open the Arduino sketch inside the `code` folder using the Arduino IDE.
3. Install the required libraries.
4. Connect the components according to the wiring diagram and pin assignments.
5. Select Arduino Uno and the correct port in the Arduino IDE.
6. Upload the code and test the system.

Check the pin assignments in the code before connecting the hardware.

## Project Structure

```text
automatic-toll-gate-system/
├── code/
│   └── automatic_toll_gate.ino
├── images/
│   └── prototype.jpg
├── docs/
│   └── wiring-diagram.png
├── LICENSE
└── README.md
```

The image and wiring diagram can be added as the project documentation is prepared.

## Future Improvements

Some ideas I would like to explore in future versions:

- Adding an ESP8266 for IoT connectivity
- Sending data to ThingSpeak for remote monitoring
- Storing toll activity in a database
- Building a dashboard to view system activity
- Improving vehicle detection and error handling

These are planned improvements and are not part of the current implementation unless stated otherwise.

## Project Details

**Author:** Dhruv Singh

**Course:** B.Tech in Industrial Internet of Things (IIoT)

**Institution:** GGSIPU, USAR

**Project Type:** College project

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
