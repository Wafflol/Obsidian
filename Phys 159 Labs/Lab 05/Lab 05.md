Tommy Su 83203398
Partner: Ryan Mahinpey 39959770

Objective: We are trying to map the pressure distribution of sound waves inside a tube for $f_{0}$. We are also trying to determine the speed of sound
	- We know harmonic sound wave, we can find anti-nodes and nodes by mapping out the pressure and seeing where the pressure has maximum amplitude and minimum amplitude to find out the wavelength of the sound wave
	- The wavelength of a sound wave is the distance between peaks of the wave for a snapshot in time (note: the wavelength is related to the speed of sound)
	- The speed of sound is also related to frequency, which we would find by using a time vs pressure graph of the sound wave

Variables used in the calculations later on:
$f$ is frequency in $Hz$
$n$ is the harmonic number 
$v$ is the speed of the sound wave in $\frac{m}{s}$
$L$ is the length of the tube in meters
$m$ is the ratio of $\frac{f}{n}$

Note: in the previous lab, we forgot to add the uncertainty of the oscilloscope, as we took the frequency reading from the waveform generator instead of the oscilloscope

The uncertainty equation derivation is taken from the previous lab:
We start with a known $\frac{f}{n}$ taken from matlab
$$\frac{f}{n} = m$$
$$v = 2mL$$
$$\delta v = \sqrt{ 4 L^{2} \delta m^{2} + 4 \delta L^{2} m^{2} }$$
$$\delta v = 2\sqrt{ L^2\delta m^2+m^2\delta L^2 }$$


Below is the procedure copied from last time with edits made in the notes:
**Procedure**
Note: for the uncertainties for our oscilloscope measurements, we used 1/4 of the variation in the peaks.
We are doing procedure #2
1. First, connect the waveform generator, oscilloscope, and speaker box to power. Then, a splitter at ch1 of the waveform generator is connected to the oscilloscope at ch2 and "sine in" at the speaker box. And then, connect ch1 of the oscilloscope to the speaker box at "scope", and the microphone into the speaker box.
2. put the tube right up to the speaker, and set up the microphone in the center of the tube
3. Then, find the first fundamental frequency by playing around at around 300-400 hz on the waveform generator, until you find the peak on the oscilloscope.
4. Record this data point for frequency and record the harmonic
5. repeat for 3rd 5th, and extra harmonics if necessary
6. Then, graph it on matlab, find the slope, and use the equations above to find the speed of sound

Tools used:
- oscilloscope
- meter stick
- tube
- speaker
- waveform generator
![[Pasted image 20240214172431.png]]
![[Pasted image 20240214181118.png]]

Data collection:
We are using the procedure as depicted above to get the frequency of the harmonics
To get the uncertainty of each frequency, we are reading 1/4 of the fluctuations on the oscilloscope
We only used odd harmonics, as that would put a pressure anti-node in the centre, unlike even harmonics, which would result in pressure nodes.
Note: our resolution for the oscilloscope is different for each harmonic, but they are in ms from the oscilloscope, so to get our uncertainty, we have to get it in terms of Hz, which we can do by using the same ratio we used to go from period to frequency, or when the waves were really shaky, we would use 1/4 of the range that they were moving in

| n   | f                        |
| --- | ------------------------ |
| 1   | $322.6\pm 5$ $\text{Hz}$ |
| 3   | $950.6\pm 2 \text{Hz}$   |
| 5   | $1590\pm 4\text{Hz}$     |
| 7   | $2210\pm$ $2\text{Hz}$   |
| 9   | $2810\pm$ $$             |
