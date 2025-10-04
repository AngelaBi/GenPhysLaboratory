(ideal-gas-absolute-zero-lab-overall)=
# Ideal Gas Law with Isothermal & Adiabatic Compression; Estimating Absolute Zero

## Background

A general and complete description of an ensemble of many atoms or molecules is a very difficult, if not impossible task, given the large number of objects involved. Luckily enough most gases follow a relatively simple approximation for a rather large range of conditions.

The ideal gas law describes the behavior of a gas of point-like particles. While there is no such thing as an ideal gas (all real molecules have a small but non-zero size), it is nevertheless a good approximation to the behaviour of gasses at ordinary temperatures and pressures.

### Ideal Gas Law

The Ideal Gas Law assumes that

- The gas is made up of molecules moving in straight lines, but random directions,
- All collisions between the molecules themselves and between the molecules and the walls of the container are perfectly elastic,
- The temperature of the gas is directly proportional to the kinetic energy of the molecules,
- The pressure of the gas is due to the collisions of the molecules with the walls of the container,
- All inter-molecular forces can be neglected, and
- The volume occupied by the molecules is negligible as compared to the volume of the container.

Under these conditions the pressure, temperature, and volume of the gas will follow a simple relationship,

```{math}
:label: eq-idealgas
P V = n R T
```

where $P$ is the gas pressure in Pascals (1 Pa = 1 N/m²), $T$ is the gas temperature in Kelvin, $V$ is the volume (in m³), and $n$ is the number of moles in the gas (1 mole = 6.022×10²³ molecules). $R$ is called the universal gas constant and for these units has the value $R = 8.3145$ J/(mol·K).

Most gases will behave approximately as an ideal gas within a certain range of conditions across a number of different types of processes, but the law fails at low temperatures or higher pressures when forces between the gas molecules become important.

For today's lab, the two processes we will focus on are
 - **Isothermal**: temperature is kept constant through the process (e.g. a process analyzed when initial temperatures are the same as the final temperatures). This is possible when the ratio ${PV}$ is kept constant.
 - **Adiabatic**: energy of the system is kept constant (i.e. the parcel of gas does not exchange or lose energy to its surroundings). This is possible when the ratio $\frac{PV}{T}$ is kept constant.

### Absolute Zero

One of the things the ideal gas law assumes is that the kinetic energy of the gas molecules is directly proportional to the temperature of the gas. Therefore, if the molecules have no kinetic energy (the molecules are at rest) then the temperature of the gas is at its lowest possible value. This temperature is called absolute zero and is used as the zero-point of the Kelvin temperature scale

$$0\,\text{K} = -273.15\,°\text{C}.$$

Note that, according to the definition of pressure, gas molecules at absolute zero will also exert no pressure on the walls of the container the gas is in.

## Experimental Procedure

This experiment uses temperature and pressure sensors plugged into an interface so that data for both variables can be recorded simultaneously.
For the Ideal Gas Law experiment the air inside a syringe is compressed by pushing on the plunger. Pressure and temperature values are collected and recorded with the Capstone program, which is then also used to analyze the data.
For the Absolute Zero experiment a hollow sphere (with a fixed volume) is submerged in liquids of different temperature. Capstone will again collect and record pressure and temperature data of the gas enclosed in the sphere.
Pictures of the experimental setups are shown in {numref}`H01Fig01`, {numref}`H01Fig01b`,and {numref}`H01Fig02`.

```{figure} IdealGasFigures/Figure01a_v2025-01.png
:name: H01Fig01
:width: 50%
:align: center

The picture shows the Ideal Gas Law experimental apparatus. The two cables coming from the syringe are the temperature and pressure connectors. The plunger of the syringe has a mechanical stop to prevent full compression of the syringe. Note: be gentle with the pressure connector; you need to insert and gently twist to lock it in place. DO NOT FORCE IT.
```

```{figure} IdealGasFigures/Figure01b_v2025-01.png
:name: H01Fig01b
:width: 50%
:align: center

 The  picture shows the Absolute Zero experiment. The pressure and temperature connectors are shown exiting at the end of the black cable of the device. Note: be gentle with the pressure connector; you need to insert and gently twist to lock it in place. DO NOT FORCE IT.
```

```{figure} IdealGasFigures/Figure02_v2025-02.png
:name: H01Fig02
:width: 80%
:align: center

This picture shows the experimental methods for the Ideal Gas Law (left) and Absolute Zero (right) experiments. In both cases the temperature and pressure connectors are plugged into the PasPort Absolute Pressure/Temperature Sensor (the small blue box).
```

### The Ideal Gas Law Experiment

1. Create a Part 1 Data Table for your ideal gas law measurements and calculations.

