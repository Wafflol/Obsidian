Tommy Su 83203398
Partner: Ryan Mahinpey 39959770
3/13/2024

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

We recorded 1 exponential decay graph as seen in the picture:
![[Pasted image 20240313174553.png|325]]
Then, we imported it into matlab, which gave us this graph:
![[Pasted image 20240313174810.png|450]]
Then, we truncated the data from 35000 to 25000, and took the natural log of the voltage and graphed it again:
![[Pasted image 20240313175119.png|450]]
Then, we found the linear fit graph using matlab:
![[Pasted image 20240313175245.png|425]]
Using this graph, we get the following values:
$$m = -20500 \pm 1 \text{ V/s}$$
Thus, using our values and equations from above:
$$C = 10.492* 10^{-9} \pm -2 * 10^{-12} \text{ F}$$
Note: When we first calculated the capacitance, we got 3 times the expected value. After trying to figure out how to improve our accuracy, as the capacitance was way off, we realised that our offset was messing up our data, making it no longer linear. By subtracting 2 volts from every single data point prior to linearization, our final value for $C$ was a lot closer to the expected value.

**Reflection**
Pulled from above, the expected capacitance was $10.00\pm 0.005 \text{ nF}$. Compared to our measured capacitance, $C = 10.492* 10^{-9} \pm -2 * 10^{-12} \text{ F}$, we were very close to the expected value. 

Overall, our procedure went pretty smoothly. Our uncertainty was very low compared to other groups.

The uncertainty was very low, as we only used the digital equipment to get our measurements, and the oscilloscope has a very low uncertainty. The majority of the uncertainty comes from the measurement of the resistance from the DMM.
Additionally, we made the assumption that there is no resistance in the wires for our calculations, and that the resistance comes from only the resistor.

Our precision can be attributed to the high precision of the oscilloscope, and our procedure eliminates human error. 

Our result was a lot more accurate than  lab 06, due to some of the improvements we made. 



**Improvements**:
One improvement we made was by truncating out the end part of the exponential decay graph. We did this because when the graph nears the x-axis, the values become extremely small, and are thus, sensitive to the factors that attribute to errors in our readings, such as resistance in the wires. Thus, by only taking the steeper part of the graph, we take much more robust values that attribute to a slope of higher accuracy.

Another improvement we made was that we used a lower frequency, which meant that each period was longer, and thus, there were more data points that we could use. Last time, we had to truncate a lot of data because there was more than one period on the screen of the oscilloscope. However, this time, due to a lower frequency, there were more data points we could use, which attributed to a higher accuracy. (see the diagram below)

(This paragraph is half copied from the note above) 
The final improvement we made was that when we first calculated the capacitance, we got 3 times the expected value. After trying to figure out how to improve our accuracy, as the capacitance was way off, we realised that our offset was messing up our data, making it no longer linear. By subtracting 2 volts from every single data point prior to linearization, our final value for $C$ was a lot closer to the expected value.

Thus, due to the improvements we made, our measured capacitance had an extremely high accuracy.
![[Pasted image 20240313182712.png]]

Overall, if we were to do this lab again, we would measure the resistance of the entire circuit to get rid of the assumption that there's no resistance elsewhere in the circuit.