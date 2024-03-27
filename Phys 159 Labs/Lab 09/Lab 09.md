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
- Then, use three weights to find the calibration factor:
	- attach the weights one by one onto the syringe
	- give the syringe a slight tug to overcome the static friction
	- measure the reading from the scale each time as well as the final volume
	- also record the masses of each weight
	- then divide the mass of the weights by the reading when they were on the syringe to get a ratio of the masses, and take their average
- attach an assortment of masses to the syringe and measure the final volume of the syringe for each mass (repeat for 5 masses)
	- make sure to give the syringe a tug to overcome static friction
- convert the mass to force, and then graph it against 1/volume in matlab
- use matlab to find the slope and y-intercept
- use the equations above to find the values and the uncertainties

These are the equations we derived from Lab 08:
$$P_{atm} = \frac{b}{-A}$$
$$d = -\frac{m}{VART}$$
$$\delta d = \frac{1}{RA^2T^2V^2}\sqrt{ A^{2} T^{2} V^{2} \delta m^{2} + A^{2} T^{2} \delta V^{2} m^{2} + A^{2} V^{2} \delta T^{2} m^{2} + T^{2} V^{2} \delta A^{2} m^{2} }$$
$$\delta P_{atm} = \sqrt{ \frac{A^{2} \delta b^{2} + \delta A^{2} b^{2}}{A^{4}} }$$
