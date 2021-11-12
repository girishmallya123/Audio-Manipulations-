# Audio-Manipulations-
This repository contains code to manipulate audio signals in Julia

These audio manipulations are done using the DSP (Digital Signal Processing) package in Julia.

The file "Julia Audio Signal Manipulations" contains the various audio filtering using convolution methods. It includes samples for, 
  - **creating a smoothing effect on the audio.**
    In smoothing, the data points of a signal are modified so that individual points that are higher than the immediately adjacent points (presumably because of noise) are reduced, and points that are lower than the adjacent points are increased. This naturally leads to a smoother signal (and a slower step response to signal changes). As long as the true underlying signal is actually smooth, then the true signal will not be much distorted by smoothing, but the high frequency noise will be reduced.
  - **creating an echo** - The Audio Echo Filter repeats a sound after a given Delay
  - creating an echo with reducing amplitude, and creating repeated echoes.


Convolution is a type of cross-synthesis, a process through which the sonic characteristics of one signal are used to alter the character of another. We are familiar with the concepts used for FM synthesis, in which an oscillator’s signal is used to modulate the signal of another oscillator. To an extent, this would be another form of cross-synthesis.

However, there are no oscillating waveforms involved in the convolution process. Instead, we work with two audio sources, an input signal and an impulse response. The input signal is the sound that will be affected, while the impulse response contains the sonic characteristics of the space or object that we will impart on the input signal.

References:
- https://terpconnect.umd.edu/~toh/spectrum/Smoothing.html
- https://www.izotope.com/en/learn/the-basics-of-convolution-in-audio-production.html
- https://docs.unity3d.com/Manual/class-AudioEchoFilter.html
