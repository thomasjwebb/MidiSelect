# Midi Select

Basic midi processing plugin I made to get around a limitation of [Bitwig's](http://bitwig.com) built in sampler, where it can't do round-robin selecting of samples to prevent machine gun sounding drums. It takes input midi and changes the pitch each time to a different pitch within the specified range. The use case I had in mind is to have one multisample for each drum pad and have this plugin between the pad and the multisample to select the range of pitches. Place round robin samples in adjacent pitches.

There is no gui. This is very no-frills. I made it for a specific purpose in a few hours for a song I'm working on. I don't even like working with samples (I'm all about analog/virtual analog and fm). But I put this up in case it helps anyone else out in the same situation. My hope is that Bitwig adds round-robin support, rendering this not necessary anymore unless you need a very weird chromatic note effect.

## TODO

1. Make a simple screencast tutorial on how to use this in case anyone's interested.
2. Support random or round-robbin down samples
3. Make builds (Mac OS X, Windows & Linux) available on github

## License

This uses juce which is under a dual license GPL/proprietary. I am not a lawyer, but the intention here is to be as permissive as possible. If you are using juce under the terms of the GPL, you may also use this code under those terms. If juce is ever given a more permissive license (BSD, MIT, lGPL or MPL), then you may use this under those terms as well. If you have a license to use juce in closed source products, you may also integrate this code as well under the terms of the BSD license LICENCE). Also if you re-write this to not need juce, again the BSD license applies.
