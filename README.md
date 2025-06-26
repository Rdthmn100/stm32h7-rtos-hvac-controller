# STM32H7 RTOS HVAC Controller

An embedded HVAC control system using the STM32H743IXH6 and FreeRTOS. This project demonstrates real-time scheduling, temperature and pressure sensing, and GPIO control for simulated heating/cooling.

## Features
- Real-time multitasking with FreeRTOS
- ADC-based temperature monitoring
- I2C based pressure monitoring
- GPIO-driven actuator logic (cooling/heating)
- UART logging via DMA
- Modular, RTOS-ready architecture
- Watchdog and fault detection framework

## Hardware
- STM32H743IXH6
- Temperature sensors
- Pressure sensors
- USB/UART for debugging and user interface to display data

## Tasks
| Task            | Function                            |
|----------------|-------------------------------------|
| SensorTask      | Read and filter temperature/pressure data     |
| ControlTask     | Manage heating/cooling logic         |
| LoggerTask      | Output system state to UART          |
| FaultMonitor    | Detect and report WDT or sensor faults |

## 📈 Roadmap
- [ ] RTOS boilerplate with task creation
- [ ] Sensor input via ADC
- [ ] GPIO control logic for heating/cooling
- [ ] UART logger task
- [ ] Watchdog and fault state handling
- [ ] CLI for runtime setpoint configuration

## Future Enhancements
- PID loop for temperature control
- EEPROM config storage
- CLI via UART
- GUI over USB or RS485

## 🔌 Getting Started
- Open in STM32CubeIDE
- Configure ADC, I2C, UART3, GPIOs, and FreeRTOS middleware
- Flash to target board
- Monitor serial output

## 🧠 License
MIT — see [LICENSE](LICENSE) for details.
