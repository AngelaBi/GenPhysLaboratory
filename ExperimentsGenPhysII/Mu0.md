(magnetic-force-mu0-overall)=
# Magnetic Force & the Determination of $\mu_0$



## Background

```{danger}
⚠️ ⚠️ ⚠️ ⚠️ WARNING ⚠️ ⚠️ ⚠️ ⚠️

⚠️ ⚠️ ⚠️ ⚠️ HIGH CURRENT IN USE TODAY ⚠️ ⚠️ ⚠️ ⚠️

⚠️ ⚠️ ⚠️ ⚠️ DO NOT TOUCH THE METAL CONDUCTORS (BARS) or WIRE PLUGS ⚠️ ⚠️ ⚠️

⚠️ ⚠️ ⚠️ ⚠️ YOU CAN BE SERIOUSLY INJURED ⚠️ ⚠️ ⚠️ ⚠️

⚠️ ⚠️ ⚠️ ⚠️ WARNING ⚠️ ⚠️ ⚠️ ⚠️
```


### ● Background Overview

```{admonition} OVERALL GOALS
:class: note
Use a set of parallel bars to generate magnetic fields to:
- Investigate the relationship between magnetic force $F_B$ and current $I$ (i.e. $F_B$ vs. $I$).
- Experimentally determine the permeability of free space $\mu_0$
- Along with your previous plotting-derived measurements of $\varepsilon_0$, determine the speed of light $c$
```



By measuring the magnetic force between two parallel current-carrying conductors, the permeability of free space, $\mu_0$, will be experimentally determined. $\mu_0$ is a fundamental constant of nature, and, with its electric equivalent $\varepsilon_0$ that we determined in an earlier experiment, we will now be able to determine the magnitude of the velocity of propagation of an electromagnetic wave --- the speed of light. These constants are related to the speed of light, c, by the following relation, derived from Maxwell's equations which describe the behavior of electric and magnetic fields:

```{math}
:label: eq-speed-of-light
c=\sqrt{\frac{1}{\varepsilon_0\mu_0}}
```

You will measure $\mu_0$ here, and, with your previous measurement of $\varepsilon_0$, determine the speed of light $c$.

The 2019 redefinition of SI units defined exact values of fundamental constants including the electron charge $e$, the speed of light $c$, and Planck's constant $h$. The second is defined in terms of the frequency of a Cesium atomic clock. As a result, the value of $\mu_0$, the magnetic constant, must now be experimentally determined.

Note: Until 2019, $\mu_0$ was defined to be exactly $4\pi \times 10^{-7}$ T⋅m/A. This 2019 value is so close to the current best measurement, that you can use $\mu_0=4\pi \times 10^{-7}$ T⋅m/A as the *accepted value*. 



The magnetic field strength $B$ a distance $r$ from the center of a very long, straight conductor carrying a current $I$ is given by:

```{math}
:label: eq-magnetic-field
B=\frac{\mu_0 I}{2\pi r}
```

A conductor of length $L$ [m] carrying a current $I$ [A] in a magnetic field of strength $B$ [T] experiences a force $F_B$ [N], given by:

```{math}
:label: eq-magnetic-force
\vec{F_B}=I \vec{L} \times \vec{B} =I L B \sin{\theta}
```

where $\theta$ is the angle between the vectors $\vec{B}$ and $\vec{L}$. If the magnetic field is produced by the current in a second conductor, the currents in the two conductors exert equal magnitude and opposite forces on each other.

For the case of two long, parallel conductors, each carrying the same current $I$ and separated, center-to-center, by the distance $d_\text{center-to-center}$, the force between the two conductors is the force on one in the magnetic field of the second. Thus if {eq}`eq-magnetic-field` is used in {eq}`eq-magnetic-force`, we obtain for the force:

```{math}
:label: eq-parallel-conductor-force
\boxed{
F_B=\frac{\mu_0}{2\pi}\frac{L I^{2}}{d_\text{center-to-center}}
}
```

