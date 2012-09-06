Super-Arduino-Bros
==================

Arduino sketch that plays the Super Mario Bros theme over and over and over...

This sketch is actually a polyphonic chiptune synthesizer that plays up to three voices simultaneously, reading the notes to play from 3 tracks. It also features a timer that can vary from 30 to 120 bpm. The tracks have a resolution of 1/16th. To play a note, the synth reads into an array a pitch index (index -1 is a pause), it uses the index to read the actual frequency of the note to play, then it calculates an offset for reading into the wavetable and outputs it onto pin 9. The synth can play notes from C1 to C8, it features 5 8-bit, 8-bits adressable wavetables: sine ,square, tri, sawtooth and exponential stair, and it sampling rate is 31.25 KHz at 8-bit. The note frequencies table, the wavetables, and the tracks are all stored in the flash memory. There is also a very barebone java program that takes the first 3 tracks of a midi files and formats it to be read by this synth.

Total size is 4020 bytes in flash memory WITHOUT any sequencer track.