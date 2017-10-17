# Hardware PWM
## Summary
1. Initialize inputs and outputs
2. Pull up resistor enabled
3. Enable Timer A in upmode
## Description
The timers that were initialized was TimerAx and TaxCCry.  The timers were set on a button interrupt which incremented the PWM by 10% each time.  The PWM was set to a frequency of 1 kHz.
## Board Differences
The 5529 did not have a hardware PWM option.  The 5529 did not have the hardware PWM option in that it was not able to connect to the TAoutmode to an LED register.  The programs were all pretty similar except the 2311.  The 2311 board had to have BX.y as its output.  The other programs had Ax.y as its output.
## Project Demonstration
In this demonstration the G2553 was used and the brightness increases by 10% each time the button is pressed.

![](https://media.giphy.com/media/3ov9k7EOnOUcq3ZQpq/giphy.gif)
