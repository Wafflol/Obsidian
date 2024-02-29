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
For the length of the tube, we got:
$$L = 0.4990\pm 0.0005m$$

We are using the procedure as depicted above to get the frequency of the harmonics
To get the uncertainty of each frequency, we are reading 1/4 of the fluctuations on the oscilloscope
We only used odd harmonics, as that would put a pressure anti-node in the centre, unlike even harmonics, which would result in pressure nodes.
To determine the uncertainty for the frequency, we looked for the smallest frequency at which we observe the maximum amplitude, and find the largest frequency at which we still observe it, and then take half of that range to get the uncertainty.

| n   | f                       |
| --- | ----------------------- |
| 1   | $322\pm 1$ $\text{Hz}$  |
| 3   | $965\pm 5 \text{Hz}$    |
| 5   | $1595\pm 5\text{Hz}$    |
| 7   | $2210\pm$ $10\text{Hz}$ |
| 9   | $2810\pm$ $10\text{Hz}$ |
To get our pressure distribution for $f_{1}$, we collected 5 data points starting at the closest end to the speaker. We used 12.5 cm increments from one end of the tube.

Note: Here is an added procedure for it:
1. Use the same setup as the previous procedure for wiring
2. Measure the length of the tube, divide it by n-1 where n is the number of data points you want to measure
3. Take the first data point at the very end of the tube closest to the speaker
4. Increment by length/(n-1) until you get to the end of the tube
5. plot in matlab to see pressure distribution

To get the uncertainty for amplitude, we took 1/4 of the range of the amplitude variance

| Distance (cm) | Amplitude (V)    |
| ------------- | ---------------- |
| 0             | $0.081\pm 0.006$ |
| 12.5          | $1.11\pm 0.04$   |
| 25            | $1.39\pm 0.05$   |
| 37.5          | $1.15\pm 0.04$   |
| 50            | $0.13\pm 0.01$   |
Below is the graph of the pressure distribution of the sound waves inside the tube for $f_{1}$
![[Pasted image 20240228181202.png]]
For $f_{2}$, we did the same thing but with the second harmonic we found:

| Distance (cm) | Amplitude (V)  |
| ------------- | -------------- |
| 0             | $0.11\pm 0.01$ |
| 12.5          | $0.26\pm 0.02$ |
| 25            | $0.38\pm 0.02$ |
| 37.5          | $0.29\pm 0.03$ |
| 50            | $0.15\pm 0.01$ |
Below is the graph of the pressure distribution of the sound waves inside the tube for $f_{1}$


This is the starting position:
![[Pasted image 20240228180312.png]]And this was the end position:
![[Pasted image 20240228180344.png]]


Calculations for the speed of sound:

This is the graph we got from plotting the data we got:
![[Pasted image 20240228182828.png]]
$$m = \frac{f}{n} = 315.1\pm0.9$$
$$v = 2ml$$
Using the equations listed above, we get that
$$v = 314\pm 3 \text{m/s}$$
**Reflection**
This result is very reasonable, and has a relatively low uncertainty. Compared to other groups using different procedures, it was also pretty similar, so our final calculation seems to be relatively accurate.

Overall, our procedure went pretty smoothly. Our uncertainty was pretty high compared to other groups, but the reason we had such a high uncertainty was because we were unsure of which frequency was the peak frequency, so we factored that into our uncertainty. 
