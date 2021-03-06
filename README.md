# Color-Catchers
UCR CS120B Project

## Video
[![IMAGE ALT TEXT HERE] (https://img.youtube.com/vi/I1TSJ78IGaY/0.jpg)]
(https://www.youtube.com/watch?v=I1TSJ78IGaY)

## Setup
- Color-Catchers uses an ATMega1284 microcontroller, three shift registers, a speaker, LCD display, and an 8x8 RGB LED matrix.
- A0 - A3 controls the green LEDs in the matrix using a shift register, A4 - A7 controls the blue LEDs in the matrix using a shift register
- B0 - B3 controls the selection of LED's in the matrix
- B6 controls the sound effects played in-game for denoting color changes, being damaged, victory, and defeat.
- D3 - D5 are button inputs (left, middle, right)
- D6, D7 and C0 - C7 are used for the LCD display

## How to Play
The player is in the bottom row of the LED matrix and must avoid the colored orbs they are not while collecting
whichever colored orbs they are. The player will change colors throughout the game at regular intervals. To win the player must score
at least 50 points. For every 50 points, the player gains a life, capping at five lives.

Bullet Hell mode can be turned on and off by pressing the right button in the start menu.
Alternating color generation can be turned on and off by pressing the left button in the start menu.
Start the game by pressing the middle button.

## Bugs
- LCD displays game end screen while matrix is still in start game state
- Game state sometimes gets stuck and requires a hard reset
- Constant switching from "bullet hell" to normal mode may result in infinite lives.


