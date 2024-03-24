
Tommy Su 83203398
Partner: Ryan Mahinpey 39959770
3/20/2024

1. **Clarify objective**
	- Objective: We are trying to measure the pressure in the room and measure the molar density of air
	- We know that the pressure in the room is equivalent to 1 atm, and it is caused by the pressure of the gas molecules in the air. It is related by the volume of a space, as well as the number of molecules and the temperature
	- The pressure of a gas is how much pressure that the weight of air exerts of the earth
	- Molar density is the related to the number of molecules per volume of space
	- thus, the units for molar density is mol/volume
2. **Explore Tools*

| Tool            | Physical Parameter | Resolution      | Reading Uncertainty | Range   | Usage                                         |
| --------------- | ------------------ | --------------- | ------------------- | ------- | --------------------------------------------- |
| Plunger/syringe | Volume             | 0.2 mL          | 0.1 mL              | 0-10mL  | To measure the volume of fluid in the syringe |
| Caliper         | Length             | 0.05mm          | 0.03mm              | 0-155mm | To measure the length of objects              |
| Scale           | Mass               | 1g              | 0.5g                | 0kg-5Kg | To measure the mass of objects                |
| Meter stick     | Length             | 0.1cm           | 0.05cm              | 0-100cm | To measure longer lengths of objects          |
| Thermostat      | Temperature        | 0.1 $\degree C$ | 0.05$\degree C$     |         | To measure the temperature of the room        |
We also have lever and fulcrum, as well as a pin that goes through the lever
We also have a vice to hold the parts together
![[Pasted image 20240320171348.png|150]]![[Pasted image 20240320171408.png|200]]![[Pasted image 20240320171428.png|170]]
![[Pasted image 20240320171450.png|200]]![[Pasted image 20240320171516.png|200]]![[Pasted image 20240320174014.png|200]]



3. **Relate Quantities**
	- what we can measure
		- volume in syringe
		- force on scale from pin
		- mass of weights
		- distance from fulcrum to pin and syringe
	![[Pasted image 20240320173704.png|269]]
	From the FBD, we can see that there are three forces on the syringe: the force from the atmosphere, the force from the gas, and the external force.
	We know that the cross sectional area $A$ of the plunger times the pressure of the atmosphere is equal to the force $F_{atm}$ of the atmosphere:
	$$F_{atm} = AP_{atm}$$
	Similarly, the force of the gas is the area $A$ times the pressure of the gas inside the syringe, $P_{gas}$:
	$$F_{gas} = AP_{gas}$$
	Going back to gasses, we know through the ideal gas law that $PV = nRT$, where $P$ is pressure, $V$ is volume, $n$ is the number of moles, $R$ is the gas constant, $T$ is the temperature of the gas.

	From the FBD, we can add the forces together based on their signs, with the upwards direction being positive:
	$$F_{ext}+F_{atm}=F_{gas}$$
	From here, we can move $F_{atm}$ to the other side:
	$$F_{ext} = F_{gas} - F_{atm}$$
	Then, replacing $F_{gas}$ and $F_{atm}$ with $AP_{gas}$ and $AP_{atm}$ respectively, we get:
	$$F_{ext} = AP_{gas}-AP_{atm}$$
	Then, we can replace $P_{gas}$ with $\frac{nRT}{V}$ from the ideal gas law mentioned above:
	$$F_{ext} = AnRT\left( \frac{1}{V} \right)-AP_{atm}$$
	From here, a plot of $F_{ext}$ over $\frac{1}{V}$ gives us a slope of $AnRT$, which I will replace as $m$, and a y-intercept $-AP_{atm}$, which I will call $b$.

	Using $b$, we can divide it by $-A$, which gives us $P_{atm}$
	Thus, $$P_{atm} = \frac{b}{-A}$$


	To find the molar density of the air, we can use the slope $m$, and divide it by $ART$, which gives us $n$. Then, we can divide $n$ by the original volume $V$, which gives us molar density, $d$: NOTE: we added a negative to the density because slope s=will be negative
	$$d = \frac{n}{V}$$
	$$n = \frac{m}{ART}$$
	$$d = -\frac{m}{VART}$$
	We need to find the uncertainty equations for $P_{atm}$ and $d$:
	They can be found using the general uncertainty equations:
	
	$$\delta d = \frac{1}{RA^2T^2V^2}\sqrt{ A^{2} T^{2} V^{2} \delta m^{2} + A^{2} T^{2} \delta V^{2} m^{2} + A^{2} V^{2} \delta T^{2} m^{2} + T^{2} V^{2} \delta A^{2} m^{2} }$$
	
	$$\delta P_{atm} = \sqrt{ \frac{A^{2} \delta b^{2} + \delta A^{2} b^{2}}{A^{4}} }$$
