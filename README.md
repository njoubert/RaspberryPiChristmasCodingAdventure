# The Joubert Family's Christmas Coding Adventure!

The Joubert family all gets Raspberry Pi computers for Christmas, and embarks on a *Coding Adventure!*

### What??? What the...?? What IS all this stuff?? Where's the Candy??

1. I just gave all you guys **real computers!**. It can do everything your laptop can do!
2. You can actually build stuff with it! 
	- Simple stuff, like hook up speakers to it and use it as a music player... or
	- Build your own Hardware! You can connect buttons, lights, a small screen, etc!



### What the hell Niels, what kind of Christmas gift is this? Now what?

It was Pierre-Henri's idea! Anyway, the point is:


Here's some ideas!


## OK I guess that's cool... What can I build?

### Cool communities / places to look

A big part of building stuff is having inspiration and a community to draw from. Here's some great places that's fun to look at people's projects online:

- [Hackaday, both the blog and the whole site](https://hackaday.com/blog/)
- [Dangerous Prototypes](http://dangerousprototypes.com/)


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



### Useful Additional Add-ons:

There's a bunch of additional stuff you can buy to do even more cool things.

[FarmBot](https://hackaday.io/post/7593) is a great overall example! It pairs a Raspberry Pi and an Arduino, with a stepper motor driver ([line this one](https://www.adafruit.com/products/1438)) and a bunch of railings, to build a big robot that plants and waters your garden!