By measuring the force between two such conductors, the value of $\mu_0$ can be determined. By considering the parameters of the apparatus to be used, it can be seen that the magnitude of the force between the two conductors is quite small and will require some care to accurately measure. If $L$ is about 30 cm, $I$ about 10 A, and $d_\text{center-to-center}$ about 2 mm, the force would be in the range of $10^{-4}$ N, or the weight of a few milligrams of mass. Since this force is well below the weight of a reasonable conductor to be used for the experiment, a counter weighted balance system will be used to provide the mechanical support for the movable conductor. This is essentially the same apparatus as {ref}`Electric Force & ε₀ Lab <electric-force-and-epsilon-overall>`. The movable conductor can then be loaded by a known mass whose weight can then be matched by the small magnetic force. The apparatus is schematically illustrated from a top-down perspective in {numref}`fig-apparatus-diagram`.

```{figure} Mu0Figures/Figure01.jpg
:name: fig-apparatus-diagram
:width: 100%
:align: center

Apparatus dimensions from a top-down perspective, similar to the apparatus setup from {ref}`Electric Force & the Determination of ε₀ <electric-force-and-epsilon-overall>`.
```

As before, similar to the setup and measurement methods from the {ref}`Electric Force & ε₀ Lab <electric-force-and-epsilon-overall>`, an optical lever, telescope and scale are used to observe the deflection of the balance, which carries the movable, upper conductor. The magnitude of the magnetic force can be measured when the magnetic force has restored the loaded system to its original position. In this case we make the same magnitude current flow in opposite directions in the two conductors so the force between the two conductors is repulsive. Thus on the upper conductor, there is a gravitational force down (the weight of the added mass) and a magnetic force upward which we will adjust by controlling the current equal to the gravitational force. More conveniently than the electric force version of the balance beam, this equilibrium is stable!

With the required balancing current determined along with the other dimensions of the apparatus, we can now determine the value of $\mu_0$.


### ● Equipment

<!---
- Telescope with crosshair & centimeter-scale ruler on vertical pole
- AC power from wall outlet, controlled with large, cylindrical potentiometer. Controls range from 0 -- 100% of wall power (~0 -- 15 A). Ignore the scale on the dial since the knob is not actually lined up to them.
- Voltage transformer to drop AC voltage to ~6 V (small metal cube)
- Fluke multimeter -- in series, set to read AC current ($\tilde{\text{A}}$), red wire to 10 A, black wire to COM ports
- Small masses of 1 -- 500 mg, plastic tweezers
- Parallel-conductor apparatus
  - Bottom conductor held in static position
  - Top conductor that can swing up or down when changing amount of applied mass or current. Set up to be parallel to bottom conductor when empty (holding 0 mg).
  - Mirror to view the scale (ruler) via telescope to determine angle between plates
  - Beam lift knobs to reset top plate position
  - Leveling screws to level whole apparatus
- x4 Banana plug wires (12 AWG, x2 1', x2 3') connecting wall power from transformer to ammeter & parallel-conductor apparatus
- Protective box with the mirror-to-scale distance written on it

--->

```{table} Equipment
:name: parallel-conductor-equipment-table

| Category | Items |
|---|---|
| **Optical Measurement** | • Telescope with crosshair<br>• Centimeter-scale ruler mounted on vertical pole |
| **Power Supply** | • AC power from wall outlet controlled by large cylindrical transformer/potentiometer (0–100% of wall power, ~0–20 A) *Dial markings are not accurate; ignore scale on knob* <br>• Voltage transformer (small metal cube) reducing AC voltage to ~6 V |
| **Current Measurement** | • Fluke multimeter used as AC ammeter ($\tilde{\text{A}}$, ![alt text](../Intro/IntroductionFigures/FigExtra_034_ACCurrent_v01.png)), connected **in series** with circuit<br>• One lead in **10 A** port ![alt text](../Intro/IntroductionFigures/FigExtra_031_HighAmp_v01.png), other lead to **COM** port ![alt text](../Intro/IntroductionFigures/FigExtra_033_COM_v01.png) |
| **Masses & Tools** | • Small masses (5, 20, 50, 100, 200 mg)<br>• Plastic tweezers for handling masses |
| **Parallel-Conductor Apparatus** | • Bottom conductor fixed in place<br>• Top conductor free to swing vertically when current or mass changes<br>• Adjust so conductors are parallel when **0 mg** is applied<br>• Mirror used with telescope to read ruler and determine balance beam angle<br>• Beam lift knobs to reset top conductor position<br>• Leveling screws to level apparatus |
| **Electrical Connections** | • 4× banana plug wires (12 AWG)<br> • 2× 1 ft<br> • 2× 3 ft<br>• Connect transformer $\rightarrow$ ammeter $\rightarrow$ parallel-conductor apparatus |
| **Additional Equipment** | • Protective box with mirror-to-scale distance written on it |
```



