---
title: "Data-O-Tone"
date: 2022-08-27T22:00:00+02:00
tags: ["pedal"]
draft: false
---

Tags: pedal

This electric keyboard was an impulse buy that I hoped could mark my humble beginning into circuit bending. It was just 75 kr. (~10 EUR), looks vintage and has just a few simple controls, perfect for doing a pitch bend or adding an adjustable amplifier.

It was nearly impossible for me to find any information on the keyboard. The brand seems to be "KE Tronic", but searching for this name reveals nothing. Searching for the model name, "Data-O-Tone" doesn't yield any results either, except the name "Model 810".

## Build

For my first circuit bending project, I had three things I wanted to try:

- Add a jack output.
- Add a pitch bend.
- Add an internal amplifier / diode clipping circuit to add some "grit" to the sound.

### Jack output

This was very straightforward - drill a hole in a place that looks suitable, screw the mono jack in, solder the positive terminal to the positive terminal of the speaker, solder the ground terminal to the ground terminal of the speaker. To be honest, I wasn't too sure if I was soldering things rights, I just tried and it worked.

Of course, doing this resulted in the sound going to the jack output _and_ speakers at the same time. An improved solution would have been to add a toggleswitch, but I didn't have any, so screw it.

### Diode clipper overdrive

This didn't really work out. I was inspired by [this video](https://www.youtube.com/watch?v=P56SDeXFsLM&t=70) of a circuit bent SA-2, where they acheive an awesome synth sound by adding a feedback loop.

I tried to achieve something similar by adding a diode clipping circuit. Following this schematic, I was hoping that achieving a gritty synth took nothing but a 10k pot and two LEDs:

![Diode clipping schematic](/public//images/posts/data-o-tone/diode-clipping.gif)

However, the circuit did nothing but lower the volume by reducing the voltage. My theory on electronics is not that strong, so I can't tell what the right way to making it work is, but I imagine that there needs to be an op-amp before the clipping to increase the signal voltage to the point where clipping can occur.

### Pitch bend

Dejected by the lack of progress with the overdrive, I never got around to making the pitch bend. Touching the keyboard circuit with my fingers revealed many connections which would bend the pitch down, although I imagine that there must have been a pitch resistor which I could have simply replaced with a potentiometer. Ah well, maybe I will get around to doing this on the next one.

## Sound

It's vintage so surely it has some 80s or 90s charm, right?

This thing made me remember that not everything old is a forgotten, underappreciated, soon-to-be-upcycled treasure. Sometimes, old junk is just junk.

First problem: the keyboard is monophonic, meaning you can play just one key at a time. Even worse, pressing a second key while playing the first sustains the first note instead of switching. Letting go of the first key but holding down the second still sustains the first note. Thus, to play this keyboard properly, you need to always let go of a key before pressing the next, which can be surprisingly hard.

Second problem: There is just one sound and it's not pleasant. The sound is very close to that of a basic waveform, somewhere between a sine and saw wave, and can only be adjusted in two ways: volume (1-4) and vibrato (on/off).

After adding the jack output, I tried running the sound through some of my guitar pedals, adding e.g. overdrive, chorus and reverb. No matter what I did, it seemed to just amplify the suckiness of the original tone.

## Fate

I was a bit on the fence about keeping this. Like I said in the beginning, I wanted to have a "humble beginnings" keyboard to mark the start of my adventures into circuit bending. On the other hand, working with this thing was frustrating. The keyboard can only play when the casing is closed, so I had to open and close it between every modification. Because of their age and poor quality, multiple internal wires broke while I was working with the keyboard. The control buttons are not held in place and would frequently fall out.

In the end, I decided that this keyboard was not worth the effort. If I am going to circuit bend something, I want it to be something that I will want to keep. So, I desoldered what I could and recycled the rest. So far, Data-o-Tone, I hope that someone else was able to make a nice project out of you.
