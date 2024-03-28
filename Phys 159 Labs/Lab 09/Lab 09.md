Tommy Su 83203398
Partner: Ryan Mahinpey 39959770
3/27/2024

- Objective: We are trying to measure the pressure in the room and measure the molar density of air
- We know that the pressure in the room is equivalent to 1 atm, and it is caused by the pressure of the gas molecules in the air. It is related by the volume of a space, as well as the number of molecules and the temperature
- The pressure of a gas is how much pressure that the weight of air exerts of the earth
- Molar density is the related to the number of molecules per volume of space
- thus, the units for molar density is mol/volume


**Procedure**
Tools used: Lever, fulcrum, support, pin, scale, calilper, syringe, weights, vice
- First, set up the apparatus like shown in the picture: (make sure to plug up the syringe)
- ![[Pasted image 20240320190951.png|400]] 
	- Attach the lever to the base of the arm, and fix it to the table using the vice
	- attach the pin to the center of the arm, and rest it onto the scale
	- attach the syringe to the end of the arm, and then plug it up using the stopper
- Measure initial volume by observing side of syringe and record it
- Find the force of friction:
	- measure the mass of the syringe plunger
	- first set the syringe to a large enough initial volume
	- pull the syringe down and let it go back up by itself
	- record the final volume, and use $P_{1}V_{1}=P_{2}V_{2}$ from the ideal gas law to calculate $P_{2}$, the pressure of the gas inside the syringe
	- subtract that from the atmospheric pressure (assumed), to get $\Delta  P$
	- then, use the equation $F_{f} = A*\Delta P-mg$ to find the force of friction, where $A$ is the area of the plunger, $m$ is the mass of the plunger, and $g$, is the acceleration due to gravity
- Then, use three weights to find the calibration factor:
	- attach the weights one by one onto the syringe
	- give the syringe a slight tug to overcome the static friction
	- measure the reading from the scale each time as well as the final volume
	- also record the masses of each weight
	- then divide the mass of the weights by the reading when they were on the syringe to get a ratio of the masses, and take their average
- attach an assortment of masses to the syringe and measure the final volume of the syringe for each mass (repeat for 5 masses)
	- to take the measurements, pull the masses down and let it go back up by itself
- convert the mass to force, subtract the calculated force of friction from it, and then graph it against 1/volume in matlab
- use matlab to find the slope and y-intercept
- use the equations below to find the values and the uncertainties

These are the equations we derived from Lab 08:
$$P_{atm} = \frac{b}{-A}$$
$$d = -\frac{m}{VART}$$
$$\delta d = \frac{1}{RA^2T^2V^2}\sqrt{ A^{2} T^{2} V^{2} \delta m^{2} + A^{2} T^{2} \delta V^{2} m^{2} + A^{2} V^{2} \delta T^{2} m^{2} + T^{2} V^{2} \delta A^{2} m^{2} }$$
$$\delta P_{atm} = \sqrt{ \frac{A^{2} \delta b^{2} + \delta A^{2} b^{2}}{A^{4}} }$$
Tools used:

![[Pasted image 20240320171348.png|150]]![[Pasted image 20240320171408.png|200]]![[Pasted image 20240320171428.png|170]]
![[Pasted image 20240320171450.png|200]]![[Pasted image 20240320171516.png|200]]![[Pasted image 20240320174014.png|200]]
FBD for the syringe:
![[Pasted image 20240320173704.png|269]]


**Derivation of equations taken from lab 08**:

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


**Experiment:**
Calibration factor table:
Note: while measuring the masses for the calibration factor, we measured the masses of the weights first, and then without changing the position of anything, we added the weights one by one to make sure the changing position of the pin wouldn't matter like it did in lab 08

