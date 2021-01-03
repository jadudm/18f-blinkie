---
title: Welcome to the 18F Blinkie
layout: docs
---


# The 18F Blinkie 

<img src="{{ '/assets/images/large-18f-blinkie.gif' | prepend: site.baseurl }}"
      style="float: right; border: solid;" 
      alt="An animated GIF of the 18F blinkie." 
      width="200px">

Congratulations! If you're reading this, you must have an 18F blinkie! Your 18F blinkie is artistnal, Maine-made craft electronics **that you can program to blink**. 

To use your 18F blinkie:

1. Plug the small end of the USB-C cable into the blinkie.
2. Plug the big end of the USB-C cable into a power source.

Let there be blinkenlights!

## Changing the Blinkenlights

There are many ways to change what the blinkie does. My favorite is MakeCode. Here's the code that is currently on your blinkie:

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://maker.makecode.com/---codeembed#pub:_K0r5T1HavJf6" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

### An Easy Change

If you open that code in your browser (right-click on the code above and open in a new tab), you can actually edit the program for yourself! The code has two pieces: **on start** and **forever**. The first, **on start** runs just once when the blinkie is turned on, and **forever** then runs in a loop, over-and-over, until you turn the blinkie off.

If you click on the dropdown in the "show frame of animation" block, you can choose a new pattern. Try picking something else!

### Download

Now, click download. This will take a moment, and it will offer up a .UF2 file. While there is a great deal of awesome packed into that file, it is enough to say right now that this file contains the code that runs on the QtPy.

Find the file in your Downloads folder.

### Reset the Blinkie

On the QtPy, there's a tiny reset button. Press it once.

You have now moved your QtPy into "program mode." Two things will happen. First, a solid, green light should be showing on the QtPy. Second, a new drive should have appeared on your computer; it will be called **QTPY_BOOT**.

Open up your Finder and go to your Downloads folder. You should find the .uf2 file you just downloaded. Drag the .uf2 file onto the drive **QTPY_BOOT**.

### Sit Back and Watch Das Blinkenlights

Now that you dragged the code onto the blinkie, it will reboot, and run your code!

YOU HAVE JUST PROGRAMMED THE INTERNET OF THINGS!

`:bunny-star-power:`

### A Note About Reprogramming

To program new patterns, you will repeat the process described above: 

1. modify your code
2. download
3. reset, and
4. drag-and-drop

Your computer may complain that you've "unplugged without unmounting" the 18F blinkie. This will happen *every time* and it is *supremely annoying*. It is how the process works, however, and it *cannot hurt the blinkie or your computer*.

In short, it happens every time, it's OK, it is annoying, and there's nothing to be done about it. Meh.

## In Conclusion

There's a ton of documentation out there regarding programming blinkenlights with the QtPy and its larger siblings from Adafruit. MakeCode is widely used for novice programmer education, for both experimenting with hardware like the QtPy, as well as game development with novices. For example, if you wanted to explore old-skool game development, you might pick up a [Kittenbot Meowbit](https://www.kittenbot.cc/products/meowbit-codable-console-for-microsoft-makecode-arcade), which is essentially a slightly larger version of the QtPy, but with a screen and buttons.

Your QtPy is, truly, a fully programmable $6 computer, and you can do many, many things with it if you choose. You could say that the 18F logo is a "shield" or "backpack" for the QtPy, and does little more than provide a few blinkenlights against the backdrop of the 18F logo. You can program your cutiepie in C/C++, Python, and MakeCode, as well as many other languages. And, it opens the door to more explorations with other embedded devices and the "internet of things," if you ever so choose.

Enjoy, and may 2021 treat you near-infinitely better than 2020. 

*At least there will be blinkenlights...*

### A Resource or Two

* [NeoPixels with MakeCode](https://learn.adafruit.com/neopixels-with-makecode)
* [CircuitPython and NeoPixels Uberguide](https://learn.adafruit.com/adafruit-neopixel-uberguide/python-circuitpython)

Of course, you can always ask the hardware designer questions, too.

#### Revision History

* [jadudm] Small cleanups, simplification. 20210103
* [jadudm] First version. 20201223
