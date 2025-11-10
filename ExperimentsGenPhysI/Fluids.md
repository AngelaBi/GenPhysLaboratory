(fluid-physics-arch-bern-lab-overall)=
# Fluid Physics with Archimedes' & Bernoulli's Principles

## Background 

```{admonition} OVERALL GOALS
:class: note
Conduct two experiments to investigate:
- Buoyancy Force using:
  - Archimedes' Principle
  - Direct force measurements
- Bernoulli's Principle using:
  - Flow rate
  - Venturi tube's fluid pressure and velocity
```

Matter most commonly exists as a solid, liquid, or gas; these states are known as the three common phases of matter. We will investigate liquids in today's experiments. While solids are rigid with specific shapes and definite volumes where molecules are locked in position with their neighbors, liquids and gases are considered to be fluids because they are *not rigid* where the molecules are not locked in place and can therefore flow (i.e. move with respect to each other).

In today's experiments, we seek to understand why objects float or sink in a liquid (water) using Archimedes Principle regarding fluid statics as well as how liquid flows using Bernoulli's Principle regarding fluid dynamics.

### Archimedes' Principle

Archimedes' Principle states: "When an object is submerged in a fluid, the fluid exerts an upwards buoyant force equal to the weight of the fluid displaced by the object."

As depth increases, pressure in a fluid increases. Therefore, for an object in a fluid, the upward force on the bottom of that object is greater than the downward force on top of that object (see pressure forces $F_{\text{down}}$ vs $F_{\text{up}}$ in {numref}`M08_fluids_Fig00` *left*). There is a net upward force, or **buoyant force**, on any object in any fluid. If the buoyant force is greater than the object's weight, the object will rise to the surface and float. If the buoyant force is less than the object's weight, the object will sink (depicted in {numref}`M08_fluids_Fig00` *right-a* with $F_\text{Buoyancy} < w_\text{object}$). If the buoyant force equals the object's weight, the object will remain suspended at that depth. As such, there is always a buoyant force acting on an object regardless of whether it floats, sinks, or remains suspended.

```{figure} FluidsFigures/M08_fig00_2.jpg
:name: M08_fluids_Fig00
:width: 530px
:align: center

**LEFT**) Pressure due to the weight of a fluid increases with depth causing a greater upward force on the bottom of the object than the smaller downward force on the top of the object. ($F_{\text{down}} < F_{\text{up}}$ and horizontal forces cancel.) **RIGHT-a**) An object submerged in a fluid experiences a buoyant force $F_\text{B}$. If $F_\text{B}$ is greater than the weight of the object $w_\text{obj}$, the object will rise. If $F_\text{B} < w_\text{obj}$ as depicted in **a**, the object will sink. **RIGHT-b**) If the object is removed, it is replaced by fluid having weight $w_\text{fl}$. Since this weight is supported by surrounding fluid, the buoyant force must equal the weight of the fluid displaced. That is, $F_\text{B} = w_\text{fl}$, a statement of Archimedes' principle.
```

How could we determine the buoyancy force $F_\text{B}$ acting on the object within the fluid? It helps to describe this by removing the object (as in {numref}`M08_fluids_Fig00` *right-b*). The volume of the space left behind is filled in by fluid having a weight $w_\text{fl}$. Since that fluid is supported by the surrounding fluid, that weight of the fluid $w_\text{fl}$ (originally displaced by the object) is equal to the buoyancy force $F_\text{B}$. This is **Archimedes' Principle** --- The buoyant force on an object equals the weight of the fluid it displaces: 

```{math}
:label: M08_fluids_Eq01
F_\text{B} = w_\text{fl}
```

**First experiment (Archimedes)**

In this experiment, we will first determine the mass, volume, and density of 6 objects (see {numref}`M08_fluids_Fig02`). We will then determine the buoyant force acting on each object using Archimedes' Principle by determining the weight of water each object displaces. Finally, we will determine the buoyant force by measuring the apparent weight of an object.

```{figure} FluidsFigures/M08_fig02_v2025-01.png
:name: M08_fluids_Fig02
:width: 290px
:align: center

3 cylinders, 2 blocks, 1 irregular.
```

As a reminder, the density $\rho$ of an object depends on its mass $m$ and volume $V$:

```{math}
:label: M08_fluids_Eq02
\rho = \frac{m}{V}
```

