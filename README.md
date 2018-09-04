# IDD-Fa18-Lab1: Blink!

**A lab report by Natalie B. Abrams**

## Part A. Set Up a Breadboard


![a relative link](./breadboard_setup.JPG)


## Part B. Manually Blink a LED

**a. What color stripes are on a 100 Ohm resistor?**
 brown, black, black, red, red
**b. What do you have to do to light your LED?**
push the button and hold it! if you let go the LED turns off

## Part C. Blink a LED using Arduino

### 1. Blink the on-board LED

**a. What line(s) of code do you need to change to make the LED blink (like, at all)?**

digitalWrite()


**b. What line(s) of code do you need to change to change the rate of blinking?**

the delay() lines. the smaller the number the faster the blinking


**c. What circuit element would you want to add to protect the board and external LED?**

over voltage protector? short cuircut protector 
 
**d. At what delay can you no longer *perceive* the LED blinking? How can you prove to yourself that it is, in fact, still blinking?**

10/15. you can prove to yourself that it is still blinking because the light is on.


**e. Modify the code to make your LED blink your way. Save your new blink code to your lab 1 repository, with a link on the README.md.**

[My Blink](/my_blink.ino)

```arduino
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(20);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(100);                       // wait for a second
    digitalWrite(LED_BUILTIN, HIGH); 
  delay(40);                       
  digitalWrite(LED_BUILTIN, LOW);    
  delay(1000);                       
    digitalWrite(LED_BUILTIN, HIGH); 
  delay(30);                       
  digitalWrite(LED_BUILTIN, LOW);    
  delay(300);                   
    digitalWrite(LED_BUILTIN, HIGH);   
  delay(15);                       
  digitalWrite(LED_BUILTIN, LOW);    
  delay(15);                       
}
```



### 2. Blink your LED

**Make a video of your LED blinking, and add it to your lab submission.**

[Blink my LED](/blink_my_led.MOV)

[Blink your LED](/blink_your_led.MOV)

## Part D. Manually fade an LED

**a. Are you able to get the LED to glow the whole turning range of the potentiometer? Why or why not?**

yes I am able to get it to glow the whole turning range.

## Part E. Fade an LED using Arduino

**a. What do you have to modify to make the code control the circuit you've built on your breadboard?**

you need to set the variable 'led' to 11 so that it connects to my circut which is connected at pin 11.

**b. What is analogWrite()? How is that different than digitalWrite()?**

AnalogWrite() is a PWM (Pulse-Width Modulation), making it able to write an analog value through digital means. It is different than digitalWrite() because digitial write only writes a High or Low value and analog is able to create varying brightnesses (dimming).

[reference](https://www.arduino.cc/reference/en/language/functions/analog-io/analogwrite/)

[reference](https://www.arduino.cc/reference/en/language/functions/digital-io/digitalwrite/)

## Part F. FRANKENLIGHT!!!

### 1. Take apart your electronic device, and draw a schematic of what is inside. 
![a relative link](./mouse.JPG)
![a relative link](./front.JPG)
![a relative link](./back.JPG)

**a. Is there computation in your device? Where is it? What do you think is happening inside the "computer?"**

**b. Are there sensors on your device? How do they work? How is the sensed information conveyed to other portions of the device?**

**c. How is the device powered? Is there any transformation or regulation of the power? How is that done? What voltages are used throughout the system?**

**d. Is information stored in your device? Where? How?**

### 2. Using your schematic, figure out where a good point would be to hijack your device and implant an LED.

**Describe what you did here.**

### 3. Build your light!

**Make a video showing off your Frankenlight.**

![a relative link](https://youtu.be/EGgCspMCIh4)

**Include any schematics or photos in your lab write-up.**
