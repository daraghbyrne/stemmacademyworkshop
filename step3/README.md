# Step 2: Fade with a Potentiometer

Another step towards our bigger goal. We'll add a potentiometer 


## Pushbuttons

![How a button works](button.jpg)

It’s a pretty simple component. It has two terminals on either side. By pushing down on the button, it creates a connection between the terminals allowing electricity to flow. When you release the electricity can no longer flow.

In our code we use `digitalRead( pin )` to check the power flowing to a pin on our microcontroller. This method returns high or low

## Circuit

Make some changes to the circuit as follows:

![Pushbutton circuit](LedandSwitch_bb.png)