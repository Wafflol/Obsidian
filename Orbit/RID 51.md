|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1) The Space Debris Mitigation Plan / Report (SDMP / SDMR) shall be prepared according to ESSB-ST-U-007 and contain a compliance and verification matrix with all the requirements in ESSB-ST-U-007.  <br>  <br>2) The maximum orbit altitude to comply with LEO clearance in less than 5 years shall be analyzed according to the correct timeline and ESSB-ST-U-007 (sect. 6) to capture solar cycle variability such to confirm the feasible orbit altitude.  <br>  <br>3) The risk of battery cell explosion and break-up probability (towards 10-3 threshold) shall be assessed taking into account battery cell procurement, battery cells safety devices, battery qualification/acceptance tests, worst-case thermal conditions, structural consequences in terms of debris generation in case of battery cells explosion. |
|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |

1.  Still WIP, will be fixed by next SATPF. Only have template set up, is it correct to use all LEO applicable requirements from ESSB-ST-U-007 Table C-1: Requirements applicability matrix?

2.  Acknowledged. How far apart should each iteration of the simulation be run in to insure full coverage of solar cycle variability? Also need clarification on "correct timeline" (Use launch date of 2027 Q4?). 
	Need guidance on solar cycle model: as per A.2.8 of ESSB-HB-U-002, ECSS has a higher fidelity than Monte Carlo Sampling - is there a reason not to use ECSS sample solar cycles in DRAMA/OSCAR?
	In ESSB-ST-U-007 section 6.2.g, need clarification on what percentile is referring to.

3. The battery pack is procured from ISISpace and the battery cells are unprotected 18650 type cells from Panasonic/Sanyo that have been extensively used in both terrestrial and orbital systems. Upon request we can provide the datasheets for the batteries.
	1. Qualification and acceptance testing:
		1. Follows IPC-A-610 Class 3 standard
		2. QT: Functional, Vibration, Mechanical Shock, Thermal Cycling, Thermal Vacuum
		3. AT: Functional, Thermal Cycling
	2. Flight heritage and quality assurance from manufacturer
			1. Design based on heritage from ICEPS1 design flown on PEASSS CubeSat (2016)
		1. ICEPS2, second generation, flown on the Hiber 1,2 CubeSats (2018)
		2. Qualification Thermal Testing, -40 to +80 degrees Celsius
		3. Design qualification load Static +10.8 [g], three axes 
		4. Sine and Random Vibration ASAP5 Qualification Levels
		5. IPC-A-610 Class 3 PCB, flight units thermally acceptance tested
		6. PBP-4S1P has deployment heritage from ISS.
		(not too sure how to analyze structural consequences in case of explosion) 
![[Pasted image 20241014204349.png]]
 ![[Pasted image 20241014200844.png|825]]
![[Pasted image 20241014202258.png]]

1. Acubesat:
   Battery Cells The battery pack bears the Nanoavionics credibility as one of the leading companies in the nano-satellite mission design field (ISO 9001 certified). Flight-heritage data from previous successful missions using the same EPS Board [7, Sect. 2.7] are to be found in the NanoSats Database. According to [8], the battery pack's design provide over-voltage and over-current protection measures. As a result the function of the battery cells will remain at the desirable level avoiding any potential mission threatening event [7, Sec. 2.6]. The thermal analysis concluded to the maximum and minimum temperature values for 18 Space Debris Mitigation Report [SDMR] ASAT_SDMR_2021-05-31_v2.2 the baseline orbit (LTAN 6) in which the EPS board will be exposed to [4, Sec 2.2]. These values are cited in Table VI. Table VI: EPS’s Board Maximum & Minimum Exposed Temperature Scenarios Values Hottest Case 20.84 ◦C Coldest Case -8.816 ◦C Based on Table V it is confirmed that the exposed temperature for the battery cells is within the acceptable limits. Furthermore, an on-board heater is integrated allowing the user to select the desirable temperature levels for the batteries [7, Sect. 2.3] while guaranteeing that these will remain between the acceptable limits. Another potential danger for the battery cells to malfunction is the exposure to radiation. The radiation analysis concluded that as far the baseline orbit is concerned the TID equals to 3.9 krad during the entirety of the mission [11]. The Nanoavionics EPS board is tested to NASA GEVS environmental levels and up to 20 kRad TID [8]. Furthermore, a set of radiation protection methods are implemented [7, Sec. 2.6]. The manufacturer of the battery cells, Nanoavionics, has informed us that they conduct a range of in-house certification tests to assess the quality of every cell. These acceptance tests include: Vacuum testing, full charge discharge cycle testing for capacity measurement, and impedance measurements. Also, qualification campaigns are performed on the battery packs, for TVAC and vibration (up to 14 Grms, according to the NASA GEVS 7000 standard). However, more details on the tests will become available to the team after the purchase of the batteries. The presence or absence of further lot qualification procedures is currently not known and will be included as soon as it becomes available. Lastly, Nanoavionics does not provide an ISS certification or qualification as we have already discarded the ISS orbit scenario


---

#### Questions

Oscar setup correctness

