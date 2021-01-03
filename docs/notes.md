---
title: Notes and Details
layout: docs
---

# Notes and Details

These are a few details that are important to note if you decide to keep playing with your blinkie. If all you do is explore a few patterns, and then stop fiddling with it, these notes won't really matter.

## About the LEDs

The blinkies are [WS2812Bs](https://cdn-shop.adafruit.com/datasheets/WS2812B.pdf). These are a particular RGB LED that are commonly used on LED strips around the world. There are probably hundreds of millions of these in the world right now.

The WS2812B has a small processor in it, and colors are communicated from one LED to the next via a digital protocol. Therefore, the six LEDs on the 18F board present as a *strip* of LEDs. When commands are generated on the QtPy, they are sent to L1, and then on to L2, and so on. 

## Feather vs QtPy

When programming the QtPy in MakeCode, we can't (yet?) select the QtPy as a target board. Therefore, we have to pick a board that has the same processor, and then fake a few things. 

When programming the QtPy, select the Adafruit Feather M0. This means you are picking an Adafruit product that has the same processor as the QtPy. Your QtPy has a SAM21D processor, which is otherwise part of the ARM Cortex M0 family. 

These are details. The important thing here is that you are picking 1) a different *board*, but it has 2) the *same processor*. That way, the code you write will run correctly on the QtPy.

## Pin A4

Take a look at the sample program that came with the 18F blinkie:

<div style="position:relative;height:calc(300px + 5em);width:100%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://maker.makecode.com/---codeembed#pub:_K0r5T1HavJf6" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

The strip is defined as being 6 LEDs long, and attached to pin A4. Why pin A4?

If you look at the schematic for the Adafruit Feather, you can see that pin A4 is "Port A, Pin 5." This is a designation at the *hardware level*. When I designed the 18F blinkie, I chose this pin to drive the LED strip. Therefore, to program it in MakeCode, we need to use the Feather designation for the pin, which is **A4**. 

This is all detail, but serves as a quick explanation for why that *must* be the pin that you chose for your LED strip. The LEDs are wired to that pin on the board, and that is in turn wired to the processor in a particular location, which (internally) is known as port A, pin 5.