### ● Adjustment of apparatus

The apparatus has been carefully adjusted before your lab and should not require further significant adjustments. This section describes how the apparatus was prepared. If something seems to need adjusting, see the lab instructor. The apparatus is very similar to the apparatus setup from {ref}`Electric Force & ε₀ Lab <electric-force-and-epsilon-overall>`.

1. The beam lift provides a definite location for the beam and thus guarantees continued alignment of the parallel conductors. Use the beam lift each time you change weights or relocate the counterweight.
2. The fixed conductor can be adjusted vertically, the movable conductor horizontally, so that the conductors are parallel. *If the conductors are NOT parallel with no mass in place, seek the instructor's help.*
3. The counterweight behind the mirror can be used to change the equilibrium separation of the conductors.
4. Level the apparatus with the adjusting screws so that it sits securely on the table.
5. Mirror-to-scale distance was measured from rear of mirror (reflective surface) to roughly the middle of $S_1$ and $S_0$ on the scale (ruler).



(demo-video-mu0-constant)=
## Demo Video: Setup & Procedure

Some clarifications, additions, or corrections since this video is slightly outdated:

- Wires are thicker and safer now, still don't touch, don't exceed 20 A
- White board slightly outdated as there have been slight changes
- Masses in **decreasing** order, rather than increasing order
- Using average and **uncertainty** (not standard deviation)
- Speed of light just from **plotting-derived** (i.e. from `LINEST`) values from first lab ($\varepsilon_0$) and today's lab ($\mu_0$)

<div style="text-align: center;">
  <iframe
    width="80%"
    height="315"
    src="https://www.youtube.com/embed/EpYTWOcaFSU"
    title="YouTube video"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
  <figcaption>Demonstration video. Reviews overall setup and procedure. *Yes audio*</figcaption>
</div>


If embedding is broken, follow: <a href="https://www.youtube.com/watch?v=EpYTWOcaFSU" target="_blank" rel="noopener noreferrer">
https://www.youtube.com/watch?v=EpYTWOcaFSU
</a>



## Experimental Procedure
### ● PRECAUTIONS

  - The wire frame that supports the current carrying conductor and counterweight is supported on knife edges. The frame is easily bent, and the knife edges can be easily damaged. Treat the system with the same care as a precise analytical balance. Handle the weights with tweezers and store them in the case.
  - The current must pass through the knife edges and intense local heating is produced. Reduce the current to zero as soon as possible after making the observations.

    ```{danger}
      - **DO NOT TOUCH THE METAL CONDUCTORS (BARS) or WIRE PLUGS**
      - **The current should not exceed 20 A!**
    ```



<!---
```{admonition} OVERVIEW
:class: note
- Understand the relationship between magnetic force and current using a consistent induced magnetic field, reasonably produced by high current through parallel, cylindrical conductors
- Conduct three rounds of nine trials each (total 27 trials) of applying more mass (more gravitational force) and more current to produce a magnetic field (and therefore more magnetic force). Do the rounds sequentially rather than all of a single applied mass in a row to ensure you catch and correct any significant errors early (e.g. if the apparatus is bumped out of alignment) rather than having to do all 27 trials again. The order of the trials for applied masses would be 0, 25, 50, 75, 100, 125, 150, 175, 200, 0, 25, 50, 75, 100, 125, 150, 175, 200, 0, 25, 50, 75, 100, 125, 150, 175, 200 mg
- In this experiment, first determine the separation distance, $d$. Then add mass with a series of increasing masses and apply the necessary current $I$ applied along the conductors so they return to parallel where the separation distance returns to $d$. Under this condition, the magnetic force required to maintain the separation $d$ will be the difference of the gravitational force on the applied mass. Then determine $\mu_0$ for each trial, and an overall value through both averaging of all your trials and plotting of all your data (i.e. magnetic force vs. current² between the conductors). Comparing then your results from both analysis methods to the accepted $\mu_{0\text{-accepted}}$. Ultimately determine the speed of light $c$.
```
--->

