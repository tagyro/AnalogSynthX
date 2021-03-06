# AudioKit Analog Synth X Example

[![Build Status](https://travis-ci.org/AudioKit/AnalogSynthX.svg)](https://travis-ci.org/AudioKit/AnalogSynthX)
[![License](https://img.shields.io/cocoapods/l/AudioKit.svg?style=flat)](https://github.com/AudioKit/AnalogSynthX/blob/master/LICENSE)
[![Twitter Follow](https://img.shields.io/twitter/follow/AudioKitMan.svg?style=social)](http://twitter.com/AudioKitMan)

This is a simple iPad synthesizer app example by **Matthew Fecher** and **Aure Prochazka** built with Swift and AudioKit. It includes examples of Audiobus, Inter-app audio, and more. Created in late 2015, this is the first open-source synthesizer ever written in Swift. This code was originally included in AudioKit, and now has been updated to its own repo.

The complete source code is MIT open source. Meaning, you can use it as a learning tool, or even create your own synth app from the code. There's no charge or fee to use the code. Use it as a starting point to create the synth of your dreams! If you use this code in an app to be released to the App Store, you must change the graphics. And, please thank AudioKit. 🙏

<img width="50%" align="right" src="http://audiokit.io/examples/AnalogSynthX/analgsynthx.jpg">

## Compiling from source:

This project makes use of CocoaPods, so make sure you have that installed and then run

```
cd Examples/iOS/AnalogSynthX; pod install;
```

## Synth Features   

* 5-Voice Virtual Analog Synthesizer
* Audiobus and Inter-app Audio (IAA)
* Dual VCO-style Oscillators
* MIDI in for notes
* Dedicated Sub Oscillator
* FM Oscillator w/ Mod (Nord Lead style)
* 4-Pole Vintage Low-Pass Filter (Moog style)
* Oscillator Morph Knob (Access Virus style)
* Beautiful Sean Costello Reverb
* Free-running LFO w/ 4 waveforms
* Multi-tap (ping-pong) delay
* ADSR Envelope
* Detune Oscillators by Semitone & Hz
* Hold & Mono modes for keyboard
* Noise generator
* 8-Bit Crusher

## Sound Tips for Analog Synth X:

* You can get a pure Sine wave by (1) turning the Osc Mix to the left (2) turning off VCO1 (3) Turning the FM up!
* Use the morph knob between square and pulse for basic PWM control.
* Not getting enough low-end for your liking? Turn down the Rez.
* Use 2 saws and detune VCO2 for a shimmery vintage Polysynth sound. Slowly open the filter to your taste.
* The reverse saw LFO (the last wave setting on the LFO) can simulate a basic voltage-controlled note repeat.
* Keep dry/wet knobs under 50% for a more powerful sound.
* Turn the ADSR Release down to zero and turn the echo on to hear how the echo taps fire.

## Get in the Code:

* The sub is set to a sine wave for a more powerful bass tone. You can change it to a square if you'd like the synth to have more of a vintage feel. You can also experiment between -12/-24 settings.
* Try changing the preset knob bounds (minimum/maximum) in the SynthViewController to extremes to play a synth with wild settings!
* Sub and FM are tracked to the keyboard. Try tracking them to VCO1 for a more accurate Analog synth effect. (i.e. If you detune VCO1, FM & Sub also detune).
