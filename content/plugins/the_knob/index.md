---
title: "The Knob"
description: "My first plugin"
---

## Description

[The Knob on GitHub](https://github.com/poofyOwl/plugins-theknob)

The Knob is an audio effect plugin I developed using the [JUCE](https://juce.com/) framework. 

It features 3 different modes, Violet, Teal, and Crimson, each offering a unique effect to your sounds.


{{< inline_image path=theknob_violet.png width=33.33 alt="Violet Mode" >}}
{{< inline_image path=theknob_teal.png width=33.33 alt="Teal Mode" >}}
{{< inline_image path=theknob_crimson.png width=33.33 alt="Crimson Mode" >}}

<br><br><br><br><br><br>

## Download

[Windows Installer](https://github.com/poofyOwl/plugins-theknob/raw/refs/tags/v1.1/installers/Windows/Output/TheKnobSetup.exe)

[MacOS Installer](https://github.com/poofyOwl/plugins-theknob/raw/refs/tags/v1.1/installers/MacOSX/build/TheKnob-setup.pkg)

## Modes

### Violet

**FX Chain: HPF -> Distortion -> Reverb -> Delay -> EQ**

- HPF: goes from 10 Hz to 150 Hz as the knob is turned up
- Distortion: uses the following transfer function: `tanh(sin(x))` 
- Reverb:
  - Small room, low spread
  - Less damping as the knob is turned up
  - Wet goes from 0% to 50% as the knob is turned up
- Delay:
  - Medium delay time with some feedback
  - Wet goes from 0% to 60% as the knob is turned up
- EQ:
  - Reduction at 400 Hz
  - Boost at 10 kHz

### Teal

**FX Chain: HPF -> Distortion -> Delay -> Reverb -> EQ**

- HPF: goes from 10 Hz to 150 Hz as the knob is turned up
- Distortion: uses the following transfer function: `tanh(x)` 
- Delay:
  - Short delay time with high feedback
  - Wet goes from 0% to 50% as the knob is turned up
- Reverb:
  - Medium room, medium spread 
  - Less damping as the knob is turned up
  - Wet goes from 0% to 80% as the knob is turned up
- EQ:
  - Boost at 1000 Hz
  - Boost at 10 kHz

### Crimson

**FX Chain: HPF -> Delay -> Reverb -> Distortion -> EQ**

- HPF: goes from 10 Hz to 150 Hz as the knob is turned up
- Delay:
    - Long delay time with some feedback
    - Wet goes from 0% to 100% as the knob is turned up
- Reverb:
    - Big room, high spread
    - More damping as the knob is turned up
    - Wet goes from 0% to 100% as the knob is turned up
- Distortion: uses the following transfer function: `tanh(x)` 
- EQ:
  - HPF that goes from from 10 Hz to 111 Hz as the knob is turned up
  - LPF that goes from from 20 kHz to 2500 Hz as the knob is turned up
  - Boost at 177 Hz
  - Boost at 1777 Hz