### ● Preview


   ```{admonition} PROCEDURE OVERVIEW
   :class: note
   - Investigate the relationship between magnetic force and current using the magnetic field induced by high current in parallel, cylindrical conductors.
   - Determine permeability of free space $\mu_0$
   - Determine speed of light $c$
   - Perform **three rounds of nine trials** each (27 trials total). In each round, sequentially apply less mass (below). Repeat this sequence three times (rather than completing all trials for a single mass) so that any alignment issues or experimental errors can be detected and corrected early without repeating the entire experiment.
     - First determine the conductor separation distance, $d_\text{center-to-center}$. Then add mass and adjust the current $I$ until the conductors return to parallel, restoring the separation to $d_\text{center-to-center}$ (or telescope crosshair to $S_0$). Under this condition, the magnetic force balances the additional gravitational force from the applied mass.
     - For each trial, determine $\mu_0 \pm \delta \mu_0$.
     - Obtain an overall value by both:
       - averaging the results from all trials
       - plotting magnetic force vs. $I^2$
         - include additional magnetic force vs. $I$ plot for comparisons
     - Compare these results with the accepted value $\mu_{0\text{,accepted}}$
     - Determine speed of light $c$ by using your plotting-derived value of $\mu_0 \pm \delta \mu_0$, and previous plotting-derived values of $\overline{\varepsilon_0} \pm \sigma \varepsilon_0$
   ```



### ● Preliminary Setup

If $b$ is the mirror-to-scale distance and $a$ is the length of the frame (see {numref}`fig-apparatus-diagram`), then a straightforward geometrical analysis (like in {ref}`Electric Force & ε₀ Lab <electric-force-and-epsilon-overall>`) will show that the vertical displacement of the conductor, $y$, is given by:

```{math}
:label: eq-vertical-displacement
y=\frac{D a}{2 b}
```

where $D$ is the change in scale reading from the equilibrium value and the value when the two conductors are in contact (the contact reading is determined by adding a mass to the pan which depresses the beam until contact occurs). The factor of 2 results from the fact that the optical path reflected off of the mirror to the scale rotates through an angle twice that of the beam holding the movable conductor.

However, the change in scale reading doesn't account for the conductors' **thickness**. Since the B-field generated by current flowing in the cylindrical conductors is organized about their center, we must add in two radii to get the center-center separation between the two conductors. This gives us:

```{math}
:label: eq-center-separation
\boxed{
d_\text{center-to-center}=\frac{D a}{2 b}+2r_\text{conductor}
}
```

