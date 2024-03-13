Tommy Su 83203398
Partner: Ryan Mahinpey 39959770
3/6/2024

1. **Clarify objective**
	- Objective: We are trying to find the capacitance of a capacitor,
	- The capacitance of a capacitor is related how much charge a capacitor can hold
	- The amount of charge a capacitor is also related to the voltage of the power supply


Variables used in the calculations later on:
$V$ is voltage in $volts$
$R$ is resistance in $\Omega$
$C$ is capacitance in $F$

Our uncertainty was calculated in the previous lab:


**Procedure**
1. Measure and record the resistance of the resistor using the DMM
2. Set up circuit same as in picture
	1. Connect the waveform generator, resistor, and capacitor in series, and connect the DMM across the capacitor in parallel
3. On the waveform generator, create a square wave, and adjust the frequency and amplitude until you get a good exponential decay curve on the oscilloscope that shows the max and min (make sure you see the graph plateau before it switches)
4. Add an offset on the oscilloscope to make sure the graph is above the x axis so there are no negative values
5. Use a usb to download the data and input it into matlab
6. Use matlab to linearize data, and then calculate the capacitance using the slope and the derived equations
![[Pasted image 20240306191135.png|200]]
