# Embedded IoT Homework 2

## Task 1: PWM Control of Two LEDs

### Description
The ESP32 controls two LEDs using PWM. Both LEDs fade in opposite directions, using different PWM frequencies.

- LED 1: GPIO 18, frequency 1000 Hz
- LED 2: GPIO 19, frequency 5000 Hz
- PWM resolution: 8-bit
- Resistor: 220 ohms for each LED

## Task 2: OLED PWM Monitor

### Description
An SSD1306 OLED display is used to monitor both LEDs. It displays their duty-cycle percentages and PWM frequencies while the LEDs fade.

### OLED Connections
- VCC: 3V3
- GND: GND
- SDA: GPIO 21
- SCL: GPIO 22
- I2C address: `0x3C`

### Wokwi Simulation
[Open the working Wokwi simulation](https://wokwi.com/projects/478586998694108161)

### Screenshots
- `screenshots/wokwi_circuit.png` — Complete Wokwi circuit
- `screenshots/wokwi_running_pwm.png` — Task 1 simulation
- `screenshots/wokwi_running_oled.png` — Task 2 simulation with OLED
- `screenshots/hardware_circuit.jpeg` — Physical circuit
- `screenshots/hardware_running_pwm.jpeg` — Task 1 physical test
- `screenshots/hardware_running_oled.jpeg` — Task 2 physical test with OLED

### Testing
The simulation was tested to verify that both LEDs fade in opposite directions and the OLED displays the changing duty-cycle percentages and configured PWM frequencies.

The physical hardware was tested successfully, and photographs were taken as evidence.

## Comparison Between Wokwi and Physical Hardware

The PWM project worked similarly in Wokwi simulation and on the physical ESP32 hardware. In both, the two LEDs faded in opposite directions, and the OLED displayed their duty-cycle percentages and PWM frequencies. Wokwi made it easy to test the circuit virtually, while physical hardware testing verified its operation with actual components.