where $r_\text{conductor}$ is the radius of the conductor (multiplied by two to deal with the fact that we're dealing with two conductors).

1. Investigate the use of the telescope and scale so that the rotation of the frame can be measured in terms of scale divisions (see {numref}`fig-measurement-apparatus`).

```{figure} Mu0Figures/E6_Figure02_v02.jpg
:name: fig-measurement-apparatus
:width: 100%
:align: center

Schematic of the measuring apparatus, similar to the setup and measurement methods from {ref}`Electric Force & ε₀ Lab <electric-force-and-epsilon-overall>`.
```

2. **Do not turn on the power supply until requested in the procedure later in {ref}`data-collection-mu0-section`.**

3. Create a common data table with:
    - $a$: length of frame, $0.215\,\text{m}$
    - $b$: mirror-to-scale distance (on top of protective box)
    - $L$: wire/bar length $0.265\,\text{m}$
    - $r_\text{conductor}$: wire radius $1.6\,\text{mm}$    
    - $S_0$: equilibrium crosshair position
    - $S_1$: bars touching crosshair position
    - $D$: ruler (a.k.a. scale) distance between $S_0$ and $S_1$
    - $d_\text{center-to-center}$: length of frame
    - $g$: acceleration due to gravity for Fairfield, CT, $9.803\,\text{m/s}^2$
    - $\mu_{0\text{,accepted}}$: accepted value of the permeability of free space, $4\pi \times 10^{-7}\,\text{T⋅m/A or N/}\,\text{A}^2$
    - $c_{\text{accepted}}$: accepted value of the speed of light, $2.9979\times10^8\,\text{m/s}$
    - Also add in the plotting-derived (i.e. from `LINEST`) $\varepsilon_0$ from the first lab for each member of your lab group
      - Of your group members' values, take the average ($\overline \varepsilon_0$), and use the standard deviation ($\sigma \varepsilon_0$) of your groups' values as the uncertainty for later speed of light use.
      - *If you are completing the lab individually*, use your single plotting-derived $\varepsilon_0$ and its associated uncertainty $\delta \varepsilon_0$


(restart_step_for_mu0)=
4. In order to measure the equilibrium separation distance, $d_\text{center-to-center}$, of the conductors, two readings are made.

    - The first is the scale reading, $S_0$, at the equilibrium position, i.e. when no mass has been added to the pan on the movable conductor.
    - The second scale reading, $S_1$, is made when the top conductor contacts the lower conductor ({numref}`fig-measurement-apparatus`). Place a sufficient mass in the pan on the top conductor to make it contact the lower, stationary conductor. Record $S_1$.
      - ⚠️ ***POWER MUST BE OFF FOR THIS STEP*** ⚠️
      - You will periodically verify that $S_0$ and $S_1$ are not changed throughout the experiment.
    - Determine $D = | S_1 - S_0 |$ from two scale readings (reminders: absolute value there is to represent the total distance between $S_0$ and $S_1$. If your crosshair crosses 0, make sure to consider the negative).
    - Calculate and record the conductor separation distance, $d_\text{center-to-center}$. Refer to {numref}`fig-apparatus-diagram`, {numref}`fig-measurement-apparatus`, {eq}`eq-center-separation`.

5. Prepare a data table with columns for the variables below. You'll have rows for each trial as well as for averages. Reminder, you will conduct 27 trials total by conducting **three rounds** of *sequentially changing* the applied masses:
      - Trial number
      - Lab member's initials (person looking through telescope)
      - $m_{\text{applied}}$: Applied mass
      - $F_B$: Applied magnetic force
      - $I_\text{min}$: Minimum current $I$ required to return to the equilibrium position
      - $I_\text{max}$: Maximum current $I$ required to return to the equilibrium position
      - $I$: Current $I$ required to return to the equilibrium position
      - $\delta I$: Estimated current uncertainty ***(to be assumed as majority source of uncertainty for today)***
      - $I^2$: Current squared
      - $\delta I^2$: Current squared
      - $\mu_{0\text{,experimental}}$: Experimental value of $\mu_0$
      - $\mu_{0\text{,experimental,max}}$: Maximized experimental value based on $\delta I^2$
      - $\delta \mu_{0\text{,experimental}}$: Uncertainty in experimental value
      - $\Delta \mu_{0\text{,experimental vs. accepted}}$: Magntitude of difference between experimental and accepted values of $\mu_0$


(data-collection-mu0-section)=
### ● Experimental Data Collection

6. With the power off 🟥, make sure the conductor beam is still at equilibrium, then place the current trial's mass $m_\text{applied}$ on the upper conductor (see full list in {numref}`magnetic-force-trials-table`). The top bar will swing downwards. In following steps, you will apply a current to counteract the gravitational force. Record the trial's mass value and calculate $F_\text{B}$ (reminder, use SI units; these masses are in units of milligrams; *hint: what does the magnetic force balance?*).

    ```{table} Experimental Trials Breakdown
    :name: magnetic-force-trials-table
    | Student on telescope | Trial Applied Masses (mg) | POWER ON 🟢 / Off 🟥 |
    |---------|-------------------|-------------------|
    | Student #1 | 200, 175, 150, 125, 100, 75, 50, 25 | ON 🟢 |
    | Student #1 (and #2) | 0 (ensure $S_0$ has not changed) | Off 🟥 |
    | Student #2 | 200, 175, 150, 125, 100, 75, 50, 25 | ON 🟢 |
    | Student #2 (and #3) | 0 (ensure $S_0$ has not changed) | Off 🟥 |
    | Student #3 (or #1<br>again for a group of two) | 200, 175, 150, 125, 100, 75, 50, 25 | ON 🟢 |
    | Student #3 (and #1) | 0 (ensure $S_0$ has not changed) | Off 🟥 |
    ```

    ```{admonition} Consider: 0 mg Trials
    :class: question
    Why do we have the power off for the 0 mg trials, but not the other masses?
    ```

7. Determine current $I$ required to balance the weight of the added mass and return to equilibrium by finding a current range. **Make sure the transformer setting is zero before turning on the power.** Turn on 🟢 the power supply and slowly increase the current until the bars return to parallel (i.e. crosshair in telescope back to $S_0$, as it was with no applied mass on the top). Determine this by having an observer watching the scale reading with the telescope during this process. The telescope observer should be calling out instructions to the power supply operator to slowly approach the $S_0$ value.
    - When the $S_0$ value is approximately reached, call out to the power supply operator.
    - Power supply operator shall decrease the current *until the telescope observer is no longer confident* the crosshair is at the $S_0$ position, at which point the telescope observer shall call for a minimum current reading from the multimeter and record the lower end of the range of current $I_\text{min}$.
    - Power supply operator shall then increase the current *until the telescope observer is no longer confident* the crosshair is at the $S_0$ position, at which point the telescope observer shall call for a maximum current reading from the multimeter and record the upper end of the range of current $I_\text{max}$.
    - **As soon as you make these readings, reduce the transformer setting to zero and turn off 🟥 the power switch. Under no circumstances should the current exceed 20 A.**
    - Calculate applied current $I$ as the average of the min and max currents, $I\,=\,(\,I_\text{max}\,
    +\,I_\text{min}\,)\,/\,2$
    - Calculate applied current uncertainty $\delta I$ as half the difference between max and min current, $\delta I\,=\,(\,I_\text{max}\,-\,I_\text{min}\,)\,/\,2$
    - Calculate $I^2$ as well as $\delta I^2$ by maximizing and taking the difference (i.e. $\delta I^2 = (I + \delta I)^2 - I^2$)

    ```{admonition} Wire Burn Out
    :class: warning
    **DO NOT LEAVE THE POWER ON, IT CAN BURN OUT THE WIRES IF LEFT ON TOO LONG AND CAUSE INJURY**
    ```

8. For the current trial, calculate $\mu_{0\text{,experimental}}$ from {eq}`eq-parallel-conductor-force` and determine its uncertainty by maximizing by your measurement uncertainties (primarily due to current today) and taking the difference (i.e. $\delta \mu_{0\text{,experimental}} = \mu_{0\text{,experimental,max}} - \mu_{0\text{,experimental}}$, *hint: should be a positive value*).

9. Also calculate the difference $\Delta \mu_{0\text{,experimental vs. accepted}}$ between your experimental and accepted permeability of free space values for quick comparisons.

10. With power off, replace the applied mass for the next trial, and repeat the previous steps in {ref}`data-collection-mu0-section` to find the current required to balance the system again, and subsequently calculate $\mu_0 \pm \delta \mu_0$ again.

    ```{admonition} Sequential Trials Reminder
    :class: tip
    Do the rounds sequentially (e.g. 200, 175, 150... then change telescope observer and repeat 200, 175, 150... mg) rather than all trials of a single applied mass at once to ensure you catch and correct any significant errors early (e.g. if the apparatus is bumped out of alignment) rather than having to do all trials again. 
    - Reminder, equilibrium is with no applied mass, when the power supply if off; ***why?***
    ```


### ● Data Analysis

#### ○ Averages


11. Calculate your average values from everyone's trials (ignoring those that give a divide-by-zero error):
    - Average experimental value $\mu_{0\text{,experimental,avg}}$
    - Average experimental uncertainty $\delta\mu_{0\text{,experimental,avg}}$
    - $\overline{\Delta \mu_{0\text{,experimental vs. accepted}}}$, the average difference between experimental and accepted $\mu_0$


    ```{admonition} Average of Uncertainties
    :class: note
    - Using the average of individual trial uncertainties is generally not statistically rigorous because independent random uncertainties should decrease as $1/\sqrt{N}$.
    - However, for simplicity in today's lab and assuming systematic errors dominate, we can use it as an acceptable conservative upper bound of our experimental average's true uncertainty.
    ```

12. If, after performing the graphical data analysis below, you find some or all of the data unacceptable, repeat from {ref}`Step 4 <restart_step_for_mu0>`, checking that the telescope and scale were not disturbed during your measurements.


#### ○ Graphical

13. The graphical display of data permits the comparison of all the values and associated errors at once. Points that depart markedly from the general trend of the data are quickly detected. We expect from theory {eq}`eq-parallel-conductor-force` that magnetic force and current are related like:

    ```{math}
    :label: eq-force-current-squared
    F_B=k I^{2}
    ```

    Using **all** of your data points from **all rounds and trials**, including those at equilibrium ($0\,\text{mg}$) that you should have ignored earlier when you calculated $\mu_0$ for each individual trial and the overall average:

    A) ***SCATTER PLOT 1*** --- $F_B$ vs. $I^{2}$ (i.e. $F_B$ as ordinate ($y$) and $I^{2}$ as abscissa ($x$)). Fit a trend line through the all these points, display the trendline equation on the chart, and confirm the slope of the line $k$ matches what you found with the `LINEST()` function (for review, see {ref}`data-acquisition-plotting-in-excel`). From {eq}`eq-parallel-conductor-force` and {eq}`eq-force-current-squared`, the value of $k$ is given by {eq}`eq-slope-constant`.

      ```{math}
      :label: eq-slope-constant
      k=\frac{\mu_0}{2\pi}\frac{L}{d_\text{center-to-center}}
      ```

      - Calculate the plotting or slope-derived $\mu_{0\text{,slope-derived}}$ by rearranging {eq}`eq-slope-constant` and using this experimentally determined value $k$.
      - Similar to earlier, calculate $\delta\,\mu_{0\text{,slope-derived}}$ by maximizing by the slope uncertainty (output from the `LINEST()` function), and subsequently taking the difference: $\delta\,\mu_{0\text{,slope-derived}} = \mu_{0\text{,slope-derived,max}} - \mu_{0\text{,slope-derived}}$
      - Also calculate the difference between the slope-derived and accepted permeability of free space values to quickly compare whether your results agree with the accepted value.

    B) ***SCATTER PLOT 2*** --- $F_B$ vs. $I$. Fit a quadratic (a.k.a. polynomial order of 2) trend line, and display the equation.

      ```{admonition} Discussion Point: Linear vs. Quadratic
      :class: question
      Notice the shape of the data. How does this compare to your first plot?
      - What is the physical relationship between $F_B$ and $I$? What does it mean for magnetic force when current is doubled?
      - Would you expect the linear fit to go through the **origin** of the $F_B$ vs. $I^2$ plot? 
      ```

