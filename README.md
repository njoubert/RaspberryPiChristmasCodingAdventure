# The Joubert Family's Christmas Coding Adventure!

The Joubert family gets Raspberry Pi computers for Christmas, and embarks on a *Coding Adventure!*

### What??? What the...?? What IS all this stuff?? Where's the Candy??

1. I just gave all you guys **real computers!**. It can do everything your laptop can do!
2. You can actually build stuff with it! 
	- Simple stuff, like hook up speakers to it and use it as a music player... or
	- Build your own Hardware! You can connect buttons, lights, a small screen, etc!

**Yup, we're going to spend Christmas building something!**

### OK I guess that's cool... What can I build?

We can built *lots* of stuff. But that's not a useful answer. The RaspberryPi is *primarily an educational tool*, but it's beefy enough to do tons of real-world stuff. So, here's the *capabilities* of this little kit:

The **RaspberryPi** is a quad-core 1Ghz computer, with 1Gb RAM and a 16GB SD card for storage. It has a **fast graphics card** on it (for its size) that can decode 1080p movies to your big screen (1920x1080 maximum resolution). So, you can definitely play movies, netflix, youtube, all that kinds of stuff on here. 

It also has **100Mbps ethernet and four USB2.0 ports**. So you can plug in (multiple!) external hard drives, and you can use it as a file server. It can share four hard-drives on your network. It's also powerful enough to run a webserver! You can host your own website on it. Or use it to torrent things! You can even leave it plugged into the university's network at school, and use it as a file server. Log into it remotely, and download things over the fast school internet. Host a minecraft server! Host an IRC chat server! Host a Tor node for anonymous browsing! Naturally, you can plug in many USB devices! Plug in a webcam and use it as a remote monitor!

You can **power it from batteries** (I can help you set this up), and it's reasonable to imagine getting 5 to 10 hours of battery life from it.

It runs **linux or android** so you can learn how to work with a linux system. It's a really great **machine for programming**: Use it to learn how to program all kinds of stuff in Python: For example, use PyGame to write your own game!

....

Most importantly, it's **highly extensible!**

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

### Cool communities / places to look

A big part of building stuff is having inspiration and a community to draw from. Here's some great places that's fun to look at people's projects online:

- [Raspberry Pi Blog](https://www.raspberrypi.org/blog/)
- [Hackaday, both the blog and the whole site](https://hackaday.com/blog/)
- [Dangerous Prototypes](http://dangerousprototypes.com/)

### CURRICULUM / RESOURCES:

The main programming languages I suggest is **Python** and **C**. Use Python for all the experiments and hacking, use C for things that needs to be fast or needs to run *without an operating system: bare meta right on the hardware!*

- Pat's CS107e [Raspberry Pi Course Guides](https://github.com/cs107e/courseware/blob/master/guides/README.md)
	- For hardware, [understand basic electricity](https://github.com/cs107e/courseware/blob/master/guides/electricity.md)
	- Learn the (UNIX command line)[https://github.com/cs107e/courseware/blob/master/guides/unix.md]
- Learn basic Python!
	- [Instant Hacking with Python! Short, covers all the main stuff!](http://hetland.org/writing/instant-hacking.html)		- [Automate the boring stuff with Python! Lots of great useful things to build](https://automatetheboringstuff.com/)
	- [A Gentle Introduction to Python Coding on the Raspberry Pi](http://davidbriddock.blogspot.com/p/learn-python.html)
	- [Basic hardware programming with Python](http://makezine.com/projects/tutorial-raspberry-pi-gpio-pins-and-python/)

	

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
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/11_res.jpg)       | 1k and 10k Resistors!       | You need these to hook up LEDs and Buttons! |
|![rpi](https://raw.githubusercontent.com/njoubert/JoubertFamilyChristmasCodingAdventure/master/images/12_trans.jpg)     | 2N3904 Transistors!         | General purpose digital switch and amplifier! Use it to switch on and off larger stuff from the Pi. You can build a touch switch with it! |



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


### Useful Additional Add-ons:

There's a bunch of additional stuff you can buy to do even more cool things.

[FarmBot](https://hackaday.io/post/7593) is a great overall example! It pairs a Raspberry Pi and an Arduino, with a stepper motor driver ([line this one](https://www.adafruit.com/products/1438)) and a bunch of railings, to build a big robot that plants and waters your garden!

