# Software PWM
## Summary
1.Initialize inputs and outputs
2. Enable pull up resistor
3.Enable Timer A in up mode
4. Initialize TA0CCR0 and TA0CCR1
## Description
This program begins with intiailizing the device and setting up the inputs and outputs.  The board that was tested for this was the MSP430G2553.  The timer was intially set to run run at 250 Hz.  This was done by setting the internal divider to 8 and setting the timer to up mode.  The timer ran on SMCLK.  The two interrupts that were enabled was the CCR0 and CCR1.  The LED would turn on when CCR0 begain to interrupt and the LED turned off when CCR1 began to interrupt.  A if statement had to be created when both interrupts went off at the same time.  In that statement the CCR0 was set to have a zero state.

## Project Demonstration
Below the MSP430G2553 board is used to demonstrate the software PWM.

![](https://media.giphy.com/media/3o7aDa12x754vG7xmw/giphy.gif)