#### ○ Speed of Light

14. Using the average of your group's experimentally-determined **plotting-derived** values of the electric constant ($\overline \varepsilon_0$) from the {ref}`Electric Force & ε₀ Lab <electric-force-and-epsilon-overall>`, and the **plotting-derived** value of $\mu_{0\text{,slope-derived}}$ determined above, calculate your estimate for the speed of light $c$ with {eq}`eq-speed-of-light`.
    - As should be in your common data table, and if not yet completed, average the group members' plotting-derived values of the electric constant ($\overline \varepsilon_0$), and use the standard deviation $\sigma \varepsilon_0$ of your groups' values as its uncertainty.
      - *If you are completing the lab individually*, use your single plotting-derived $\varepsilon_0$ and its associated uncertainty $\delta \varepsilon_0$

15. Estimate your uncertainty in $c$ by maximizing and taking the difference. Reminder, for $\delta \mu_0$ from today's error propagation, and $\delta \varepsilon_0 = \sigma \varepsilon_0$:

    ```{math}
    :label: eq-speed-of-light_uncertainty
    \delta c = \sqrt{\frac{1}{(\overline{\varepsilon_0}-\delta\varepsilon_0) \times (\delta\,\mu_{0\text{,slope-derived}} - \delta\,\mu_{0\text{,slope-derived}})}} - c
    ```

