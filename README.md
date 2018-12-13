# touchdesigner
Touchdesigner components

##DMXUnfucker
A component that @matthewwachter and i built a while back when we had to deal with a bunch of random fixtures. I've gone back and done some cleanup to make it more self explanatory / user friendly, so it's now DMXUnfucker-v2

*Please note that the channels are 1-indexed as this is how we usually discuss them -- dmx channel 1 is referenced by the component pars as channel 1, not channel 0, and corresponds to the output channel 'dmxchan1'.

###Functionality:
-send random values to all channels - useful if you just need to see 'is anything working'
-set a single channel to a specific value
-turn a single channel off
-set a range of channels to a specific value
-turn a range of channels off

Single channel and range of channel selections are applied at the time a pulse is sent for their respective commands, so you can freely control a universe of DMX this way by changing channel selections and then pulsing buttons. 

You can use DMXUnfucker as both a diagnostic / testing tool and a means to send specific dmx channel data as part of your project. We've found this handy especially handy when dealing with dmx fixtures that we can't necessarily change the addressing on. The output of the component is a full dmx universe worth of channels that can be easily selected and shuffled as needed.
