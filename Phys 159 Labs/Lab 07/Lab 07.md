Tommy Su 83203398
Partner: Ryan Mahinpey 39959770
3/6/2024

1. **Clarify objective**
	- Objective: We are trying to find the capacitance of a capacitor,
	- The capacitance of a capacitor is related how much charge a capacitor can hold
	- The amount of charge a capacitor is also related to the voltage of the power supply

Variables used in the calculations later on:
$V$ is voltage in $V$
$R$ is resistance in $\Omega$
$C$ is capacitance in $F$
$m$ is the slope of $\ln(V) \text{ vs. } t$, which is equal to $-\frac{1}{RC}$

Our uncertainty was calculated in the previous lab:
$$m = -\frac{1}{RC}$$
$$-Rm = \frac{1}{C}$$
$$C = -\frac{1}{Rm}$$
Using the general uncertainty equation, we can calculate the uncertainty:
$$\delta C = \sqrt{ \frac{R^{2} \delta m^{2} + \delta R^{2} m^{2}}{R^{4} m^{4}} }$$
$$\delta C = \sqrt{ \frac{\delta m^2}{R^2m^4}+\frac{\delta R^2}{R^4m^2}}$$
$$\delta C = \frac{1}{Rm}\sqrt{ \frac{\delta m^2}{m^2} + \frac{\delta R^2}{R^2}}$$



**Procedure**
1. Measure and record the resistance of the resistor using the DMM
2. Set up circuit same as in picture
	1. Connect the waveform generator, resistor, and capacitor in series, and connect the DMM across the capacitor in parallel
3. On the waveform generator, create a square wave, and adjust the frequency and amplitude until you get a good exponential decay curve on the oscilloscope that shows the max and min (make sure you the frequency is low enough that you can see the graph plateau before it switches from charging to discharging)
4. Add an offset on the oscilloscope to make sure the graph is above the x axis so there are no negative values
5. Use a USB to download the data and input it into matlab
6. Use matlab to linearize data, and then calculate the capacitance using the slope and the derived equations
![[Pasted image 20240306191135.png|200]]

Tools used:

![[Pasted image 20240306164359.png|150]]![[Pasted image 20240306164417.png|150]]![[Pasted image 20240306165244.png|200]]
![[Pasted image 20240306165303.png|175]]![[Pasted image 20240306165319.png|150]]![[Pasted image 20240306165329.png|200]]

**Experiment**:
Initial measurements:
Capacitor capacitance: $10.00\pm 0.005 \text{ nF}$
Resistor resistance: $4650 \pm 1 \Omega$

We 