and the weight of an object is the downward force due to gravity:

```{math}
:label: M08_fluids_Eq03
w_\text{obj} = mg
```

```{figure} FluidsFigures/M08_fig06_v2025-01.png
:name: M08_fluids_Fig04
:width: 80%
:align: center

Left) Force diagram. Apparent weight in water is the difference of weight in air and buoyant force. Right) Force sensor measuring apparent weight of object in water.
```

When an object is submerged in a fluid, the apparent weight of the object is less than the weight in air because of the upward buoyant force (see {numref}`M08_fluids_Fig04`). Thus, the buoyant force can be calculated by finding the difference between the weight of the object in air and the apparent weight of the object when it is submerged in water.

```{math}
:label: M08_fluids_Eq04
F_\text{B} = w_\text{obj in air} - w_\text{obj in water}
```

### Bernoulli's Principle

Imagine fluid flowing through a channel of varying width (ex. of such a setup in {numref}`M08_fluids_Fig07`). As the cross-sectional area changes, the volumetric flow rate remains constant, but the velocity and pressure of the fluid vary.

```{figure} FluidsFigures/M08_fig07.jpg
:name: M08_fluids_Fig07
:width: 390px
:align: center

Example of a Venturi tube, where velocity $v_1 < v_2$, pressure $P_1 > P_2$, and cross-sectional area $A_1 > A_2$
```

An incompressible fluid of density $\rho$ flows through a pipe of varying diameter. As the cross-sectional area decreases from $A_1$ (large) to $A_2$ (small), the speed of the fluid increases from $v_1$ to $v_2$. The flow rate, $R = \text{volume}/\text{time}$, of the fluid through the tube is related to the speed of the fluid ($v = \text{distance}/\text{time}$) and the cross-sectional area of the pipe $A$. The flow rate must be constant over the length of the pipe as everything that goes in one side comes out the other end. This relationship is known as the **Continuity Equation** which can be expressed as:

```{math}
:label: M08_fluids_Eq05
R = A_1 v_1 = A_2 v_2
```

As the fluid travels from the wide part of the pipe to the constriction, the speed increases from $v_1$ to $v_2$, and the pressure decreases from $P_1$ to $P_2$. This drop in fluid pressure due to fluid speeding up as it flows through a constricted section of a pipe is known as the **Venturi effect**. This effect can be created with the use of a Venturi tube which allows an incompressible fluid to flow from a wider to narrower section with minimal turbulence.

Assuming the path an incompressible fluid takes is frictionless with no viscous forces, then the energy of the fluid is conserved. The fluid can be analyzed by the total work done on the fluid from the initial position to final position within the tube (total change in both kinetic and potential energy). The full derivation is in your lecture textbook, but for now, we arrive at **Bernoulli's Equation**. For an **incompressible, frictionless fluid**, the combination of pressure and the sum of kinetic and potential energy densities is *constant* not only over time, but also along a streamline:

```{math}
:label: M08_fluids_Eq06
P + \frac{1}{2}\rho v^2 + \rho g y = \text{constant}
```

Note the similarities in {eq}`M08_fluids_Eq06` to our previous labs' equations for kinetic and potential energies ($\frac{1}{2}m v^2$ & $m g h$). Applying this to our Venturi tube of {numref}`M08_fluids_Fig07`:

```{math}
:label: M08_fluids_Eq07
P_1 + \frac{1}{2}\rho v_{1}^2 + \rho g y_1 = P_2 + \frac{1}{2}\rho v_{2}^2 + \rho g y_2
```

However, since our tube will be horizontal, we can remove the height dependence and our pressure change is due only to the velocity change (noted by the Continuity Equation in {eq}`M08_fluids_Eq05`). Thus, our equation simplifies to **Bernoulli's Principle** of fluid flow at a **constant height**:

```{math}
:label: M08_fluids_Eq08
P_1 + \frac{1}{2}\rho v_{1}^2 = P_2 + \frac{1}{2}\rho v_{2}^2
```

Rearranged another way to determine the pressure at the constriction:

```{math}
:label: M08_fluids_Eq09
P_2 = P_1 - \frac{1}{2}\rho (v_{2}^2 - v_{1}^2)
```

**Second experiment (Bernoulli)**

