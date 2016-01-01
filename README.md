# A Raspberry Pi Christmas Coding Adventure!

Dieter, Pierre-Henri and Gleb gets Raspberry Pi computers for Christmas, and embarks on a *Coding Adventure!*

This document gives you everything you need to get hacking with the Raspberry Pi!


| Section | **Table of Contents** | 
|---------|-----------------------|
|1|[What is a Raspberry Pi?](https://github.com/njoubert/RaspberryPiChristmasCodingAdventure#what-is-the-raspberry-pi)|
|2|[Step-By-Step Getting Started and Warm-up 15-minute Projects!](https://github.com/njoubert/RaspberryPiChristmasCodingAdventure#how-do-we-get-started)|
|3|[What Can I Build?](https://github.com/njoubert/RaspberryPiChristmasCodingAdventure#ok-i-guess-thats-cool-what-can-i-build)|
|4|[Learning More: My Curriculum for Next Steps with Guides and Resources](https://github.com/njoubert/RaspberryPiChristmasCodingAdventure/blob/master/README.md#learning-more-next-steps-guides-and-resources)|
|5|[Inspiring Projects, Great Communities, and Awesome Additions to the Pi!](https://github.com/njoubert/RaspberryPiChristmasCodingAdventure/blob/master/README.md#inspiring-projects-great-communities-and-awesome-additions-to-the-pi)|
|6|[What's in the Kit?](https://github.com/njoubert/RaspberryPiChristmasCodingAdventure#whats-in-the-box)|
|7|[Useful Testing Tools and Debugging Procedures](https://github.com/njoubert/RaspberryPiChristmasCodingAdventure#useful-testing-tools)|

### What the hell Niels, what kind of Christmas gift is this? Now what?

1. I just gave all you guys **real computers!**. It can do everything your laptop can do!
2. You can actually build stuff with it! 
	- Simple stuff, like hook up speakers to it and use it as a music player... or
	- Build your own Hardware! You can connect buttons, lights, a small screen, etc!

### What is the Raspberry Pi?

It's basically the innards of an iPhone 5, with all the pins exposed! It's built and maintained by the [Raspberry Pi foundation](https://www.raspberrypi.org/) as an educational tool.

- It has a powerful graphics card, can play 1080p video and has HDMI out!
- It can run either Linux or Android, and is built for easy programming! We'll mess around with Linux and Python!
- You can easily build your own hardware and attach it! Like buttons, LEDs, the christmas lights, etc...
- It's the most popular educational computer on the market!

Specifically, I gave you guys the newest Raspberry Pi 2! [Here's the Specs](https://www.raspberrypi.org/products/raspberry-pi-2-model-b/)

### How do we get started?

Raspberry Pi has a [quickstart guide here.](https://www.raspberrypi.org/help/quick-start-guide/) 

**Step 1: Setup!** 

[Copy NOOBS onto the SD card I gave you using your computer. Then stick it into your Raspberry Pi.](https://www.raspberrypi.org/help/noobs-setup/)

**Step 2: Connect!** 

Plug your Raspberry Pi into a monitor, keyboard, mouse and power! Then follow the NOOBS installer to install Raspbian (a derivative of Debian Linux, just like Ubuntu)

**Step 3: Mini Project: LEDs and Buttons!** 

Let's do some [Physical Computing on the Raspberry Pi!](https://www.raspberrypi.org/documentation/usage/gpio-plus-and-raspi2/) Try to make a little circuit with an LED, and [use python to turn it on and off using the GPIO pins!](http://openmicros.org/index.php/articles/94-ciseco-product-documentation/raspberry-pi/217-getting-started-with-raspberry-pi-gpio-and-python)

Expand it to also read the value of buttons!

	*CAREFUL:* You CAN damage your raspberry pi by connecting the pins incorrectly!

	1. ALWAYS disconnect your circuit before plugging and unplugging components or changing things.
	2. DO NOT draw more than 3.3V or less than 0V from a pin. Don't wire power directly to ground!
	3. Do NOT draw more than 5mA from a pin! Use the included transistors to switch higher power things on and off.
	4. Use Pull-down and Pull-up resistors with buttons.

[What is a pull-up and pull-down resistor?](http://playground.arduino.cc/CommonTopics/PullUpDownResistor)

Check out Pat's course CS107E, it has a [guide to basic electronics with the Raspberry Pi.](https://github.com/cs107e/courseware/blob/master/guides/electricity.md)

**Step 4: Serial Bridge from Laptop to RPi!** 

Install the SILABS USB to UART CP21xx driver, and try to make Python on your Raspberry Pi talk to you computer over Serial!

1 	Install the [SILABS driver](https://www.silabs.com/products/interface/usbtouart/Pages/usb-to-uart-bridge.aspx)

2	Plug the USB to UART adapter into your computer

3	Install a serial console on your computer, like [CoolTerm](http://freeware.the-meiers.org/)

4	[Write a Raspberry Pi program to send and receive serial data](http://www.instructables.com/id/Read-and-write-from-serial-port-with-Raspberry-Pi/), and see if it shows up on your laptop.

**Step 5: Mini Project: Transistors and Lasers!** 

Switch the Laser on and off with the Raspberry Pi using transistors!

The laser wants a higher voltage and higher current supply than the Raspberry Pi can provide. This is where you can use the transistor: The transistor is just a switch. A switch you can control electronically. By switching low power on the "base" pin, you can control whether high power flows through the other pins.

Follow [This article on how to switch 9v using a NPN transistor](https://electronics.stackexchange.com/questions/95089/switching-9v-using-a-npn-transistor-and-an-arduino) and hook up a higher voltage to your laser!

**Step 6: Mini Project: Servos and why you also need an Arduino!** 

Drive a Servo with PWM!

[Make the servo turn left and right from Python!](http://razzpisampler.oreilly.com/ch05.html)

Python is not great for driving Servos (and Linux in general isn't!) since it doesn't guarantee the *timing* of when things will happen. The same little processor is also driving your screen, mouse, keyboard, the network, keeping time, etc etc.

You can do better than python by using this [ServoBlaster Kernel Module](https://github.com/richardghirst/PiBits/tree/master/ServoBlaster) or by connecting it to an Arduino or a [Motor Shield / HAT](https://www.adafruit.com/products/2348)

The BEST you can do is to use hardware PWM. RaspberryPi has *one* dedicated little chip just to make PWM signals. This tutorial explains how to [use WiringPi to access this port.](http://raspi.tv/2013/how-to-use-wiringpi2-for-python-with-pull-ups-or-pull-downs-and-pwm)

**Step 7: Start Designing Your Own Stuff, or Get Insired By Others!** 

Read the rest of this page, and check out the "Cool communities and places to look" or google for "Raspberry Pi projects"!

### OK I guess that's cool... What can I build?

We can built *lots* of stuff. But that's not a useful answer. The RaspberryPi is *primarily an educational tool*, but it's beefy enough to do tons of real-world stuff. So, here's the *capabilities* of this little kit:

The **RaspberryPi** is a quad-core 1Ghz computer, with 1Gb RAM and a 16GB SD card for storage. It has a **fast graphics card** on it (for its size) that can decode 1080p movies to your big screen (1920x1080 maximum resolution). So, you can definitely play movies, netflix, youtube, all that kinds of stuff on here. 

It also has **100Mbps ethernet and four USB2.0 ports**. So you can plug in (multiple!) external hard drives, and you can use it as a file server. It can share four hard-drives on your network. It's also powerful enough to run a webserver! You can host your own website on it. Or use it to torrent things! You can even leave it plugged into the university's network at school, and use it as a file server. Log into it remotely, and download things over the fast school internet. Host a minecraft server! Host an IRC chat server! Host a Tor node for anonymous browsing! Naturally, you can plug in many USB devices! Plug in a webcam and use it as a remote monitor!

You can **power it from batteries** (I can help you set this up), and it's reasonable to imagine getting 5 to 10 hours of battery life from it.

It runs **linux or android** so you can learn how to work with a linux system. It's a really great **machine for programming**: Use it to learn how to program all kinds of stuff in Python: For example, use PyGame to write your own game!

- You can buy any size (from tiny to huge) LCD touchscreen on eBay, and [build your own tablet!](https://learn.adafruit.com/7-portable-raspberry-pi-multitouch-tablet/overview)
- You can *build your own hardware* that connects to the GPIO pins on the side! 
	- Buttons, switches, LEDs, and LED matrices! 
	- Stepper motors, DC motors, servos! Things that turn!
	- Accelerometers, Magnetometers, Gyroscopes, Barometers, Thermometers! Tons of sensors that measure the real word!

You can make a weather station that displays the current temperature and the chance of rain. Or measure the current internet ping latency and light up a row of LEDs accordingly. You can have it check your email for you, and light up an LED for every unread message - and beep every time a new message arrives! 

There's a whole range of **RaspberryPi HATs** that sit on top of the Raspberry Pi to give you additional functionalty! My favorite is the [Sense HAT](https://www.raspberrypi.org/blog/the-sense-hat-headgear-for-the-terminally-curious/)! It's currently in *space* on the ISS, and it has a ton of sensors, a small joystick, and a badass 8x8 RGB LED display matrix, so you can make cool animations.

You can pair it with **LED controllers** (like the [PixelPusher](http://www.heroicrobotics.com/products/pixelpusher)) and make an LED wall, or a starry night sky on the ceiling of your room!

You can hook up a **motor controller** and build a 2D cutter that slices up paper into shapes! Or moves a pen around to draw things programmatically! You can even build a **[robot](https://www.raspberrypi.org/blog/tag/robots/)!** A super-fancy robot would be a **[rubix cube solver](https://www.raspberrypi.org/blog/cube-solver/)**!

Hook it up to a Passive Infrared Sensor, and it can sense when someone is moving in your room - regardless of whether the light is on! Build a security system!

Here's some more ideas:

*Multimedia-related:*

- Set it up as Airplay speakers! You can stream music to it from your phone!
- Use it as a media center! Hook it up to a screen and your external harddrive, and it can play movies!

*Software-related:*

- Use it to run a torrent client to save stuff to your external harddrive without needing your computer
- Make a digital picture frame! Have it cycle through instagram pictures.

*Hardware-related:*

- Easier:
	- Display temperature forecast for today on the 7-segment display
	- Make the buttons send emails, texts, or scroll through different things on the display
	- Measure latency to your favorite server, display it as an LED graph
	- Make a sweet animation of LEDs blinking
- Intensely awesome:
	- Pair it with an Arduino Mega and RAMPS shield, and build any 3-axis movable CNC machine!
	- Build a 3D Printer

### Learning More: Next Steps, Guides, and Resources 

**Where to go to learn more?**

The main programming languages I suggest is **Python** and **C**. Use Python for all the experiments and hacking, use C for things that needs to be fast or needs to run *without an operating system: bare meta right on the hardware!*

Here's the **curriculum** I suggest you work through:

- Pat's CS107e [Raspberry Pi Course Guides](https://github.com/cs107e/courseware/blob/master/guides/README.md)
	- For hardware, [understand basic electricity](https://github.com/cs107e/courseware/blob/master/guides/electricity.md)
	- For using a transistor as a switch, [follow this TL;DR](https://electronics.stackexchange.com/questions/95089/switching-9v-using-a-npn-transistor-and-an-arduino) then read [this tutorial](https://www.techhouse.org/~dmorris/projects/tutorials/transistor.switches.pdf)
	- Learn the (UNIX command line)[https://github.com/cs107e/courseware/blob/master/guides/unix.md]
- Learn basic Python!
	- [Instant Hacking with Python! Short, covers all the main stuff!](http://hetland.org/writing/instant-hacking.html)		- [Automate the boring stuff with Python! Lots of great useful things to build](https://automatetheboringstuff.com/)
	- [A Gentle Introduction to Python Coding on the Raspberry Pi](http://davidbriddock.blogspot.com/p/learn-python.html)
	- [Basic hardware programming with Python](http://makezine.com/projects/tutorial-raspberry-pi-gpio-pins-and-python/)

**More Advanced Topics:**

- [Write your own hardware driver for a GPIO pin](http://sysprogs.com/VisualKernel/tutorials/raspberry/leddriver/)

### Inspiring Projects, Great Communities, and Awesome Additions to the Pi!

**Great Communities:** A big part of building stuff is having inspiration and a community to draw from. Here's some great places that's fun to look at people's projects online:

- [Raspberry Pi Blog](https://www.raspberrypi.org/blog/)
- [Adafruit Learn](https://learn.adafruit.com/)
- [Pimoroni Learn](http://learn.pimoroni.com/)
- [Wolfgang Klerk's Arduino and Raspberry Pi Projects](https://wolfgangklenk.wordpress.com/)
- [Hackaday, both the blog and the whole site](https://hackaday.com/blog/)
- [Dangerous Prototypes](http://dangerousprototypes.com/)

**Sources of Hardware and Software:** Where can you browse around and buy all the cool hardware parts for your awesome project?

- [SparkFun Store](https://www.sparkfun.com/)
- [AdaFruit Store](https://www.adafruit.com/categories)
- [Seeed Studio](http://www.seeedstudio.com/depot/)
- [ElectroDragon Prototyping Parts](http://www.electrodragon.com/)
- [NavSpark GPS Modules](http://www.navspark.com.tw/)

- [Adafruit Python GPIO Library](https://github.com/adafruit/Adafruit_Python_GPIO)
 

**Badass Projects Built on Raspberry Pi:**

- [FarmBot](https://hackaday.io/post/7593). Plants and waters a garden. Pairs a Raspberry Pi, Arduino, [stepper motor drivers](https://www.adafruit.com/products/1438)
- [Pi Tablet](https://learn.adafruit.com/7-portable-raspberry-pi-multitouch-tablet/overview). A 7" multitouch home-made tablet!
- [Pi-Top Laptop](http://www.pi-top.com/). A hackable laptop - slide open the top to reveal a raspberry pi and breadboard space.

**Cool hardware additions to the Raspberry Pi:**

- [AdaFruit Trinket](http://learn.pimoroni.com/tutorial/raspberry-pi/raspberry-pi-programming-adafruit-trinket). Like a tiny arduino: good for PWM generation, analog sensor reading, and real-time programming.
- [SenseHAT](https://www.adafruit.com/products/2738). So cool - RGB LED matrix and a boatload of sensors!
- OLED Displays like [this](http://www.amazon.com/gp/product/B00O2LLT30?keywords=raspberry%20pi%20oled&qid=1451470478&ref_=sr_1_1&sr=8-1) and [this](http://www.amazon.com/gp/product/B00ZOXWA7Y?psc=1&redirect=true&ref_=oh_aui_detailpage_o03_s00). Small, cheap, low-power, programmable displays.
- [Rechargeable LiPo power source.](https://www.adafruit.com/products/2465)
- [LED Matrix Displays](https://www.adafruit.com/products/2345)
- High Fidelity Audio Out such as the [pHAT DAC](https://shop.pimoroni.com/products/phat-dac) for phat beats.

### What's in the Box?
	
Each of you have slight variations on this, but here's the list of everything! 

|Img| What is it?                 | What's it for?? |
|---|-----------------------------|-----------------|
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/01_rpi.jpg)       | 1x Raspberry Pi 2 (Model B) | A single-board 1Ghz quad-core computer with 1GB Ram! |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/02_case_power.jpg)| Case and Power Supply       | Put the Pi in it, and power it up! |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/03_sd.jpg)        | 16GB MicroSD Card           | This is the "hard drive" for your Pi! We'll put Linux on this. |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/04_uart.jpg)      | SILabs USB to UART Bridge   | We can use this to connect to the Pi from our normal computer, when we don't have a screen or a ethernet cable for the Pi. |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/05_cobbler.jpg)   | T-Cobbler                   | A simple way to connect the Pi to a breadboard to hook up electronics! |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/06_bboard.jpg)    | Breadboard                  | Build electronic circuits simply by pushing components into this! |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/07_cables.jpg)    | Assorted Jumper Cables      | Hook things up together! |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/08_buttons.jpg)   | Buttons!                    | Program these to do something on click! |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/09_led.jpg)       | R,G,B,W LEDs!               | Light them up from your code! |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/10_segment.jpg)   | 7-segment display!          | Display numbers from your code! Temperature? Latency? Unread emails? Anything! |
|   | Micro Servo!          | [Make the servo turn left and right from Python!](http://razzpisampler.oreilly.com/ch05.html) Although an arduino is really better for this, since it can run in real time rather than sitting on top of linux. |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/11_res.jpg)       | 1k and 10k Resistors!       | You need these to hook up LEDs and Buttons! |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/12_trans.jpg)     | 2N3904 Transistors!         | These are NPN Transistors! General purpose digital switch and amplifier! Use it to switch on and off larger stuff from the Pi. You can build a touch switch with it! |



### Useful testing tools...

When you build stuff, you *really* need tools to test what you're doing. This avoids getting really frustrated when things don't work and you don't know why. Here's the testing tools I recommend:

**Hardware:**

- A multimeter! Like our Fluke! With it, you can check that something is turned on, that there's not too much or too little power before you plug something in, and what values your resistors are. This lets you measure voltage, resistance, and continuity.
- A Serial to USB connection! I included one! This lets you plug your computer directly into anything that has a serial connection, so you can check the data going in and out of it. For example, you can check whether a GPS is actually spitting out positions before wiring it up to your raspberry pi.
- A logic analyzer! This connects to a wire, and reads every bit going on that wire. So you can use it to "snoop" on the digital data sent between chips. 
- An oscilloscope for analog circuits: This can display the analog wave going along a cable. For example, this can show you the sound waves going to your speaker! So you can check whether they're distorted or clipped.


**Software:**

- First of all, use the Scientific Method to debug your code: Come up with a hypothesis for what might be wrong. Formulate an experiment to test your hypothesis. Then run your experiment and see if it proves or disproves your hypothesis. For example: Problem: "the LED doesn't turn on". Hypothesis: "there is no power coming out of the raspberry pi on that pin". Test: "Put a multimeter between the pin and ground. It should read 0v". Take the measurement, if it is 0v, now you know the problem must be with turning the pin on! If it is 3.3V, then the problem must be something with the LED.
- Put "print" statements in your code and check that each part is working as expected.
- Write your code in small chunks, and test every chunk.
- Learn how to use a debugger to step through your code.

