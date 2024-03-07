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
$$X_{c}= \frac{1}{\omega c}$$
, which can be found through the circuit's impedance: $$z = \sqrt{ R^2+Xc^2 }$$
*derive equation*
	*derive uncertainties*
4. **Test & Try**
	One possible procedure:

	Another possible procedure:

	The two procedures differ in that


5. **Procedure**
Tools used:
- procedure
Add pictures of procedure
	**Reflection**:
		