4. **Test & Try**
	Note: Before we do our procedures, we need to find/calibrate the ratio of the mass reading on the scale to the actual mass hanging on the syringe. To do so, we measured the mass of the masses by the mass reading from the pin on the halfway point on the lever. Finding the average of 4 readings gives us a good estimate of the mass ratio. From our average, we got that the ratio was $r = \frac{5}{9}$

	One possible procedure:
	We can attach 3 masses to the syringe, and then we can measure the volume that the syringe stretches to. Tabulating this data with the mass of the weights:
	
| **mass  ($g \pm 0.5g$)** | V ($mL \pm 0.1mL$) |
| ------------------------ | ------------------ |
| 0                        | 2                  |
| 1685                     | 3.1                |
| 1896                     | 3.5                |
| 2791                     | 6.9                |
Mass was measured, multiplied by 9.81 then divided by 1000 to find force, then scaled by the calibration factor found earlier.

| $F_{ext} (N \pm 0.1N$) | $\frac{1}{V}L \pm 0.0005 L$ |
| ---------------------- | --------------------------- |
| 0                      | 500.0                       |
| 9.2                    | 322.8                       |
| 10.8                   | 285.7                       |
| 15.2                   | 144.9                       |
Graphing this in matlab, we can get the slope $m$ and the intercept $b$:
![[Pasted image 20240320182720.png]]
$$m = -0.0433 \pm 0.0005 N*L$$
$$b = 22.4 \pm 0.2 N*L$$
Thus, solving for the molar density and atmospheric pressure:
Note: diameter = $14 \pm 0.03 mm$, temp = $296.55 \pm 0.05  K$, original volume is $2mL \pm 0.1 mL$
Note: we also converted the units to SI units in calculation:
$$d = 57\pm 1 \frac{mol}{m^3}$$
$$P_{atm} = 150kPa \pm 1.0*10 kPa$$

Another possible procedure:
For this procedure, we will repeat the same procedure as before, except instead of using the masses, we will use our hands to pull down on the syringe:

| **mass  ($g \pm 0.5g$)** | V ($mL \pm 0.1mL$) |
| ------------------------ | ------------------ |
| 0                        | 6                  |
| 1600 $\pm 100g$          | 4                  |
| 1500 $\pm 50g$           | 3                  |
| 4500 $\pm 100g$          | 2                  |
The uncertainties were found by taking the range of values on the scale. This is appropriate because there are huge fluctuations.

Forces were found in the same manner as before

| $F_{ext} (N \pm 0.1N$) | $\frac{1}{V}L \pm 0.0005 L$ |
| ---------------------- | --------------------------- |
| 0                      | 166.6                       |
| 8.72 $\pm 2N$          | 250                         |
| 9.175 $\pm 2N$         | 333.3                       |
| 24.825 $\pm 2N$        | 500                         |
The uncertainties for $F_{ext}$ were decided to be increased due to the fact that there were rapid fluctuations in our measurements. It was standardised to the highest uncertainty value we found.

Calculations are the same as procedure 1:
![[Pasted image 20240320185834.png]]
$$m = 0.072 \pm 0.007 N*L$$
$$b = -12 \pm 1 N*L$$
$$d = 9.0*10 \pm 2.0 * 10 \frac{mol}{m^3}$$
$$P_{atm} = 8.0*10 \pm 2.0 * 10 kPa$$
The two procedures differ in that one uses weights to change the force applied, while the other uses our hands to change the force applied. The first procedure is much more accurate and has a lower uncertainty, so we chose the first one.


5. **Procedure**
Tools used: Lever, fulcrum, support, pin, scale, calilper, syringe, weights
- First, set up the apparatus like shown in the picture: (make sure to plug up the syringe)
- ![[Pasted image 20240320190951.png|400]] 
- Then, use three weights to find the calibration factor:
	- attach the weights one by one onto the syringe
	- measure the reading from the scale each time
	- also record the masses of each weight
	- then divide the mass of the weights by the reading when they were on the syringe to get a ratio of the masses, and take their average
- attach an assortment of masses to the syringe and measure the volume of the syringe for each mass
- convert the mass to force, and then graph it against 1/volume in matlab
- use matlab to find the slope and y-intercept
- use the equations above to find the values and the uncertainties
**Reflection**:
Overall, neither of our values agreed with the accepted/expected values for the density and pressure. Although, the values we got for the first procedure were a little more accurate than the second procedure. 
For the calculations, we assume the process is isothermal, but in reality, there should be a bit of a change in temperature when the gas expands/compresses.
We also assume that friction is negligible, which it isn't. 
The uncertainty of our measurement for pressure was very high, which we think could be due to a calculation error, which is pretty easy to fix.