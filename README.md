# Flight Computer

This project is a flight computer powered by an ESP32-C3 microcontroller, designed to control two motors and two servos. It integrates multiple sensors and supports a range of functionalities that make it suitable for small UAVs and drones. The system is designed to operate on a 300mAh LiPo battery, with built-in charging through USB-C.

## Features

- **ESP32-C3** microcontroller for reliable performance and wireless connectivity.
- **Motor Control:**
  - Motor 1: GPIO4
  - Motor 2: GPIO5
- **Servo Control:**
  - Servo 1: GPIO1
  - Servo 2: GPIO6
- **Sensors:**
  - **MAX17048G** (Fuel Gauge) on Address: `0x36` (00110110b)
  - **BMP388** (Barometric Pressure) on Address: `0x76` (1001100b)
  - **QMC5883L** (Magnetometer) on Address: `0x0d` (0001101b)
  - **ICM-42670-P** (6-axis IMU) on Address: `0x68` (1101000b)
- **LEDs:**
  - Internal LED: GPIO7
  - External LED: GPIO0
- **Battery:**
  - Recommended battery: **300mAh LiPo** for optimal performance
  - **USB-C charging** support for ease of use

## Recommended Hardware

- **Battery:** 300mAh LiPo
- **USB-C charger** (included)

## Pinout

| Component      | GPIO Pin  | Description                      |
|----------------|-----------|----------------------------------|
| Motor 1        | GPIO4     | Motor driver pin                 |
| Motor 2        | GPIO5     | Motor driver pin                 |
| Servo 1        | GPIO1     | Servo control pin                |
| Servo 2        | GPIO6     | Servo control pin                |
| Internal LED   | GPIO7     | Status indicator                 |
| External LED   | GPIO0     | Additional LED indicator         |
| MAX17048G      | I2C (0x36)| Fuel gauge sensor                |
| BMP388         | I2C (0x76)| Barometric pressure sensor       |
| QMC5883L       | I2C (0x0d)| Magnetometer sensor              |
| ICM-42670-P    | I2C (0x68)| 6-axis IMU sensor                |

## Power Management

The flight computer operates on a **300mAh LiPo battery**, which provides sufficient power for typical operations. For convenience, the board features **USB-C charging**, allowing you to charge the battery easily.

## Getting Started

To get started with the flight computer:

1. Connect the appropriate motors, servos, and sensors as listed in the pinout table.
2. Power the device using a 300mAh LiPo battery.
3. Use the onboard USB-C port to charge the battery when needed.

## License

This project is open source and available under the [MIT License](LICENSE).
