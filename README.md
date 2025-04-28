      ETTI LED board

ETTI stands for "Facultatea de Electronică Telecomunicații și Tehnologia Informației" and I wanted to make a small
interactive device with this abbreviation. This device can be used as a promotional device, and also for events.

The whole device is composed out of 2 distinct boards. One is holding the LEDs configuration that makes the letters for
the logo and one that holds the control and the power circuit. They are connected via custom male-female connectors
and wires.

On the logo board are placed a number of 30 red LEDs and every one has a current limiting resistor of 220 ohm, that
are connected on the control board. The circuit runs on 5V, but it is not recommended to be plugged in the USB
devices ports, due to the high current needed. The circuit must be connected only in power banks or phone chargers.

The logic circuit that is performing the animation, is composed out of a sequential state machine, on 4 bits, with D 
flipflops, a Jonson oscillator configuration. The light animation simulates a "rotation" of the letters. The logic CMOS circuit
cannot provide enough current to drive the big number of LEDs, so a BJT NPN transistor is used on each output pin, to
act as a power switch. The clock signal is given by a 555 IC configuration, with constant 50% duty cycle and adjustable
frequency.
