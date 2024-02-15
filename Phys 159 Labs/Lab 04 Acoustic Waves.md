Tommy Su 83203398
Partner: Ryan Mahinpey 39959770
2/14/2024

1. **Clarify objective**
	- Objective: We are trying to map the pressure distribution of sound waves inside a tube for $f_{0}$. We are also trying to determine the speed of sound
	- We know harmonic sound wave, we can find anti-nodes and nodes by mapping out the pressure and seeing where the pressure has maximum amplitude and minimum amplitude to find out the wavelength of the sound wave
	- The wavelength of a sound wave is the distance between peaks of the wave for a snapshot in time (note: the wavelength is related to the speed of sound)
	- The speed of sound is also related to frequency, which we would find by using a time vs pressure graph of the sound wave
2. **Explore Tools**

| Tool | Physical Parameter | Resolution | Reading Uncertainty | Range | Usage |
| ---- | ---- | ---- | ---- | ---- | ---- |
| Osciilloscope | Voltage | 100mV | 50mV | -150V-150V | To measure the voltage in a circuit |
| Ruler | Length | 1mm | $\pm 0.5mm$ | 0cm-100cm | To measure length for a long object |
![[Pasted image 20240214174719.png]]
We also used a microphone, speaker box, and waveform generator

Note: we used a waveform generator, but it is not in the table for obvious reasons

Shown below is a picture of the setup. + tools used. To replicate, connect the waveform generator, oscilloscope, and speaker box to power. Then, a splitter at ch1 of the waveform generator is connected to the oscilloscope at ch2  and "sine in" at the speaker box. And then,
we connect ch1 of the oscilloscope to the speaker box at "scope", and the microphone into the speaker box.
![[Pasted image 20240214172431.png]]
Below is a drawing of the contraption:
![[Pasted image 20240214181118.png]]
Note: to make sure our speaker is working, we will have our generator at just a high enough amplitude so that we can hear it faintly

Experimenting with the setup:
While testing the microphone and the speaker without the tube, we noticed that the amplitude of the microphone signal decreased as some function of distance
As we increased the frequency on the waveform generator, the distance between the peaks on the oscilloscope decreased, while the opposite happened when we decreased the frequency

While testing the microphone and speaker with the tube:
As we slid the microphone to the right, the amplitude on the oscilloscope would change from very big to very small. We think this is because we are finding the pressure anti-nodes and nodes that are created by the sound waves

After testing from 300-400hz with the generator, we found that the highest peak in the middle of the tube was found at 323.2 Hz. This is our experimental fundamental frequency of the tube

Note: we used the meter stick to place the mic in approximately the centre of the tube

3. **Relate Quantities**
	NOTE: we put our uncertainty equations and calculations in test and try for each method
	- We can measure
		- the frequency of a sound wave
		- the length of the tube
		- amplitude of the sound wave using voltage
4. **Test & Try**
	One possible procedure:
		We put the microphone on one end of the tube, where the end closest to the speaker was set as position = 0. We then moved the microphone across 5 equidistant points along the tube 13cm across, and got the following data points + graph after plotting
		After finding our fundamental frequency, we can measure the wavelength of the sound wave, and using the equation $v = \lambda f$, for waves, we can find the speed of sound.
Below is the data copied from matlab:

| amplitude (V) | position (cm) |
| ---- | ---- |
| 0.3$\pm 0.01$ | $0\pm 0.01$ |
| 2.54$\pm 0.04$ | $13\pm 0.01$ |
| 3.36$\pm 0.03$ | $26\pm 0.01$ |
| 2.9$\pm 0.03$ | $39\pm 0.01$ |
| 0.84 $\pm 0.03$ | $52\pm 0.01$ |
		![[Pasted image 20240214182733.png]]
From the waveform generator, we got that the fundamental frequency was $323.1\pm 0.05$ Hz
The length of the tube is $52.50\pm 0.05m$ 
Calculating our speed of sound from this, we get 339.3$\pm 0.3$m/s

Uncertainty equation (comes from the multiplication rule): 
Let $\lambda$ = wavelength
Let $f$ = frequency
Let $v$ = speed of sound
$$v = \lambda f$$
$$\delta v = \sqrt{ \lambda^{2} \delta f^{2} + \delta \lambda^{2} f^{2} }$$
Another possible procedure:
		We can find the 2nd harmonic frequency, 3rd, 4th, and so on, and then, using $\frac{f}{n}$ where f is the frequencies and n is the nth harmonic, to find $\frac{v}{2L}$, as $f = \frac{nv}{2L}$, and using the length of the tube, we can find the speed of sound.
We already found the first frequency from the last procedure:

| n | f |
| ---- | ---- |
| 1 | $323.1\pm 0.01$ $\text{Hz}$ |
| 3 | $9320.6\pm 0.01 \text{Hz}$ |
| 5 | $1553.5\pm 0.01\text{Hz}$ |





The two procedures differ in that the second method has more variables, which is associated with a higher uncertainty. Additionally, it is more complex, so there is more error.

Thus, we chose to use the first procedure.


5. **Procedure**
Note: for the uncertainties for our oscilloscope measurements, we used 1/4 of the variation in the peaks.

Tools used:
- procedure
Add pictures of procedure
	**Reflection**:
		