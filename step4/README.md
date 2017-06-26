# Step 4: Adding Internet

It'd be really useful to know what value our potentiometer is giving, right? 

One of the best things about the Photon is that it's connected to the internet. And it let's you put this kind of information from your device online, really really quickly. It lets you see what's happening on your device, make readings and other values available in just a line of code! You can connect all sort of actions and fuctions of your device online too. 

We're going to look at how to make some of this information visible in this section! 

## Circuit

There's no changes to our circuit this time! 

## Code

Use the code from Step 3 as a starting point for this sketch. The [completed code](code-by-end/LED.ino) is available in the folder above.

### Making your variables visible

We're going to start by making our `ledBrightness` and `potReading` variables from the last example available to view online. 

It really is as simple as one line of code. 

In the setup just add this line

```Particle.variable("dial", &potReading, INT);```

to make the potentiometer reading visible online... and 

```  Particle.variable("brightness", &ledBrightness, INT);```

to make the LED brightness visible online too. 

Once you've made those changes, save and flash your code (hit the lighting!)

To view these variables in real time, you can do that from Particle Dev. Choose the `Particle` Menu (top right) and then select `Show Cloud Variables`. A new panel will open and after a few moments you should see something like this:

![Cloud Variables](variables-panel.jpg)

Try changing your potentiometer readings and refreshing the values. 

