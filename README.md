# Keil μVision_real-time-and-embedded-system
A code wirtten in C to control the functional lights and 3-axis accelaration sensor of the STM32f407 board

When the board is tilted from a flat horizontal orientation downwards in the direction of any of the four user LED’s (the centre of the pivot is the LIS3DSH) that LED should turn on – i.e the LED’s are used to indicate which edge of the board drops below the horizontal. If the board is tilted down in the direction of more than a single LED, then multiple LEDs should illuminate.


When the blue user button is “clicked”, the tilt switch from level 1 should pause and indicate that it is paused by blinking all four user LEDs on and off at 1 second intervals. The program should stay in this state until the blue button is clicked again, after which the tilt switch from level 1 will resume. This pausing state should be continuously available on further clicks of the button. A “click” means a press and release, so that the change in state occurs after the button is released.

Use the nested vector interrupt controller (NVIC) available on the processor to handle the communication with the LIS3DSH for the tilt switch developed in level 1 or 2. You have not used this functionality so far, but you have covered all of the techniques that you need to work out how to use it and to implement the required code.