In our experiment, we will assume we don't know the pressure at the constriction $P_2$, and will use the Continuity and Bernoulli equations to determine theoretically what $P_2\text{ theoretical}$ should be and compare to the actual value $P_2\text{ actual}$ as measure by our pressure sensor.

The setup will be as in {numref}`M08_fluids_Fig08`. Water can be released from the pitcher sitting on the white/plexiglass box with the cooler-style spout as the release valve. On the other end of the water hose will be a hose clamp for use during the determination of the flow-rate to rapidly stop the flow of water (if you only used the spout at the pitcher, much of the water would continue flowing out of the tube even after shutting if off, messing up the flow-rate calculations).

$P_1$, as measured by the Quad Pressure Sensor, will be treated as a known actual or accepted value to be used in our calculations to solve for $P_{2\text{ theoretical}}$. It will be connected to port 1 (or port 3 if in the future these sensors break).

We will calculate $P_{2\text{ theoretical}}$ from our Continuity and Bernoulli equations. The value of $P_{2\text{, actual}}$, as measured by the Quad Pressure Sensor, will be treated as the known actual value to compare to. $P_2$ will be connected to port 2 (or port 4 if sensor is damaged).

NOTE: The pressure sensor hoses are to have only (or mostly) air such that water does not reach the pressure sensor. To avoid water getting up the air hoses, ensure the Venturi tube is positioned with the air hoses pointed upward. After passing through the Venturi tube, the water will flow into a catch basin. There will also be a stopwatch to measure flow-rate during the first part of the experiment.

