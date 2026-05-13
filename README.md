# Daisy Patch.init() MultiFx Demo

## Overview

This is a simple multi-fx, designed for end-of-chain transition fx (but also pretty fun as a general multi-fx).

The effects consist of:

- Tempo-Synced beat repeat
- Resonant high-pass
- Resonant low-pass
- Phaser
- Tempo-Synced ping-pong delay
- Reverb
- Limiter

The effects are all stereo, and are in a fixed chain (see attached quickstart sheet). The tempo-synced effects will default to 120 bpm, or will take the incoming tempo of a 16th note clock passed into B10.

The chain is pre-configured (although I would like to add a SD-card configuration system in the future).

## Using the Fx

To enable the effects, hold button B7, set switch B8 to the "up" position, or send a gate in to B9.

If the effects are not enabled, OUT_L and OUT_R will simply output the input found at IN_L and IN_R, with a simple limiter applied.

If the effects are enabled, the CV_ inputs control the _amount_ of various effects:

- CV_1 and CV_5 control the hi-pass and reverb
- CV_2 and CV_6 control the low-pass and delay
- CV_3 and CV_7 control the hi-pass and phaser
- CV_4 and CV_8 control the beat-repeat

The effects are simple macros, so the higher the value, the more the effects are applied.

## Patch ideas

- If you're making techno or similar dance music, running your entire mix through the fx module makes for some simple dj-style effects for transitions and breakdowns
- A lead or mid-to-high pitched voice can use the module as a simple stereo multi-fx - adding a bit of high-pass, phaser, and reverb can really add some punch to more legato voices, and more transient-heavy voices can benefit from the delay and low-pass
- Automate the on/off of the effects through a gate in to B9, and throw random modulation at the beat-repeat through CV_8 to get a stuttering effect that's great for sampled drums or mixed rythmic lines (e.g. hi-hat, snare, and shaker)

![Datasheet containing the same information as this markdown file, alongside a diagram showing the controls mapped to the Patch.init().](/assets/multifx-datasheet.png)

## License

This is a closed-source demo project, with an assumption that the software will be used only on Electrosmith Daisy Patch.init() modules, for the express purpose of testing and feedback.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to use the Software only for testing and performance purposes, including without limitation the rights to use, copy,  publish, and distribute copies of the Software. Permission is not granted to sublicense, and/or sell the software, or hardware units running the software. I'm not a lawyer - so let's just say please don't be a dick (including by trying to make money of this crappy software).

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
