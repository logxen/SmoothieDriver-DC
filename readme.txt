OVERVIEW

SmoothieDriver is a series of motor controllers designed to interface with Smoothieboard and other RepRap style motion controllers, allowing an enable/direction/step interface like the Pololu A4988 breakout boards commonly used and optionally i2c block level control with closed-loop feedback for advanced systems.

SmoothieDriver-DC is a series of Full H-Bridge drivers with closed-loop encoder feedback for driving Brush DC Motors. The system allows Brushed DC Motors to be controlled much like a stepper motor.

The current prototype board (gamma) is a triple motor driver capable of up to 3.5A per motor.

For more information contact Logxen. He is easily found on irc.freenode.net in #smoothieware or by e-mail at reprap at logxen dot com.

MAJOR COMPONENTS

SmoothieDriver-DC Gamma uses an NXP LPC1114, which has an Arm Cortex-M0 core, as mcu. It drives up to three Allegro a4950 full h-bridge drivers with current control managed by an MCP4725 on each driver. An upgrade from the Beta version, Gamma includes an MCP1252 3.3V regulator on-board so that it can be safely driven from a 3.3V or a 5V motion controller.