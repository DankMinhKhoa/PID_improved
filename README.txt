***************************************************************
* Arduino PID Library - Version 1.2.0
* by Khoa Dang <minhkhoadang@gmail.com> - Originally by Brett Beauregard <br3ttb@gmail.com> brettbeauregard.com
*
* This Library is licensed under a GPLv3 License
***************************************************************

Improvisation made:
- Change of input and calculation type to float to save memory and
performance
- Change of output type to integer, as most of low level control
applications tends to drive directly from the Arduino's PWM outputs
- Modifying the anti windup method to stop increasing the integral term
when the output is saturated

// todo: adding templates to generate PID objects to work with any data
type
// todo: adding the back-calculation integral anti windup method