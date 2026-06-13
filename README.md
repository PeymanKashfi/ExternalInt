# External Interrupt

## Overview

This project demonstrates the use of an external interrupt on the STM32 NUCLEO-L476RG development board.

The on-board user push button connected to PC13 is configured to generate a falling-edge interrupt. When the button is pressed, the interrupt service routine toggles the on-board LED connected to PA5.

The system clock is configured to run at 80 MHz.

## Hardware

- STM32 NUCLEO-L476RG Development Board
- On-board User Button (PC13)
- On-board Green LED (PA5)

## Interrupt Configuration

| Function | STM32 Pin |
|-----------|-----------|
| User Button | PC13 |
| Green LED | PA5 |

### EXTI Configuration

- Falling-edge trigger
- EXTI Line 13
- NVIC EXTI15_10 interrupt enabled
- Preemption priority: 0

## Features

- External interrupt handling using EXTI
- Falling-edge interrupt detection
- NVIC interrupt configuration
- LED control inside interrupt callback
- STM32 HAL-based implementation

## Project Structure

| Folder | Description |
|----------|-------------|
| Core | Application source and header files |
| Drivers | STM32 HAL and CMSIS drivers |
| Docs | Project documentation |

## Documentation

[Schematic PDF](ExternalInt/Docs/external_int_schematic.pdf)

## Development Environment

- STM32CubeIDE
- STM32CubeMX
- STM32 HAL Drivers