If you require more water in your pitcher, use another pitcher to refill (assuming the catch basin is glass, there will be less of a chance of that breaking if we're not moving it around more than we have to).

```{figure} FluidsFigures/M08_fig08_v2025-01.png
:name: M08_fluids_Fig08
:width: 90%
:align: center

Sketch of the Venturi tube setup for the second experiment (Bernoulli).
```



## Experimental Procedure

### Archimedes' Principle (First experiment)

```{admonition} OVERVIEW
:class: note
- Understand the relationship between buoyancy force and the mass, volume, density of an object by doing:
  - Part I: Determine mass, volume, density of different objects.
  - Part II: Determine buoyant force using Archimedes' Principle.
  - Part III: Determine buoyant force by measuring the upward force directly.
```

#### Part I: Mass, Volume, and Density

1. Create a data table with:
   - Columns for the mass $m$, relevant dimensions (length, width, height, radius), volume $V$, and density $\rho$
   - Rows for each of the 6 objects (clearly label or describe the objects in the table).

2. Normally, you would measure the volume and mass of each object ({numref}`M08_fluids_Fig02`) with Vernier calipers and a triple-beam balance, however, to save time during lab, the volume and mass of each object is presented here:

    ```{table} Object Volume and Mass
    :name: tab-fluids-lab-object-volume-mass
    | Object | Volume (cm$^3$) ± 0.1 | Mass (g) ± 0.2 |
    |------------------------------|----------------|----------------|
    | Plastic Cylinder             | 24.7           | 22.4           |
    | Aluminum Cylinder            | 24.7           | 66.7           |
    | Brass Cylinder               | 24.7           | 207.7          |
    | Aluminum Block               | 24.7           | 66.7           |
    | Aluminum Irregular (hole)    | 24.7           | 66.7           |
    | Brass Block                  | 7.87           | 66.7           |
    ```

<!---
2. Using the triple-beam balance, find the mass of each of the six objects. List the objects in order from least to greatest mass. *Consider: are any of the masses nearly the same?*

3. Using the calipers, measure the dimensions of the 3 cylinders and the 2 blocks ({numref}`M08_fluids_Fig03`). Remember to divide the diameter by 2 to get the radius, $r$. Calculate the volume $V$ of these objects $V_\text{cylinder} = \pi r^2 h$ and $V_\text{block} = lwh$

4. There is no simple formula for the volume of the irregularly shaped object, so it is necessary to find the volume by measuring the volume of water it displaces:
   - Put the beaker under the overflow can spout as shown in {numref}`M08_fluids_Fig03`.
   - Pour water into the overflow can until it overflows into the beaker. Allow the water to stop overflowing on its own and empty the beaker into your pitcher and return it to its position under the overflow can spout without jarring the overflow can.
   - Tie a string on the irregular object.
   - Gently lower the irregular object into the overflow can until it is completely submerged. Allow the water to stop overflowing and then pour the water from the beaker into the graduated cylinder. Measure the volume of water that was displaced by reading the water level in the graduated cylinder in milliliters (1 ml = 1 cm³)

```{figure} FluidsFigures/M08_fig03.jpg
:name: M08_fluids_Fig03
:width: 80%
:align: center

Left) Measuring with calipers. Right) Lowering object into overflow can.
```


--->

3. List the 6 objects in order from least to greatest volume. *Consider: Is this the same order as the mass list? Are any of the volumes nearly the same?*

4. Calculate the density of each object. List the 6 objects in order from least to greatest density. *Consider: Is this list in the same order as either the mass list or the volume list? Do any of the objects have densities that are nearly the same?*

5. Group the objects according to the type of material of which they are made. *Consider: In which list (mass, volume, or density) are the objects grouped similarly?*

#### Part II: Finding the Buoyant Force Using Archimedes' Principle

For each of the objects, find the weight of the water displaced by each one:

6. Create a data table with:
   - Mass of beaker and other common data
   - Columns for the mass $m_\text{water} = m_\text{total} - m_\text{beaker}$, weight $w_\text{water} = m_\text{water} g = F_\text{B}$
   - Rows for each of the 6 objects plus a half-submerged brass cylinder (so 7 rows). Clearly label or describe the objects in the table.

7. Find the mass of the beaker. Put the beaker under the overflow can spout as shown in {numref}`M08_fluids_Fig03`.
8. Pour water into the overflow can until it overflows into the beaker. Allow the water to stop overflowing on its own and empty the beaker into the pitcher and return it to its position under the overflow can spout without jarring the overflow can.
9. If not already attached, tie a string onto each of the objects.
10. Gently lower the first object into the overflow can until it is completely submerged. Allow the water to stop overflowing. Find the mass of the water plus beaker. Subtract the mass of the beaker to determine the mass of the displaced water. Multiply the mass by the acceleration due to gravity (9.803 m/s²) to find the weight of the water.
11. Repeat this procedure for the other objects. Note that the plastic cylinder will float so don’t try to completely submerge it in the water. Also find the weight of the displaced water when only half the brass cylinder is submerged.
12. List the objects in order from least buoyant force to greatest buoyant force.

    ```{admonition} Discussion Point: Bouyancy vs. Object
    :class: question
    Is this in the same order as the mass list, the volume list, or the density list? Are any of the buoyant forces nearly the same? Why or why not?
    ```

#### Part III: Finding the Buoyant Force by Finding the Upward Force

13. Create a data table:
    - Seven rows for each of the 6 objects as well as the brass cylinder half-submerged (clearly label or describe the objects in the table).
    - Columns for weight in air $w_\text{obj in air}$, apparent weight in water $w_\text{obj in water}$, buoyant force $F_\text{B}$ as determined with {eq}`M08_fluids_Eq04`.

14. Ensure there is a loop of string attached to each object so they can be hooked onto the force sensor.

15. In Capstone, press record or monitor, and you will see the force in Newtons displayed (constantly updating). You can let this continue running to act as a continuous scale.

16. Before hanging any of the objects on the force sensor hook, zero the force sensor with the physical "zero" button on the front of the force sensor (shown in {numref}`M08_fluids_Fig04`).

17. With the water out of the way, record the weight of each object in air $w_\text{air}$ by hanging them on the hook.

18. Zero the sensor as needed if it appears to be drifting when swapping out the different objects.

19. Now place the pitcher of water beneath the force sensor such that when you hang each object from the force sensor hook, the objects can be fully submerged. Record the apparent weight of each object in water $w_\text{water}$.

20. Calculate the buoyant force for each object by taking the difference between the weight in air and the weight in water ({eq}`M08_fluids_Eq04`).

21. Add an additional column and calculate for each object case the % difference between the buoyancy force (found here by measuring the upward force) and the buoyancy force found previously by Archimedes' Principle of the displaced water.

```{math}
\% \text{ diff.} = \frac{F_\text{B, upward force method} - F_\text{B, Archimedes' method}}{F_\text{B, Archimedes' method}} \times 100
```

  ```{admonition} Discussion Point: Archimedes' vs. Force Sensor
  :class: question
  For each object case, is the buoyant force that was determined using the upward force equal to the weight of the water displaced?
  ```

### Bernoulli's Principle (Second experiment)

```{admonition} OVERVIEW
:class: note
- Understand fluid-flow continuity through different constrictions by:
  - Part I: Determine flow-rate of our system using the Continuity Equation.
- Understand Bernoulli's Principle of fluid flow at a constant height by:
  - Investigating the Venturi effect.
  - Determining the pressure of a fluid at a constriction point (in a Venturi tube).
```

#### Part I: Determining Flow Rate $R$

1. Create a data table:
   - 6 rows for five trials of the measuring flow rate as well as the average flow rate $R_\text{avg}$ and standard deviation of your flow rate $\sigma_R$.
   - Columns for the volume $\Delta V$ of water, elapsed time $\Delta t$ it took to flow, and flow rate $R$.

2. With water in the pitcher, open the release valve (spout) to allow water to flow and remove all air bubbles within the tubing to achieve laminar flow. After a few seconds, close the bottom releave valve (after the venturi tube) at the end of the tube to halt the flow. Take whatever water is in the catch basin and return it to the pitcher.

3. Start current trial with the catch basin empty.

4. Start the stopwatch and open the bottom releave valve at the same time to start water flow.

5. After a measurable amount of water has flowed through, stop the stopwatch and close the bottom releave valve at the same time.

6. Measure the volume of water that flowed out of (or into) the apparatus (either with the scale on the catch basin or graduated cylinder).

8. Calculate the average flow rate for the current trial $R = \frac{\Delta V}{\Delta t}$ where $\Delta V$ is the volume of water and $\Delta t$ is the elapsed time.

9. Empty the catch basin or graduated cylinder back into the pitcher to keep a consistent amount of water in it.

10. Rerun this process starting with the empty catch basin (assuming the water hose is still clear of air bubbles) 4 more times for a total of 5 trials.

11. From the individual trial flow rates, calculate the average flow rate $R_\text{avg}$ and standard deviation $\sigma_R$ which we will use to represent our uncertainty in the flow rate ($R_\text{avg} \pm \sigma_R$).

12. NOTE: Typically the flow rate varies with the level of water in the reservoir. To keep the flow rate close to constant, make the pressure measurements with the water level approximately the same as it was for the flow rate measurement.



#### Part II: Determining Pressure at a Constriction (with Continuity and Bernoulli Equations)

13. Create a data table:
    - Common data section including:
      - Flow rate $R_\text{avg} \pm \sigma_R$ from Part I.
      - Cross-sectional areas $A_1$ and $A_2$ and their uncertainties $\delta_{A_1}$ and $\delta_{A_2}$.
      - Velocities $v_1$ and $v_2$. Also include the max values for each (Used to estimate pressure uncertainty later).
      - Density of water $\rho$ (use 1000 kg/m³)
    - 7 rows for five trials of the measuring $P_1$ and $P_2$ in Capstone as well as their averages $P_{1\text{ avg actual}}$ and $P_{2\text{ avg actual}}$ and standard deviations $\sigma_{P_{1\text{ avg actual}}}$ and $\sigma_{P_{2\text{ avg actual}}}$.
    - Columns for $P_1$ and $P_2$.

14. Determine the cross-sectional areas of the wide and narrow constrictions ($A_1$ and $A_2$ respectively) with the calipers from the cutaway version of the Venturi tubes ($A = \pi r^2$). Note your uncertainty due to your measurement precision ($\delta_{A_1}$ and $\delta_{A_2}$).

15. Calculate $v_1$ and $v_2$ with the Continuity {eq}`M08_fluids_Eq05` based on your measured areas and average flow rate. Similarly, calculate $v_{1\text{ max}}$ and $v_{2\text{ max}}$ by maximizing the flow rate ($R_\text{avg} + \sigma_R$) and minimizing the areas (e.g. $A_1 - \delta_{A_1}$).

16. Capstone will be set up to show two pressures representing $P_1$ and $P_2$. Double check the the pressure taps of the Venturi tube are appropriately connected like in {numref}`M08_fluids_Fig08` where Channel 1 is connected to the wider part of the Venturi tube, and Channel 2 to the narrow constriction of the Venturi tube. (It'll be easier to keep track of which pressure is which when the labels are similar.)

17. Capstone will also show a plot with both $P_1$ and $P_2$ on the y-axis as a function of time on the x-axis. To analyze either data set later on, you can click directly on the plotted data.

18. Calibrate the pressure sensor by:
    - Ensure both the top release valve and bottom releave valve are closed.
    - Disconnect the air hoses from the Quad Pressure Sensor via the quick connectors so the pressure sensors are open to atmospheric pressure. Set the air hoses on top of the white box (or in a bracket to hold them if I get them prepared in time) so the end of the hose is above the spout water level to prevent water from siphoning through the air hoses.
    - In Capstone, select the green Calibration tab on the left-hand panel.
    - 1) Pressure 2) Select all "Pressure Measurements" 3) Type of Calibration as "One Standard (1 point offset)" 4) Set Standard Value to average atmospheric pressure of 101.3 kPa --- Click the "Set Current Value to Standard Value" button 5) Finish
    - Both Absolute Pressure Channels 1 and 2, when you press record, should now read at about 101.3 kPa, if not, retry the calibration.

