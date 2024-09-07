# Timers and Counters - MSP430 Microcontroller

## Presented by:
- **Bar Elias** - ID: 208545236
- **Haim Ozer** - ID: 316063569

**Course**: Microcontroller Lab  
**Group**: 3

## Overview

This presentation covers the functionality and applications of timers and counters within the MSP430 microcontroller family. It explores different timer types, configurations, and real-world usage in embedded systems.

## Topics Covered

### 1. What is a Timer?
- A timer is a binary counter driven by a clock of known frequency.
- Registers associated with timers control interrupts and enable counting.
- Elapsed time calculation formula:  
  `Δ𝑡 = (𝑇 * 𝑁)`  
  Where `T` is the clock period and `N` is the number of counts.

### 2. Uses of Timers in MSP430
- **Synchronization** of operations over periodic time intervals.
- **Periodic wake-up** from low-power modes.
- **Signal counting** with minimal current consumption in low-power modes (LPM).

### 3. Types of Timers in MSP430
- **Watchdog Timer**: Prevents hardware faults by resetting the system in case of failure.
- **Basic Timer**: Dual 16-bit counters for low-frequency operations such as Real-Time Clock (RTC).
- **Timer_A**: A 16-bit timer with multiple modes for generating PWM signals and counting.
- **Timer_B**: Similar to Timer_A but offers configurable bit-size for more advanced operations.

### 4. Watchdog Timer
- Automatically resets the system if it enters an infinite loop or experiences a bug.

### 5. Basic Timer
- Dual 16-bit counters for RTC operations and interrupt generation for low-frequency outputs.

### 6. Timer_A and Timer_B Modes
- **Stop Mode**: Pauses the timer.
- **Up Mode**: Counts up to a specific value.
- **Continuous Mode**: Continuously counts up to the maximum value.
- **Up-Down Mode**: Counts up to a specific value, then counts down.

### 7. Capture and Compare Modes
- **Capture Mode**: Measures time intervals during input events.
- **Compare Mode**: Generates interrupts or produces a PWM output.

## Key Highlights
- **Watchdog Timer** - ensures system reliability by resetting the microcontroller in case of system hangs.
- **Basic Timer** - is used in low-power systems and real-time clock (RTC) applications.
- **Timer_A and Timer_B** - provide advanced timing functionalities like Pulse Width Modulation (PWM), capture, and compare.

## Conclusion
Timers are crucial in embedded systems for managing time-sensitive tasks, improving power efficiency, and ensuring precise intervals.
This presentation discusses how MSP430 timers can be effectively utilized in various real-world applications.
