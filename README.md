# FPGA Piano Tiles Game

* Game was created in 24 hours at Elsys Easter Europe Hackathon in Belgrade 20-21. of May 2023.

## Overview
This project is a simplified version of the popular Piano Tiles game implemented on a Cyclone V FPGA using Quartus. Game is completely designed directly on hardware, without
using VHDL language. The game board consists of 8 columns, each controlled by keys A-K on the FPGA board. The objective is to press the corresponding key when a tile reaches the space between
two blue tiles at the bottom of the screen, mimicking the gameplay of the original game. 

## Team Members
- <a href=https://github.com/IgorAnton>Igor Antonijevic</a>
- <a href=https://github.com/PavleProd>Pavle Prodanovic</a>

## Functionalities
- VGA Controller: Generates video signals to display the game board on a VGA monitor.
- PS2 Controller: Interfaces with a PS2 keyboard to read the user's input from keys A-K. Contains Debouncer for backwards compatiblity with Cyclone III
- Switch 0: Toggles between two states - displaying the Belgian flag on the monitor and running the Piano Tiles game.
- Timer: Displays the elapsed time in MM:SS format on a seven-segment display.
- Sound Sensor: Produces sound output when any of the A-K keys are pressed. 
- LED output display the keys that are currently pressed(LEDR7-0 corresponding to A-K).

## Installation and Usage
1. Clone this repository to your local machine.
2. Open the Quartus project file (.qpf) in Quartus Prime.
3. Compile and build the project.
4. Configure the FPGA board with the generated programming file (.sof).
5. Connect the VGA monitor, PS2 keyboard, sound output, and Cyclone V/III board.
6. Power on the FPGA board and send code to the FPGA.