19. Ensure no water is near the end of the air hoses to prevent any water getting into the pressure sensors. Reconnect the air hoses to the pressure sensors.

20. You can open the hose clamp at the end of the hose as it will not be needed for the rest of this experiment. You will just need to catch basin to collect the water and avoid making a mess.

21. Press record, then open the release valve to allow the water to flow into the catch basin. After any air bubbles have passed and the water is flowing with minimal turbulence, continue recording pressure data for ~5 seconds, then close the release valve (spout) and stop recording.

22. Find the section of your Pressure vs. Time plot where flow was laminar (smooth without bubbles), should be a generally flat section of the Pressure vs Time plot. Click on the $P_1$ data on the plot, enable the highlight tool, and select a chunk of the plot when flow was laminar (no bubbles, the flat part). Do the same for the $P_2$ data. You can find the average value for $P_1$ and $P_2$ at the bottom of the table on the left hand side of your screen, where the mean is representing the average value of whichever subset of the data you've highlighted.

23. Record both $P_{1\text{ actual}}$ and $P_{2\text{ actual}}$. There should be a difference of ~2--5 kPa, if not, double check with an instructor.

24. Rerun this process from Step 21 an additional 4 times for a total of 5 trials.

25. Determine the $P_{1\text{ avg actual}}$ and $P_{2\text{ avg actual}}$ values from your five trials. Also determine their standard deviations $\sigma_{P_{1\text{ avg actual}}}$ and $\sigma_{P_{2\text{ avg actual}}}$.

