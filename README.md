# Booth's Algorithm Visualizer

An interactive step-by-step visualizer for Booth's multiplication algorithm using signed two's-complement binary arithmetic.

## Overview

This project demonstrates how Booth's multiplication algorithm performs signed binary multiplication at the register level.

The visualizer displays:

- Multiplicand (M)
- Multiplier (Q)
- Accumulator (A)
- Q-1 flip-flop
- Q₀Q-1 decision pair
- Arithmetic right shifts
- Step-by-step execution
- Complete execution trace
- Final A || Q product
- Decimal result verification

## Booth's Algorithm Rules

| Q₀ Q-1 | Operation |
|--------|-----------|
| 00 | No operation |
| 01 | A = A + M |
| 10 | A = A - M |
| 11 | No operation |

After the required arithmetic operation, an arithmetic right shift is performed on the combined A, Q and Q-1 registers.

## Example

For:

M = 1234

Q = -5678

The visualizer automatically selects:

N = 14 bits

The final result is:

1234 × (-5678) = -7,006,652

## Features

- Signed two's-complement multiplication
- Automatic register-width detection
- Step-by-step execution
- Previous/Next iteration controls
- Auto Play
- Arithmetic right-shift visualization
- Q₀Q-1 decision tracking
- Complete execution trace
- Final product verification
- Responsive interface

## Technologies

- HTML5
- CSS3
- JavaScript
- BigInt-based exact arithmetic

## Screenshots

### Main Interface

![Main Interface](screenshots/main-interface.png)

### Execution Trace

![Execution Trace](screenshots/execution-trace.png)

### Final Result

![Final Result](screenshots/final-result.png)

## Demo

A complete demonstration video is included in:

`demo/booths-algorithm-demo.mp4`

## How to Run

1. Clone the repository.
2. Open `index.html` in a modern web browser.
3. Enter the multiplicand and multiplier.
4. Select the register width or use Auto-detect.
5. Click **Run Simulation**.
6. Use **Next Step** or **Auto Play** to visualize the algorithm.

## Project Purpose

This project was developed as an educational visualization tool to make Booth's multiplication algorithm easier to understand by showing the internal register-level operations involved in signed binary multiplication.
