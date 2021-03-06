# TimeStretch

SuperCollider version of Alex Ness's NessStretch

by Sam Pluta - sampluta.com

Implements a phase randomized FFT (SC) time stretch algorithm, the Ness Stretch, which splits the original sound file into 9 discrete frequency bands, and uses a decreasing frame size to correspond to increasing frequency. Starting with a largest frame of 65536, the algorithm will use the following frequency/frame size breakdown:

0-86hz : 65536,
86-172hz : 32768,
172-344 : 16384,
344-689 : 8192,
689-1378 : 4096,
1378-2756 : 2048,
2756 - 5512 : 1024,
5512-11025 : 512,
11025-22050 : 256

For the python implementation, go here:

https://github.com/spluta/TimeStretch

Special thanks to Jean-Philippe Drecourt for his implementation of Paulstretch, which was a huge influence on this code
