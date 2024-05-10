# Firefly
Firefly is a set of audio plugins (VST3 and AU) developed in RNBO, that attempt to emulate some of the artifacts introduced by old tape machines. A demo of the current state of the project can be found here:

https://youtu.be/ZsKpP1Vimgs

# How it works
There are three basic pitch modulation methods implemented:
- Rust: randomly changes the pitch slightly with a given frequency.
- Dying firefly: random dropouts (like tapestop moments)
- LFOFirefly: what you would expect from an LFO modulating the speed of the signal

# What has been developed until now
There are two plugins currently developed:
- FireflySampler: a sampler with Rust and Dying Firefly capabilities. NOTE: remember to load a sample or the plugin won't work. I have added some samples in the demo samples folder.
- FireflyVibrato: an effect that allows the user to add Rust and LFOFirefly to an incoming signal, with different settings for each channel.

# How to install it
Go to the build folder, and copy the plugins to your local plugin folder (In current MacOSX version /Library/Audio/Plugins/VST3 for vst and  /Library/Audio/Plugins/Components for AU).

# How to see the code and build it
Open the Max patchers and check out the code! You might need to add the subpatchers folder to the Max paths by opening max and hitting Options -> File Preferences...
You may also need a RNBO licence.

With the max patch open, double click on the rnbo objetc, export to Audio Plugin and copy the plugin to your plugins folder.

# Future planned work
Currently working on a UI around the whole theme of the fireflies modulating sound. I am perdsonally a big believer of alternative interfaces. There are also some other problems to solve, like the fact that the parameter values don't get saved with the projects.

# About the author
Juan Riera Gomez a.k.a. LUMINECHO is a sound technologist.