### ● Summary and Cleanup


16. Create a summary table of your data (e.g. average $\mu_0$, slope-derived $\mu_0$, and speed of light values with their uncertainties, as well as the differences between experimental and accepted values).

17. When you are finished, reset your experimental setup before leaving.

    ```{admonition} CLEAN UP
    :class: important
    Please return your experimental station back to the way you found it or better:
     - Return all masses (5, 20, 50, 100, 200 mg) and tweezers to black mass case, ensuring the clear plastic cover holds the masses down inside the case. Place black case near multimeter or power supply.
        - Please inform instructor of any lost masses
     - Power supply is off, voltage knobs turned down to zero
     - Multimeter off
     - Ensure telescope is in focus and pointed at the mirror/scale
    ```



## Post-Lab Submission --- Interpretation of Results

### ● Finalized Spreadsheets

  - Make sure to submit your finalized data table (Excel sheet).
  - Please include concise summary table.
  - Please include plots:
    - $F_B$ vs $I^2$
    - $F_B$ vs $I$ (for qualitative comparisons)


### ● Post-lab Writeup

- In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
  - What is the precision of your equipment?
  - What are possible sources of systematic (i.e. affecting accuracy) and random (i.e. affecting variance) errors?
  - What are your measured uncertainties, and, based on these uncertainties, how do your final results for $\mu_0$ change? I.e. do your different measurement and slope uncertainties make your final results larger or smaller?
  - The following variables are ones you had control over for today's lab. Individually increase each by 1% in your Excel sheet (i.e. multiply by 1.01). How do these changes affect your final $\mu_0$ values; which has the greatest affect? If results are larger or smaller, are they more or less accurate to expected values?
    - Mass
    - Current
    - $d_\text{center-to-center}$
  - Based on your uncertainties (i.e. $\delta \varepsilon_0$ and $\delta \mu_0$), how do they affect you experimental value for speed of light $c$? (i.e. larger/smaller? one more than the other?)


