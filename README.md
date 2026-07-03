Nosh Robotics Embedded Firmware Internship Assignment

Name: Shriniketana Kalale

Q1 - STM32 LED Blinking

Implemented on STM32CubeIDE for STM32 NUCLEO-G070RB.

Features:
External interrupt based switch handling
Timer interrupt based LED blinking
State machine implementation
Low power Sleep Mode using HAL_PWR_EnterSLEEPMode()

LED Behaviour:
Press 1 → 0.5 Hz
Press 2 → 1 Hz
Press 3 → 2 Hz
Press 4 → OFF
Repeat

Assumptions:
TIM3 is used for periodic interrupts.
PC13 is used as switch input.
PA5 (LED_GREEN) is used for LED output.


Q2 - Producer Consumer Sensor Simulation

Implemented using POSIX Threads.

Features:
Producer generates 0–5 random bytes every simulated second.
Consumer checks buffer every 10 simulated seconds.
Prints latest 50 bytes in hexadecimal.
Mutex ensures thread-safe access to shared buffer.

Assumptions:
1 simulated second = 200 ms.
Shared buffer size = 500 bytes.
