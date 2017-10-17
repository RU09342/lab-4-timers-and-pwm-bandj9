# Software Debouncing
## Summary
1. Disable watchdog timer
2. Intialize pins
3. Enable timer
4. Enable appropriate interrupts
5. Rinse Repeat
## Description
The purpose of this lab is to eliminate the button bounce.  The bouncing of a button occurs because the contacts are made of springy metals.  When pressing the button it may look as if the button was pressed multiple times. 
## Board Differences
All of the boards had similar code to run the button blink program. There were three processors (5994, 2311, and 6989) that required one extra piece of code. For those boards the high-impedance mode pin is enabled by default. In order for the program to run this pin has to be disabled. The line that had to be added to these boards to disable this pin is as followed: PM5CTL0 &= ~LOCKLPM5
## Project Demonstration
This project is done on an MSP430G2553. When a button is pressed on the board the Red LED will turn on/off without and problems when holding down the button.

![](https://media.giphy.com/media/xT9IgIeCpTodPFeOKk/giphy.gif)
