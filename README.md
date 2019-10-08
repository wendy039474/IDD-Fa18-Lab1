# IDD-Fa19-Lab1: Blink!

## Part A. Set Up a Breadboard
<img src="/image1.jpeg">


## Part B. Manually Blink a LED

**a. What color stripes are on a 100 Ohm resistor?**

Brown-Black-Brown

**b. What do you have to do to light your LED?**

After building up the circuit, we will need to press the button to form a close circuit to light up the LED.

## Part C. Blink a LED using Arduino

### 1. Blink the on-board LED

**a. What line(s) of code do you need to change to make the LED blink (like, at all)?**

Modifying the code of line 33-36, within the loop function, will change the blinking of the LED.

**b. What line(s) of code do you need to change to change the rate of blinking?**

Line 34 and 35, two lines of delay function, control the rate of LED for staying on and off and can be changed to change the rate of blinking.

**c. What circuit element would you want to add to protect the board and external LED?**
 
Adding a resistor in the circuit to protect both the board and the external LED as limiting the voltage across the LED to protect it from burning.
 
**d. At what delay can you no longer *perceive* the LED blinking? How can you prove to yourself that it is, in fact, still blinking?**

With the delay parameter at 15 I could hardly tell the blinking.

I would probably add a print statement after each state changing of the LED to see whether the statement is being printed out. If yes, that mean the code did run through successfully with each lines.

**e. Modify the code to make your LED blink your way. Save your new blink code to your lab 1 repository, with a link on the README.md.**

[Rei_Blink](//github.com/wendy039474/IDD-Fa18-Lab1/blob/master/Rei_Blink.ino)

### 2. Blink your LED

**Make a video of your LED blinking, and add it to your lab submission.**

[Rei_Blink_Video](//youtu.be/7gvGH8JeNBg)

(Sorry that I didn't have a 220 Ohm resistor...)

## Part D. Manually fade an LED

**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**
hi

## Part E. Fade an LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**

**b. What is analogWrite()? How is that different than digitalWrite()?**


## Part F. FRANKENLIGHT!!!

### 1. Take apart your electronic device, and draw a schematic of what is inside. 

**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**

**d. Is information stored in your device? Where? How?**

### 2. Using your schematic, figure out where a good point would be to hijack your device and implant an LED.

**Describe what you did here.**

### 3. Build your light!

**Make a video showing off your Frankenlight.**

**Include any schematics or photos in your lab write-up.**
