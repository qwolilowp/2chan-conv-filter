# Two channel convolution filter

This is a little Pure Data (PD) patch, that does the following:

1. Read in 2 channel of audio from microphone.

2. If the first channel shows a significant (amplitude limit set) noise/sound (like a clap) sample this audio (1 sec) to a table.

3. Do convolution in frequency space of the stored sample with the audio of the second channel and normalize it with a window.

4. Output the signal. Every Minute write a audio file of the signal (storing in the location where the main.pd is saved).

# Hardware

This was written for a setup made of a Raspberry Pi3 and a Pisound extension ( https://blokas.io/pisound/ ).

# Samples

...
