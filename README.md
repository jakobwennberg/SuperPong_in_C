Two Player Pong is a modern implementation of the classic Pong arcade game running on an STM32F407 microcontroller. The game features two players controlling paddles 
on opposite sides of the screen, trying to hit a ball back and forth. The first player to reach 3 points wins.

Code Structure and Organization
The program follows a modular design pattern with clear separation of concerns:

Main Game Logic: main.c - Controls the game flow and rules

Display: Split between graphical display and text display:
display_driver.c - Low-level display hardware interface
graphics.c - Higher-level drawing functions
ascii.c - Character display interface
ascii_game.c - Game-specific text display functions

Input Handling: keyb.c - Reads and processes keypad input

Timing: delay.c - Provides precise timing functions

Hardware Definitions: memreg.h - Memory-mapped register definitions

Common Types: typedef.h - Basic type definitions

By Emil Tervo & Jakob Wennberg