26. Calculate your theoretical value of $P_{2\text{ theoretical}}$ with {eq}`M08_fluids_Eq08` using your previously determined velocities $v_1$ and $v_2$ and your average $P_{1\text{ avg actual}}$ treated as the known actual value for the wider part of the Venturi tube.

27. Similarly calculate your max theoretical value of $P_{2\text{, max theoretical}}$ by maximizing ${P_{1\text{ avg actual}}}$ (e.g. ${P_{1\text{ avg actual}}} + \sigma_{P_{1\text{ avg actual}}}$) and using your already determined maximized velocities $v_{1\text{ max}}$ and $v_{2\text{ max}}$.

28. Represent your uncertainty $\delta P_{2\text{ theoretical}}$ with the difference of your maximized value and average values (e.g. $\delta P_{2\text{ theoretical}} = P_{2\text{, max theoretical}} - P_{2\text{ theoretical}}$).

29. *Consider:* Does you theoretical value for $P_2$ agree with the actual value of $P_2$ as measured with the pressure sensor?



















## Post-Lab Submission --- Interpretation of Results

<!--- ### Archimedes' Principle (Post-Lab Questions) --->
<!---
- Make sure to submit your finalized data table (Excel sheet)

- First Experiment (Archimedes' Principle)
  - In which list (mass, volume, or density) are the objects grouped similarly?
  - In each object case, is the buoyant force that was determined using the upward force (Part III) equal to the weight of the water displaced (Part II)? Were the % differences between the two methods for each case relatively small, or did any case standout?
  - Which objects had the same buoyant force when submerged? Why?
  - For the plastic cylinder, what was the apparent weight in water? What would be the buoyant force be if plastic cylinder were completely submerged?
  - How did the buoyant force for the totally submerged brass cylinder relate to the buoyant force for the half-submerged brass cylinder?
  - What does the buoyant force depend on: The mass of the object, or its volume, or its density, or the material from which it is made?

- Second Experiment (Bernoulli's Principle)
  - Does you theoretical value for $P_2$ agree with the actual value of $P_2$ as measured with the pressure sensor? (i.e. $P_{2\text{ theoretical}} \pm \delta P_{2\text{ theoretical}}$ overlap with $P_{2\text{ avg actual}} \pm \sigma P_{2\text{ avg actual}}$?)
  - How is the Bernoulli Principle different than the Bernoulli Equation?
  - What assumptions about the fluid allows the Bernoulli Principle to work? (i.e. what type or characteristics of the fluid and/or flow are necessary assumptions for Bernoulli to hold true?)
  - Imagine that instead of being on the table, the Venturi tube were set on the floor with the rest of the experimental apparatus unchanged. Would the difference in pressures we see on the Capstone plot between $P_1$ and $P_2$ during the smooth, laminar flow section that we analyzed to find average pressures be *larger*, *smaller*, or *the same*. Why?
  --->


  ### Finalized Spreadsheets
  - Make sure to submit your finalized data table (Excel sheet).
    - Please include relevant screenshots of your Capstone plots including:
      - 1 plot of $P_1$ and $P_2$ vs. Time (just 1 trial)



### Archimedes' Principle --- Post-Lab Error & Results Analysis
  - In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
    - Where might errors arise in measuring the buoyant force?
    - What are your measurement uncertainties for each experiment?
    - What are possible systematic uncertainties for each experiment?
    - How do these uncertainties affect your final results for $F_\text{B}$?
  - In a **paragraph**, summarize the results you have determined in each case. Consider:
	  - In which list (mass, volume, or density) are the objects grouped similarly?
	  - In each object case, is the buoyant force that was determined using the upward force (Part III) equal to the weight of the water displaced (Part II)? Were the % differences between the two methods for each case relatively small, or did any case standout?
	  - Which objects had the same buoyant force when submerged? Why?
	  - For the plastic cylinder, what was the apparent weight in water? What would be the buoyant force be if plastic cylinder were completely submerged?
	  - How did the buoyant force for the totally submerged brass cylinder relate to the buoyant force for the half-submerged brass cylinder?
	  - What does the buoyant force depend on: The mass of the object, or its volume, or its density, or the material from which it is made?


### Bernoulli's Principle --- Post-Lab Error & Results Analysis
  - In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
    - Where might errors arise in measuring the flow rate?
    - What are your measurement uncertainties for each experiment?
    - What are possible systematic uncertainties for each experiment?
    - What errors might cause your $P_{2 \text{ theoretical}}$ to diverge from $P_{2\text{ avg actual}}$? 
  - In a **paragraph**, summarize the results you have determined in each case. Consider:
	  - Does your theoretical value for $P_2$ agree with the actual value of $P_2$ as measured with the pressure sensor? (i.e. $P_{2\text{ theoretical}} \pm \delta P_{2\text{ theoretical}}$ overlap with $P_{2\text{ avg actual}} \pm \sigma P_{2\text{ avg actual}}$?)
	  - How is the Bernoulli Principle different than the Bernoulli Equation?
	  - What assumptions about the fluid allows the Bernoulli Principle to work? (i.e. what type or characteristics of the fluid and/or flow are necessary assumptions for Bernoulli to hold true?)
	  - Imagine that instead of being on the table, the Venturi tube were set on the floor with the rest of the experimental apparatus unchanged. Would the difference in pressures we see on the Capstone plot between $P_1$ and $P_2$ during the smooth, laminar flow section that we analyzed to find average pressures be *larger*, *smaller*, or *the same*. Why?


## The Whiteboard

```{figure} FluidsFigures/FluidPhysics_2024_Fall_01.jpg
:name: flu1
:width: 600px
:align: center

```

```{figure} FluidsFigures/FluidPhysics_2025_Summer_01.jpg
:name: flu2
:width: 600px
:align: center

```

```{figure} FluidsFigures/FluidPhysics_2025_Summer_02.jpg
:name: flu3
:width: 600px
:align: center

```