| Mass (g $\pm 0.5g$) | Measured "Mass" (g $\pm 0.5g$) |
| ------------------- | ------------------------------ |
| 200                 | 377                            |
| 400                 | 751                            |
| 600                 | 1125                           |
Calibration factor (average of mass/measured mass): $0.532 \pm 0.006$
 -m/(V*
Note: for this lab, to improve our precision, we decided to start using a higher volume. (Justification in conclusion)

**Finding the force of friction**
Note: diameter = $14 \pm 0.03 mm$
Mass of piston: $12\pm 0.5g$ = $0.012 \pm 0.0005 kg$
$$F_{f}=F_{atm}-W$$
Starting volume = $4 \pm 0.1 mL$ -m/(V*
Starting pressure = $100.5 kPa$
Final volume = $5 \pm 0.1 mL$

Explanation for finding force of friction:
We know that the force of static friction should always be the same, as it is based on the normal force, which comes from the expansion of the rubber. Thus, to get a better graph, we should subtract the force of friction from our final graph to account for it.
Thus, to find the force of friction, we first measure the weight of the syringe handle, and plug the syringe up at 4 mL. Then, we pull down on the syringe, and let it go back up. The syringe stops at a different volume than its starting position due to static friction. Using the ideal gas law, we get that $$P_{1}V_{1}=P_{2}V_{2}$$
From our calculations, we get $P_{2} = 87 \pm 3$ kPa
Thus, using this equation:
$$F_{f} = A\nabla P - mg$$
$$\delta F_{f} = \sqrt{ A^{2} \delta \nabla P^{2} + \nabla P^{2} \delta A^{2} + \delta m^{2} g^{2} }$$
We get that friction is $F_{f} = 2.0 \pm 0.5 N$

Onto the actual procedure:
Using our procedure above, we took the measurements as we did last lab:

| **mass  ($g \pm 0.5g$)** | V ($mL \pm 0.1mL$) |
| ------------------------ | ------------------ |
| 0                        | 4                  |
| 681                      | 4.8                |
| 1178                     | 5.5                |
| 1498                     | 6.4                |
| 1872                     | 8                  |
| 2229                     | 10.2               |

| $F_{ext} (N \pm 0.1N$) | $\frac{1}{V}L \pm 0.0005 L$ |
| ---------------------- | --------------------------- |
| 0                      | 250.000                     |
| 3.6                    | 208.330                     |
| 6.2                    | 181.810                     |
| 7.8                    | 156.250                     |
| 0.7                    | 125.000                     |
| 11.6                   | 98.039                      |
Subtracting friction, we get the new table:

| $F_{ext} (N \pm 0.5N$) | $\frac{1}{V}L \pm 0.0005 L$ |
| ---------------------- | --------------------------- |
| -2                     | 250.000                     |
| 1.6                    | 208.330                     |
| 4.2                    | 181.810                     |
| 5.8                    | 156.250                     |
| 7.7                    | 125.000                     |
| 9.6                    | 98.039                      |

From matlab, we got that the slope $m = -0.076 \pm 0.005 N*L$
and $b = 17.3 \pm 0.8 N*L$

Thus, using a matlab script where I entered in the equations we derived:
![[Pasted image 20240327183218.png]]
We get that 
$$P_{atm} = 100 \pm 6 kPa$$
$$d = 50 \pm 3 \frac{mol}{m^3}$$
where $P_{atm}$ is the atmospheric pressure, and $d$ is the molar density of the air

**Reflection**:
Overall, our $P_{atm} (100\pm 6 kPa)$ agreed with the expected value of $100.5 kPa$, while our molar density of $50\pm 3 \frac{mol}{m^3}$ did not agree with the expected value of $41 \frac{mol}{m^3}$. This time, unlike lab 08, we made sure to calculate the uncertainty coming from every single source where applicable, as time was less of an issue, giving us a greater precision for our uncertainty.

In our procedure, we made a few assumptions, which affected the accuracy of our measurements. First, we assumed that there is a perfect relationship between pressure and volume, but that assumes that there is no air leakage, which is not necessarily true. Another assumption we made was that the piston was in impending motion, and that $F_{f} = \mu N$, but static friction is not always $= \mu N$, and can be less than that. Thus, it is likely that our calculated friction is higher than it should be. We also assume that everything is in perfect alignment, which isn't true, and because they aren't in perfect alignment, the weight would add extra force onto the walls, increasing $N$, and thus adding extra friction. Additionally, we assume that the gas behaves like an ideal gas, which isn't true, as the particles have volume, collide with each other, and have inter-molecular forces, which changes the relationship between $P$ and $V$.

Our improvements in accuracy were due to many of the improvements we made, which can be seen by the fact that our calculated values are a lot closer to the expected values than what we calculated in lab 08.

**Improvements**
The first improvement we made was to increase the initial volume of the syringe. This increases our accuracy, as each ml increase in volume inside the syringe corresponds to a lower decrease in pressure. Thus, for the same decrease in pressure (or in other words, using the same mass), there would be a greater increase in volume, which means our reading would be a lot more accurate.

Another improvement we made was to account for the force of friction. We know that when we pull the mass down, and let it rise up, it gets stopped by friction, so the forces on the syringe are the pressure inside the syringe, the gas outside, the force from gravity, and the force of friction. And because the force of friction is $F_{f} = \mu N$, where $N$ comes from the rubber pushing against the wall, it should always be constant, as $N$ is orthogonal to the force of the weights. Thus, calculating the force of friction in the way we showed, got that the force of friction was roughly $2 N$. And because the y-axis of the graph was $F_{ext}$, and friction works in the opposite direction of $F_{ext}$, if we subtract $2N$ from every single point, we end up accounting for friction for every data point, greatly improving our accuracy. This mattered a lot, as you can see in the table, of our forces, subtracting $2N$ had a very big difference on every data point.

Another improvement we made was to make sure that while measuring the masses for the calibration factor, we measured the masses of the weights first, and then without changing the position of anything, we added the weights one by one to make sure the changing position of the pin wouldn't matter like it did in lab 08. Also, we made sure to use multiple data points for our calibration unlike last lab.

Additionally, we also made sure that the stopper stayed on throughout the entire measurement process so that we were working with the same initial volume/moles of air.