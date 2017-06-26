# Step 3: Fade with a Potentiometer

Another step towards our bigger goal. We'll add a potentiometer - another input component - where we can dial up and down. We'll use this to select cities in our final implementation, but in this step you'll add it to the circuit and get more familiar with how it works. 

## Potentiometer

![Rotary Potentiometer](potentiometer.jpg)

A potentiometer is essentially a dimmer switch. As you dial it down, it becomes more resistive, allowing less electricity to flow. When you dial it up, it becomes less resistive. Inside the potentiometer, there’s a slider. This is what we connect to our circuit and read from. The slider moves along a circular track, and the track acts as a resistor. Turning the knob, moves the slider around the track. As it moves along, this track it increases or decreases the resistance and we can use this to determine the relative position of the slider.

In our code we use `analogRead( pin )` to read from an analog component (one that gives us a ranged value). This method returns a value from `0` to `4095`. 

__Using your potentiometer__

There's one in your kits. It has three pins. The outer two pins can be connected in either direction and to either Ground or Power. The middle terminal is connected to the slider (or the bit that moves) allowing us to read it’s 'position'.

When wiring a potentiometer, wire either left or the right terminal to ground; the remaining outer terminal to power (Vin or 3v3) and the middle terminal to an analog pin you want to read from.

Next we're going to wire up a potentiometer and allow you to fade up and down an LED as you turn the dial.

## Circuit

Make some changes to the circuit and add in the potentiometer: 

- Wire one side to ground (GND)
- Wire the other to Power (3V3)
- Wire the middle to A0

![Potentiometer circuit](LedSwitchPot_bb.png)

## Code

Use the LED code from Step 1 as a starting point for this sketch. The [completed code](code-by-end/LED.ino) is available in the folder above.



### Compiling and sending to the Particle device

1. Make sure you save your sketch. 

1. Make sure the Status Bar (bottom of Particle Dev) has a device connected and the photon’s indicator is breathing blue. If not make sure your Photon is connected by USB and is getting a WiFi signal.

2. Press the Lightning bolt on the top left of the window.

3. You’ll see a message ‘Compiling in the Cloud’ and a few sections later your Photon should start flashing magenta.

4. Wait a few moments, it should return to breathing blue, and the LED should begin to flash!

## Turn the Dial

Try it out by turning the potentiometer on your circuit!

## Things to Try 

Combine a switch and potentiometer. The switch should turn on and off the light while the potentiometer will fade up and down the light (but only when its on).

