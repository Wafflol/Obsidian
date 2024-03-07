Tommy Su 83203398
Partner: Ryan Mahinpey 39959770
3/6/2024

1. **Clarify objective**
	- Objective: We are trying to find the capacitance of a capacitor,
	- The capacitance of a capacitor is related how much charge a capacitor can hold
	- The amount of charge a capacitor is also related to the voltage of the power supply
2. **Explore Tools**

| Tool          | Physical Parameter                     | Resolution | Reading Uncertainty | Range      | Usage                                                                            |
| ------------- | -------------------------------------- | ---------- | ------------------- | ---------- | -------------------------------------------------------------------------------- |
| Osciilloscope | Voltage                                | 200mV      | 100mV               | -150V-150V | To measure the voltage in a circuit                                              |
| DMM           | Voltage/Resistance/Capacitance/Current | 0.1 nF     | 0.05 nF             |            | To measure the voltage/resistance/capacitance/current of components in a circuit |
|               |                                        |            |                     |            |                                                                                  |
We measured the capacitance of the capacitor with the DMM to get an expected value for later: 101.6 $\pm 0.05$ nF
Using the DMM, we can measure the resistances of the two resistors: 1986$\pm 1\Omega$, and $5055 \pm 1 \Omega$
Note: we are just using the 5055 $\Omega$ resistor for this lab

We also used a breadboard, a PCB, 2 resistors, a capacitor, and the waveform generator.

![[Pasted image 20240306164359.png]]
![[Pasted image 20240306164417.png]]
![[Pasted image 20240306165244.png]]
![[Pasted image 20240306165303.png]]
![[Pasted image 20240306165319.png]]![[Pasted image 20240306165329.png]]
Here is a picture of our circuit:
![[Pasted image 20240306172636.png]]
And this is our circuit diagram
![[Pasted image 20240306172849.png]]
3. **Relate Quantities**
	- We can measure voltage drops using a DMM 
		- *replace with measurements ex. length of string*
	We know that $q = CV$ where $q$ is charge on a capacitor, and $C$ and $V$ are the capacitance and voltage of the circuit respectively
	Thus, if we know the charge and voltage, we can find capacitance.
	We know that for a capacitor, when it is charging, $V(t) = V_{0}e^{-t/RC}$, so if we can find the time the time at which voltage is at 63% of the maximum, that time would equal $RC$, and if we divide by the resistance, we can find capacitance.
	In an AC circuits we know that the current is $V = IZ$. Capacitors behave differently, and their reactance is found by 
$$X_{c}= \frac{1}{\omega C}$$
, which can be found through the circuit's impedance: $$z = \sqrt{ R^2+X_{c}^2 }$$
Note: we decided not to go the impedance route, but I kept the relate quantities part for it here.
Note 2: The equations + uncertainty equations are in test and try, as they use different equations
4. **Test & Try**
	One possible procedure:
		Use the waveform generator to create a square AC wave, so that the capacitor is constantly charging and discharging. Then, using the oscilloscope, find the $V_{max}$, of the capacitor using the cursors, and find out the time $t$ it takes to charge to $63$% of $V_{max}$, which is equal to $\tau$. We know $\tau = RC$, and thus, we can find $C = \frac{\tau}{R}$
		For the calculations:
			We get $V_{max}$ from the oscilloscope, and using that we calculate 0.63*$V_{max}$, and using that, we find t for 63%.
			Thus, we just need to use the formula:
$$C = \frac{\tau}{R}$$
And for uncertainty:
$$\delta C = \sqrt{ \frac{\delta R^{2} \tau^{2} + \delta \tau^{2} R^{2}}{R^{4}} }$$
Running 1 test trial:
$V_{max} = 8.6 \pm 0.2V$
63% of $V_{max} = 5.41 \pm 0.1V$
Using the graph,
$$\tau = t = 283\pm 50 \mu s$$
$$= 0.000283 \pm 0.00005\mu s$$
From above, we know that $R = 5055\pm 1\Omega$

Thus, calculating our values, we get capacitance $C = 6*10^{-8}\pm 1*10^{-8} F$

Another possible procedure:
We can graph the natural log of the discharging function of voltage with respect to time on matlab.
Explaining the equation:
Going from $$V(t) = V_{0}e^{-t/RC}$$
$$\ln(V(t)) = \ln(V_{0})-\frac{1}{RC}t$$
From this form, we can see that if treat $\ln(V(t))$ as the $y$ axis, and $t$ as the $x$ axis, the slope will be $-\frac{1}{RC}$
Thus, if we call the slope $m$, the equation for $C$ can be found like this:
$$m = -\frac{1}{RC}$$
$$-Rm=\frac{1}{C}$$
$$C = -\frac{1}{Rm}$$
and thus the uncertainty is:
$$\delta C = \sqrt{ \frac{R^{2} \delta m^{2} + \delta R^{2} m^{2}}{R^{4} m^{4}} }$$
From our graph, we got ![[Pasted image 20240306190258.png]]
$$m = $$


The two procedures differ in that


5. **Procedure**
Tools used:
- procedure
Add pictures of procedure
	**Reflection**:
		