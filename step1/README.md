
# Step 1: Making a Blinking LED

## Circuit

First things first, we'll make the circuit that our Photon will control!

- __Add an LED (long leg closest to the pin)__
- __Add a 1KOhm resistor to connect it to `D0`__
- __Complete the circuit to ground__

![Basic LED circuit](BasicLed_bb.jpg)

To make this circuit you need a Particle microcontroller, an LED, a 1KΩ resistor (brown, black, red)

Along your Particle device you will see a series of PINs or legs labeled `D0` to `D7`. These are the digitalPins which can be used for input or output. In this case we’ll be using them for output or to turn power on and off to make the LED blink.

First connect a 1K Ohm resistor (brown,black red)
- One end of the resistor goes to a breadboard terminal directly beside the pin marked D0 
- The other end can go to any other row on the breadboard. 

Next add an LED with the anode (longer leg) to the same row where the resistor connects. 
The pin at `D0` will provide power when it is turned on.

Next we need to connect the cathode to ground. Use your jumper wires to make a connection to the negative column of the power rail (marked in with the blue line)

Finally, near the `GND` pin use another jumper cable to connect it to the power rail as shown. Now we have a _complete circuit_ where power from Pin `D0` will always flow to ground.

## Getting Ready to Program

We have our circuit ready… now we can use Particle Dev to tell it what to do.

Open it up and open a new Window if needed. Then choose the `File` menu and `Save`. Create a new folder called `LedBlink` and save the sketch inside it as `LedBlink.ino`  __Notice the folder and the file name are the same__  We need to include a ‘.ino’ extension on our files so that the development environment recognises it as code for our microcontroller.

## Starting a Sketch

Our sketches for a Photon will always start the same way

````

// This is where we add variables or bits of 
// information we'll use in our program


// The setup is run once. It's called when the 
// microcontroller first launches 
void setup()
{
}

// This is called repeatedly, hence it's name - loop!
// the code here gets executed over and over again
// once it reaches the bottom it starts over

void loop()
{

}

````

Copy and paste this code into Particle Dev and we'll start to add some basic stuff to make interactive!