- In a **paragraph**, summarize the results you have determined for all cases. Consider:
  - What was the point of today's lab; what did we aim to discover?
  - Compare your experimental values of $\mu_0$ from plotting with {eq}`eq-slope-constant` and the $\overline{\mu_0} \pm \delta \mu_0$ of your values from {eq}`eq-parallel-conductor-force`.
    - Do they agree with each other?
    - Do they agree with the accepted value of $\mu_0 = 1.2566\times 10^{-6}$ T⋅m/A?
  - What is the relationship between $F_B$ and $I$?
  - Explain physically, why would you expect the linear fit to go through the origin?
  - Does your plotting-derived experimental value for $c$ agree with the accepted value of the speed of light ($c = 2.9979\times10^8\,\text{m/s}$)?
  - Given the following as unchanging: the phyiscal dimensions of our apparatus setups for this lab and the $\varepsilon_0$ lab, their respective currents and voltages for a individual trial:
    - If you were to find the speed of light $c$ to be ***larger*** than the accepted value above, what would it imply about electric and magnetic fields/forces?





## The Whiteboard

2026 updates/notes on whiteboard summaries:

  - Wires are thicker and safer now, still don't touch, don't exceed 20 A
  - Masses in **decreasing** order, rather than increasing order
  - Using average and **uncertainty** (not standard deviation)
  - Speed of light just from **plotting-derived** (i.e. from `LINEST`) values from first lab ($\varepsilon_0$) and today's lab ($\mu_0$)

```{figure} Mu0Figures/mu0_2025_Summer_01_v01.jpg
:name: mu0_whiteboard_01
:width: 100%
:align: center

Overview. `LINEST()` function.
```

```{figure} Mu0Figures/mu0_2025_Spring_02_v02.jpg
:name: mu0_whiteboard_02
:width: 80%
:align: center

Separation distance equation; multimeter settings.
```

```{figure} Mu0Figures/mu0_2025_Summer_03_v02.jpg
:name: mu0_whiteboard_03
:width: 100%
:align: center

Plot notes; Speed of Light calculations.
```