# STM32H7 RTOS HVAC Controller

An embedded HVAC control system using the STM32H743IXH6 and FreeRTOS. This project demonstrates real-time scheduling, temperature sensing, and GPIO control for simulated heating/cooling.

## Features
- Real-time multitasking with FreeRTOS
- ADC-based temperature monitoring
- GPIO-driven actuator logic (cooling/heating)
- UART logging via DMA
- Watchdog and fault detection framework

## Hardware
- STM32H743IXH6 (NUCLEO-H743ZI or custom board)
- Optional: Temp sensor (NTC, TMP36) on ADC
- USB/UART for debug

## Tasks
| Task            | Function                            |
|----------------|-------------------------------------|
| SensorTask      | Read and filter temperature data     |
| ControlTask     | Manage heating/cooling logic         |
| LoggerTask      | Output system state to UART          |
| FaultMonitor    | Detect and report WDT or sensor faults |

## Future Enhancements
- PID loop for temperature control
- EEPROM config storage
- CLI via UART
- GUI over USB or RS485

## Getting Started
- Open in STM32CubeIDE
- Connect board and flash
- Observe UART output via terminal
