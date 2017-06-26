
# Step 1: Making a Blinking LED

## Circuit

First things first, we'll make the circuit that our Photon will control!

![Basic LED circuit][BasicLed_bb.jpg]

To make this circuit you need a Particle microcontroller, an LED, a 1KΩ resistor (brown, black, red)

Along your Particle device you will see a series of PINs or legs labeled `D0` to `D7`. These are the digitalPins which can be used for input or output. In this case we’ll be using them for output or to turn power on and off to make the LED blink.

First connect a 1K Ohm resistor (brown,black red)
- One end of the resistor goes to a breadboard terminal directly beside the pin marked D0 
- The other end can go to any other row on the breadboard. 

Next add an LED with the anode (longer leg) to the same row where the resistor connects. 
The pin at `D0` will provide power when it is turned on.

Next we need to connect the cathode to ground. Use your jumper wires to make a connection to the negative column of the power rail (marked in with the blue line)

Finally, near the `GND` pin use another jumper cable to connect it to the power rail as shown. Now we have a _complete circuit_ where power from Pin `D0` will always flow to ground.