2. Open graphs of absolute pressure ($y$-axis) vs. time ($x$-axis) and temperature in Kelvin ($y$-axis) vs. time ($x$-axis) in the **Capstone** program. Also have a table displaying absolute pressure and temperature open. All these can be opened by double-clicking on the corresponding items on the right-had side of the **Capstone** program.

3. Disconnect the quick-release pressure connector and push the plunger all the way down. Note that the mechanical stop will prevent the plunger from being pushed all the way to the bottom of the syringe. Record the volume reading on the syringe as the volume $V_{2}$ in your Part 1 Data Table. The value for $V_{2}$ should be about 20 cc.

4. Set the plunger for an initial volume of $V_{1} = 40$ cm³.

5. After you have adjusted the volume, re-connect the pressure port.

6. Hold the base of the syringe firmly against a sturdy, flat surface (the lab table).

7. Press the **Record** button on **Capstone**.

8. Press straight down as hard as you can on the plunger with the palm of your hand to fully compress the gas inside the syringe. Keep pressing to hold the pressure steady. Important: Do not let the pressure drop for at least 30 s. The mechanical stop will prevent you from decreasing the volume of the gas to less than than about 20 cc. Hold this position until the temperature and pressure have stabilized and are no longer changing (use the data table as an indicator). It should take less than 30 seconds for the temperature to return to room temperature.

9. Release the plunger and allow it to expand back out on its own (it may not go back to 40 cm³). Wait again until the temperature and pressure have equalized and are no longer changing.

10. Press the **Record** button again on **Capstone** to stop recording data.

#### Analysis with Constant Temperature

1. Highlight an area (click and drag with the mouse) on the pressure graph at the beginning of the data-collecting run, before you compressed the air in the syringe. The highlighted values of the selected data points will appear in the data table of **Capstone**. Record the initial pressure as $P_{1}$ in your Part 1 Data Table.

2. Highlight an area on the pressure graph at the point just before you released the plunger. Record the final pressure as $P_{2}$ in your Part 1 Data Table.

3. Calculate the ratio of initial volume over the final volume, $X_{1} = V_{1}/V_{2}$ and record the result in your Part 1 Data Table.

4. Calculate the ratio of final pressure over the initial pressure, $X_{2} = P_{2}/P_{1}$ and record the result in your Part 1 Data Table.

5. Compare the two ratios. According to the ideal gas law ({eq}`eq-idealgas`) the two values should be equal, since $P_{1} V_{1} = P_{2} V_{2}$ for constant temperature (note that the temperature is room temperature in both cases). Discuss, first amongst yourselves and then with your instructor, why the values are different.

#### Analysis with Varying Temperature

By now you have (hopefully) figured out that you have not accounted for the small amount of volume of air inside the tubing of the apparatus. Using the ideal gas law ({eq}`eq-idealgas`) and the data you collected in part 1 you can actually calculate this volume $V_{0}$ by solving the following equation for $V_{0}$

```{math}
:label: eq-volume-correction
\frac{(V_{1} + V_{0})}{(V_{2} + V_{0})} = \frac{P_{2}}{P_{1}}.
```

Using the data from your Part 1 Data Table calculate the value for $V_{0}$ and note the result in your Part 2 Data Table.

1. Highlight an area (click and drag with the mouse) on the temperature graph at the beginning of the data-collecting run, before you compressed the air in the syringe. The highlighted values of the selected data points will appear in the data table of **Capstone**. Record the initial pressure and the initial temperature as $P_{1}$ and $T_{1}$ in your Part 2 Data Table.

2. Note the initial volume $V_{1}^\prime = V_{1} + V_{0}$ in your Part 2 Data Table.

3. Highlight the area (click and drag with the mouse) on the temperature graph where the temperature peaks. The highlighted values of the selected data points will appear in the data table of **Capstone**. Note the peak temperature and the corresponding pressure at this instant as $P_{2}$ and $T_{2}$ in your Part 2 Data Table.

4. Note the volume $V_{2}^\prime = V_{2} + V_{0}$ in your Part 2 Data Table.

5. Calculate the ratio $Y_{1} = \frac{P_{1} V_{1}^\prime}{T_{1}}$ and record the result in your Part 2 Data Table.

6. Calculate the ratio $Y_{2} = \frac{P_{2} V_{2}^\prime}{T_{2}}$ and record the result in your Part 2 Data Table.

7. Assuming the most significant error is in the volume, compare the difference between the two ratios with your estimate of the uncertainty in the volume.

### Measurement of Absolute Zero

1. Connect the Absolute Zero apparatus to the PasPort sensor (both the temperature sensor and the quick-release pressure port need to be connected).

2. Close the **Capstone** Program and re-open it from the desktop.

3. Open a **Table & Graph** from the main canvas of **Capstone**. For the $x$-axis of the graph select absolute pressure and for the $y$-axis select temperature in °C. For the data table select the same two variables.

