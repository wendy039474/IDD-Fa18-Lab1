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

(Sorry that I didn't have a 220 Ω resistor...)

## Part D. Manually fade an LED

**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**
Yes: based on the circuit we used, having the 220 Ω resistor ensures that the voltage across the LED won't exceed the limitation even if the potentiometer is set to be 0 Ω.

## Part E. Fade an LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**

Line 16, setting the LED pin from 9 to 11.

**b. What is analogWrite()? How is that different than digitalWrite()?**

analogWrite() gives the ability of serial changingof voltage, dividing 5V into 0~255, whereas digitalWrite() can only set a pin state to be HIGH(5V) or LOW(GND).


## Part F. FRANKENLIGHT!!!

### 1. Take apart your electronic device, and draw a schematic of what is inside. 

<img src="/System Diagram.jpeg">

<img src="/LED Wristband1.jpeg"><img src="/LED Wristband2.jpeg"><img src="/LED Wristband3.jpeg">

**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**

Yes, I believe the small black chip on the left of LED2 (in the images above) is the "computer". The "computer" is in charge of analyzing the signals it will get from IR receiver and transcript them into commands to control the blinking rates and colors of both of the LEDs.

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**

Yes, the IR receiver is a sensor that sensing IR signals from the environment. Once the IR receiver gets IR signals, it will send the signals to the "computer" chip on the board to be transcripted into commands. Those commands will be controlling the blinking rates and colors of both of the LEDs.

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**

The device is powered with two lithium cells providing input voltage at 6V which does not seem like having transformation or regulation of the power. The device comes with onboard resistor that makes sure the working voltage of both LEDs won't exceed the limitation.

**d. Is information stored in your device? Where? How?**
Yes: since the "computer" need to be able to transcipt IR signals into commands for LEDs, there needs to be pre-set code to store the information. The information might be stored on one of the black chips on the device but I'm not sure which one it is, it could be the processing chip comes with memory storage itself.

### 2. Using your schematic, figure out where a good point would be to hijack your device and implant an LED.

At first, I thought the easiest way to hijack the device and implant an LED would be doing a parallel connect with the LEDs that are already on the board; however, to do this, I might need to have a IR transmitter to send signals to this device which I don't have one. Here, I chose just to use the power from the battery on board to power my Metro mini and controll the LED cirucit I had for this lab.

### 3. Build your light!

[Rei_Frankenlight](//youtu.be/Gpvplpwjb9c)
