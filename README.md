# FPGA Basketball Game Controller - A Purude SoCET Intro I Project

A real-time basketball scoring and game timing system implemented on FPGA hardware with a custom PCB shield interface.

Contributors: 
* Tejas Wadhwa
* Jean-Milan Albarede
* Mehmet Mercan
* Hemant Garg
* Ian Kozloski  

## Demo

![System Overview](docs/system_photo.jpg)

[Demo Video](link_here)

## Features

- Real-time basketball game clock
- Shot clock timer
- Score tracking for both teams
- Quarter indicator LEDs
- Possession indicator LEDs
- Referee button controls
- Pause/resume functionality
- End-of-game buzzer
- Seven-segment display interface
- Custom FPGA shield PCB

## System Architecture

The system is implemented as a collection of Verilog modules handling:
- game state management
- timing generation
- display multiplexing
- user input debouncing
- scoring logic
- buzzer control

## Hardware

- FPGA Development Board: Digilent Arty A7-100T
- Custom PCB Shield
- Seven-segment displays
- Pushbuttons
- LEDs
- Piezo buzzer

## Custom PCB Shield

A custom PCB shield was designed to interface the FPGA board with:
- seven-segment displays
- LEDs
- pushbuttons
- buzzer circuitry

## RTL Design

### Clock Divider
Generates slower timing domains for game timing and display refresh.

### Score Controller
Handles increment/decrement logic for both teams.

### Game Timer
Implements countdown logic for the game clock and shot clock.

### Display Driver
Multiplexes seven-segment displays.

### Input Debouncer
Filters mechanical switch bounce from referee controls.

### Buzzer Controller
Activates end-of-game buzzer when timer reaches zero.

## Integration 

## Issues Faced

## Repository Structure

rtl/        -> Verilog source files  
sim/        -> Testbenches and simulation files  
docs/       -> Images, diagrams, PCB renders  
constraints/-> FPGA constraint files  