4. Now click on the **Continuous Mode** and select **Keep mode** from the pull-down menu that will appear. Click on the **Preview** button to start collecting data.

5. Run the hot water until steam rises from the sink. Fill a pitcher to the 2 quart mark.

6. First fully submerge the sphere in hot water: Observe the data points appearing on the graph. Make sure the sphere stays completely submerged the entire time you take data. Once the temperature has reached equilibrium (i.e. the value in the digital display no longer changes), press the **Keep Sample** button (N.B. Do **NOT** stop the data collection by clicking on the red square button again). Read and note the values for pressure and temperature (from the digital display) in your Part 3 Data Table.

7. Next remove half of the water in your container and replace it with cold water from the sink. Again fully submerge the sphere in the water and make sure the sphere stays completely submerged the entire time you take data. Note how the point moves in the Temperature vs. Pressure graph as the values change. Discuss the outcome among yourselves and with your instructor. Once the temperature is stable again (this will take a few minutes) press the **Keep Sample** button again. Read off and note the values for pressure and temperature (from the digital display) in your Part 3 Data Table.

8. Finally submerge the sphere in the cold water. Once again you need to make sure the sphere is completely submerged during the time you take data. Note how the point moves in the Temperature vs. Pressure graph as the values change. Discuss the outcome among yourselves and with your instructor. Once the temperature is stable again (this will take a few minutes) press the **Keep Sample** button again. Read off and note the values for pressure and temperature in your Part 3 Data Table.

9. Press the **Record** button once again on **Capstone** to stop recording data.

10. Using the fitting tool in **Capstone**, fit a straight line to the 3 data points you have taken.

11. The $y$-intercept of the best-fit line is the value for absolute zero temperature. Discuss among yourselves and with your instructor why this is the case. Note the result as $T_{0}$ in your Part 2 Data Table.

12. Compare your result to the accepted value of $-273.15$°C.

## Data Analysis

- Create a table for the analysis at constant temperature including the measured values $V_1, P_1, V_2, P_2$ and the calculated values $X_1, X_2$.
- Create a table for the analysis with varying temperature including $V_0, V_1, P_1, V_2, P_2$ and the calculated values $V^\prime_1, V^\prime_2, Y_1, Y_2$.
- Create a table for the measurement of absolute zero including the pressure and temperature you measured at the hot, warm and cool temperatures as well as the $y$-intercept and the accepted value of $-273.15$°C.

## Post-Lab Submission --- Interpretation of Results
<!---
- Make sure to submit your finalized data table (Excel sheet)
- Constant Temperature (Isothermal):
  - What properties of a system must be proportional if compression is isothermal?
  - How do the two ratios, $X_{1}$ and $X_{2}$, compare?
  - What may cause a discrepancy between the ratios of volumes and pressures?
- Varying Temperature (Adiabatic):
  - What properties of a system must be proportional if compression is adiabatic?
  - How do the two ratios, $Y_{1}$ and $Y_{2}$, compare?
  - What may cause a discrepancy between the ratios of volumes and pressures?
  - Consider the uncertainty as due to volume, do the ratios agree based on that uncertainty range?
- Absolute Zero:
  - What does absolute zero represent about a system?
  - What is your extrapolated result for absolute zero; how does it compare to the accepted value?
  - What measurement uncertainties exist; how do they affect your determined value for absolute zero?
- What are possible systematic errors for today's experiments?
--->
- Make sure to submit your finalized data table (Excel sheet). 
- In a **paragraph**, summarize the results you have determined in each case. Consider:
	- Constant Temperature (Isothermal):
	  - What properties of a system must be proportional if compression is isothermal?
	  - How do the two ratios, $X_{1}$ and $X_{2}$, compare?
	- Varying Temperature (Adiabatic):
	  - What properties of a system must be proportional if compression is adiabatic?
	  - How do the two ratios, $Y_{1}$ and $Y_{2}$, compare?
	- Absolute Zero:
	  - What does absolute zero represent about a system?
	  - What is your extrapolated result for absolute zero? How does it compare to the accepted value?
- In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
  - What are possible systematic errors for today's experiments?
  - Constant Temperature (Isothermal):
	  - What may cause a discrepancy between the ratios of volumes and pressures?
  - Varying Temperature (Adiabatic):
      - What may cause a discrepancy between the ratios of volumes and pressures?
      - Consider the uncertainty due to volume; do the ratios agree within that uncertainty range?
  - Absolute Zero:
	  - What measurement uncertainties exist? How do they affect your determined value for absolute zero?
	
	


## The Whiteboard

```{figure} IdealGasFigures/IdealGasLawAbsoluteZero_2024_Fall_01.jpg
:name: ide1
:width: 600px
:align: center

```
