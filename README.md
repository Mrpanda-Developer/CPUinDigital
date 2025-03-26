# Simple 16-bit CPU in Digital

![CPU Screenshot](screenshot.png)  
*(Screenshot placeholder - replace with actual image of your circuit)*

## Overview
This is a simple 16-bit CPU implementation built using [Digital](https://github.com/hneemann/Digital), a digital circuit simulator. The current version implements basic functionality to add two numbers and store the result in a register.

## Features
- 16-bit data bus
- 4 general-purpose registers (R0-R3)
- Basic arithmetic operations (currently only addition)
- Program counter for instruction sequencing
- 32-bit instruction format
![image](https://github.com/user-attachments/assets/ddd7e58b-b466-4df3-9b2c-2f462130f42c)

## Current Implementation
The CPU currently supports:
- Loading values from input into registers
- Adding two register values
- Storing results back to registers

## Instruction Set Example
The EEPROM contains sample instructions:
- `3004d1` - Load immediate value into register
- `1001f`  - Add operation
- `23001f` - Store operation
- `12001f` - Additional operations

## How to Use
1. Open the circuit in Digital
2. Set input values:
   - Port A: 16-bit input value
   - Port SD: 8-bit instruction data
3. Use the clock button to step through instructions
4. View results in the output registers R0-R3

## Inspiration
This project was inspired by [Ben Eater's 8-bit computer](https://eater.net/8bit) and various educational CPU design videos found online. The design incorporates concepts from these resources while adapting them to the Digital environment.

## Future Improvements
- Implement more ALU operations (subtraction, logical ops)
- Add memory access instructions
- Improve instruction decoding
- Add conditional branching

## Requirements
- [Digital Circuit Simulator](https://github.com/hneemann/Digital)
