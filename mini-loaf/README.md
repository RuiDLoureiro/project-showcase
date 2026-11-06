# Loupher Labs — Mini_Loaf

**Stage:** Functional academic prototype with a proposed product enclosure  
**Technology:** Teensy · Arduino · MIDI / USB-MIDI · Bluetooth

Mini_Loaf is a compact digital synthesizer developed as my final undergraduate project. A dedicated Teensy sound engine generates audio, while a phone interface sends editing controls over Bluetooth. A MIDI keyboard supplies musical input.

## Contribution

I integrated the hardware modules, programmed the sound engine and connected the MIDI and Bluetooth interfaces. I explored the graphical editor in Unity, tested early Bluetooth interaction with MIT App Inventor and used Pure Data to exercise USB-MIDI. I also developed the enclosure concept and visual identity.

## Signal flow

The embedded engine combines oscillators, mixers, envelopes, filtering and effects, then sends the resulting signal through a digital-to-analogue output stage. Bluetooth carries parameter updates, keeping the phone interface separate from audio generation.

## What the prototype established

Functional testing demonstrated sound generation and communication. It also exposed filter noise and incorrect behaviour below 100 Hz, memory limits for delay, and insufficient USB power for some keyboards. Overall latency was not measured.

The black enclosure with wooden sides and the physical volume/preset control are proposed product designs. The academic build used a temporary wired assembly and adjusted volume through oscillator amplitude.

See [project milestones](MILESTONES.md).
