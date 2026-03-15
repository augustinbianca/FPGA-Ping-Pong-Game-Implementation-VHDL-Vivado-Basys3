This project implements a two-player LED Ping-Pong game on an FPGA, designed using VHDL and the Xilinx Vivado environment. The system runs on the Basys3 development board, using the onboard LEDs, push buttons, and 7-segment display to simulate a simplified digital ping-pong game.

The main idea of the game is to simulate a ball moving between two players using a sequence of LEDs. The LEDs represent the ball position and move from one side of the board to the other. Each player must press their corresponding button at the correct moment to return the ball.

Game Logic

The “ball” is represented by a single active LED that moves across the LED array. When the ball reaches the edge of the board:

Player 1 must press the left button (btnL)

Player 2 must press the right button (btnR)

If the player presses the button in time, the direction of the ball reverses and the game continues. If the player misses the timing, the opponent receives a point.

Features

LED animation simulating a moving ball

Two-player interaction using hardware buttons

Score tracking for both players

Score display using the 7-segment display on the Basys3 board

Timing control for LED movement and reaction windows

Visual feedback when a player misses the ball (e.g., LEDs turning on briefly)

Implementation

The system was implemented in VHDL and synthesized using Xilinx Vivado. The design includes several digital modules responsible for:

clock division for timing control

LED position control and direction logic

button input handling and game state management

score counting for both players

7-segment display control

Hardware Platform

FPGA board: Digilent Basys3

FPGA: Xilinx Artix-7

Development environment: Xilinx Vivado

Hardware resources used: LEDs, push buttons, and 7-segment display

Purpose of the Project

The project demonstrates the design and implementation of a digital interactive system on FPGA, combining state machines, timing logic, input handling, and hardware display control. It highlights practical concepts in digital system design using VHDL and FPGA development tools.
