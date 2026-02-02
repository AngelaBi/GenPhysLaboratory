(electric-force-and-epsilon-overall)=
# Electric Force & the Determination of $\varepsilon_0$

## Background

### Background Overview

```{danger}
**⚠️⚠️⚠️⚠️ WARNING ⚠️⚠️⚠️⚠️**

**⚠️⚠️⚠️⚠️ HIGH VOLTAGE IN USE TODAY ⚠️⚠️⚠️⚠️**

**⚠️⚠️⚠️⚠️ DO NOT TOUCH THE METAL PLATES ⚠️⚠️⚠️⚠️**

**⚠️⚠️⚠️⚠️ YOU CAN GET SERIOUSLY INJURED ⚠️⚠️⚠️⚠️**

**⚠️⚠️⚠️⚠️ WARNING ⚠️⚠️⚠️⚠️**
```

```{admonition} OVERALL GOALS
:class: note
Use a parallel-plate capacitor to create a uniform electric field to:
  - Investigate the relationship between electric force $F_E$ and voltage $V$ (i.e. $F_E$ vs. $V$).
  - Experimentally determine the electric constant $\varepsilon_0$ (a.k.a. vacuum permittivity).
```

The electric constant, $\varepsilon_0$ (pronounced "epsilon nought" or "epsilon zero"), is a fundamental constant of nature. Also known as vacuum permittivity, permittivity of free space, or dielectric permittivity of the vacuum, it is a measure of how dense of an electric field is "permitted" to form in response electric charges. As such, it is also the proportionality constant that relates the **electric force between two charges**. The constant $\varepsilon_0$ is also related to the constant $k$ in Coulomb's Law which describes the electrostatic force $F_E$ between charges:

```{math}
:label: eq_coulomb_basic
F = F_\text{electric} = F_E = k\frac{Q_1 Q_2}{r^2},
```

where $Q$ is the charge in Coulombs, $r$ is the separation distance between charges in meters, and

```{math}
:label: eq_k_epsilon
k = \frac{1}{4 \pi \varepsilon_0}.
```

The subscript zero refers to the baseline value of the permittivity of free space. 

### Electric Force Between the Plates of a Parallel-Plate Capacitor


If we apply Coulomb's law to the special case of two *large*, *closely-spaced*, *parallel plates*, we can derive an expression for the electric force between the two plates. This electric force is due to the uniform electric field generated between this configuration known as the **parallel-plate capacitor** as seen in {numref}`E1Fig_0002`.


```{figure} Eps0Figures/E1_Fig_0002_parallelPlates_v01.png
---
width: 60%
name: E1Fig_0002
---
Example of a parallel-plate capacitor. Plates of area $A$ are seaparated $d$ apart with charge $Q$ built up on each plate based on the applied voltage which creates a uniform electric field.

A parallel-plate capacitor with idential plates of the same surface area A separated by a distance d, each plate has the same surface area A.
```

Consider such a parallel-plate capacitor with plate area $A$, separation $d$, and an applied potential difference $V$. When a voltage is applied, equal and opposite charges $\pm Q$ accumulate on the plates, producing a surface charge density

```{math}
\sigma = \frac{Q}{A}.
```



#### Electric Field of the Plates

A single (ideally) infinite sheet of charge with surface charge density $\sigma$ produces a uniform electric field one either side of that sheet with a magnitude

```{math}
E_{\text{single sheet}} = \frac{\sigma}{2\varepsilon_0}.
```

In a parallel-plate capacitor, the two plates carry equal and opposite surface charge densities $\pm \sigma$. The electric fields due to each plate **add between the plates** and **cancel outside the capacitor**, resulting in a uniform electric field between the plates:

```{math}
E_\text{between plates} = \frac{\sigma}{\varepsilon_0}.
```

Because the field is uniform, the potential difference between the plates is related to the field by

```{math}
V = Ed \quad \Rightarrow \quad E = \frac{V}{d}
```

where to increase the electric field strength, you can either increase the voltage or decrease the separation distance between the plates.


#### Force on a Plate

A key point is that a charged plate does **not** exert a force on itself. The force on one plate arises solely from the electric field produced by the *other* plate.

The electric field at one plate due to the opposite plate alone is therefore

```{math}
E_{\text{other}} = \frac{\sigma}{2\varepsilon_0}.
```

The force on a plate carrying total charge $Q$ (i.e. the electric force that the charges on the one plate feel due to the other plate's electric field) is

```{math}
F_E = Q E_{\text{other}} = Q \left( \frac{\sigma}{2\varepsilon_0} \right).
```

Substituting $\sigma = \frac{Q}{A}$ gives

```{math}
F_E = \frac{Q^2}{2\varepsilon_0 A}.
```



#### Force in Terms of Voltage

Using the relation between surface charge density and electric field,

```{math}
E = \frac{\sigma}{\varepsilon_0} = \frac{V}{d}
\quad \Rightarrow \quad
\sigma = \varepsilon_0 \frac{V}{d},
```

the charge on a plate becomes

```{math}
Q = \sigma A = \varepsilon_0 A \frac{V}{d}.
```

Substituting this expression for $Q$ into the force equation yields

```{math}
F_E = \frac{(\varepsilon_0 A V / d)^2}{2\varepsilon_0 A}
= \frac{\varepsilon_0 A V^2}{2 d^2}.
```



#### Final Result


The following expression gives the magnitude of the attractive electric force between the oppositely-charge plates of an ideal parallel-plate capacitor.

```{math}
:label: eq_electric_force
\boxed{
F_E = \frac{\varepsilon_0 A V^2}{2 d^2}
}
```
















<!---
When a voltage $V$ is applied between the plates of a parallel-plate capacitor, charge is distributed evenly, such that total the surface charge density is $\sigma = Q/A$; charge $Q$ is distributed across the area $A$ of each plate in equal, but opposite sign. If looking as just a single plate by themselves, it creates its own electric field on either side of the plate such that the electric field for one side of the plate is due to half of the charge, leading to a magnitude $E_\text{singlePlateSide} = \frac{\sigma}{2 \varepsilon_0} = \frac{Q}{2 \varepsilon_0 A}$. 


(i.e. as if the charges are distributed on both the inside of the capacitor and outside of the capacitor).

When the distance $d$ between the plates is small, the charges from each plate create a uniform electric field between the plates with magnitude $E = \frac{\sigma}{\varepsilon_0} = \frac{Q}{\varepsilon_0 A}$. This describes how dense of an electric field is permitted to form due to the surface charges.

Now since the electric field is uniform, we can also describe the potential difference as $V = Ed$, which can be rearranged to show the *total* magnitude of the electric field from both plates as $E = \frac{V}{d}$, with $V$ as the voltage (potential difference) between the plates, and $d$ the separation distance between parallel plates.

To create the uniform field between the plates, we must note that each plate themselves create their own electric fields that **act soley on the opposite plate** (an individual plate's field cannot affect itself). We must also recognize that the charge $Q$ is distributed across both sides of a individual plate, so the electric field generated by one side of a single plate is due to half of the charge. This leads to the electric field for a single plate becomes thus just half, $E_\text{single} = \frac{\sigma}{2 \varepsilon_0} = \frac{Q}{2 \varepsilon_0 A}$. The electric force that the charges on the opposite plate would feel is $F = Q E_

is electric fields subsequently applies an electric force on the charges of the opposite plate. Outside the plates, the electric field cancels out

From electrostatics, we know the electric field is uniform with a magnitude $E = \frac{V}{d}$, with $V$ as the voltage (potential difference) between the plates, and $d$ the separation distance between parallel plates. The electric force of attraction between two oppositely charged plates is then


```{math}
:label: eq_electric_force
F_E = \frac{\varepsilon_0 A V^{2}}{2 d^{2}}
```


--->

where $A$ is the area of the plates, $d$ the separation distance, and $V$ the potential difference in volts across the plates.

*{eq}`eq_electric_force` is valid only under the conditions stated of large, closely spaced plates to provide a uniform electric field and charge density so we can effectively ignore fringe fields*. The physical implications of these geometric assumptions is that the electric field is totally confined to the space between the plates and is constant in value throughout the space. You will see in Lab E-2 that the electric field always 'bulges' or fringes out at the edge. For {eq}`eq_electric_force`, the fringe field is ignored. Rewriting the expression for $\varepsilon_0$, we obtain

```{math}
:label: eq_epsilon_0
\varepsilon_0 = \frac{2 F_E d^{2}}{A V^{2}}.
```

By measuring electric force, voltage, and geometry of the apparatus, $\varepsilon_0$ can be determined.




### Equipment List

Depicted across {numref}`E1Fig_00` -- {numref}`E1Fig_02`. All equipment as listed can be seen first in {numref}`E1Fig_00`.

- Telescope with crosshair & centimeter-scale ruler (a.k.a. scale) on vertical pole
- High voltage DC power supply, 0 -- 500 V
- Fluke multimeter -- set to read DC voltage (in parallel with parallel-plate capacitor)
- Small masses of 10, 20, 20, 100, 500 mg with plastic tweezers
- Parallel-plate capacitor apparatus:
  - Bottom plate held in static position on lower plate adjustment towers
  - Balanced plate/beam on thin, conductive, knife edges with:
      - Top plate with a "$+$" for where to place applied masses
        - Can swing up or down when changing amount of applied mass or voltage
        - Set up to be parallel (i.e. equilibrium) to bottom plate when holding $50\,\text{mg}$
      - Mirror to view the scale (ruler) via telescope to determine angle of plates and subsequent separation distance $d$ between plates
      - Beam lift knobs to reset top plate position after accidental bumps
      - High impedance ($1\,\text{M}\Omega$) resistor to limit current (contained in long gray box, shouldn't need to touch)
  - Leveling screws to level whole apparatus to the table
  - Metal connections to the power supply
- x5 Banana plug wires (12 AWG: x2 3', x1 1'; 18 AWG: x2 2'), connecting power supply to voltmeter & parallel-plate apparatus
- Protective box with the mirror-to-scale distance $b$ written on it


```{figure} Eps0Figures/fig_00_OverallApparatus_v02.png
---
width: 100%
name: E1Fig_00
---
Top) Example of the entire setup (note: actual setups will have telescope/scale on separate table further away). Bottom) Front view of capacitor apparatus; protective box.
```




### Adjustment of apparatus (check with Instructor if needed)

The apparatus has been carefully adjusted before your lab and should not require further significant adjustments. This section describes how the apparatus was prepared. If something seems to need adjusting, see the lab instructor.

1. The beam lift (knob location noted in {numref}`E1Fig_00` bottom-left) provides a definite location for the beam and thus guarantees continued alignment of the parallel plates. Use the beam lift each time you change weights or relocate the counter weight.
2. Both plates can be adjusted vertically and horizontally in order to make it possible for the plates to be parallel. The counterweight behind the mirror can be used to establish the equilibrium separation of the plates. The plates should have already been adjusted parallel with the counterweight set so the plates are essentially parallel when a $50\,\text{mg}$ mass is placed on the movable plate. *If the plates are NOT parallel with the $50\,\text{mg}$ mass in place, seek the instructor's help.*
3. The apparatus can be leveled with the leveling screws so that it sits flat on the table.
4. Mirror-to-scale distance was measured from rear of mirror (reflective surface) to ~center of $S_0$ and $S_1$ on the scale (ruler).

## Experimental Procedure



### Procedure Preview

```{danger}
**⚠️⚠️⚠️⚠️ DO NOT TOUCH THE METAL PLATES ⚠️⚠️⚠️⚠️**

**⚠️⚠️⚠️⚠️ TURN OFF POWER WHEN CHANGING APPLIED MASSES ⚠️⚠️⚠️⚠️**
```
 <!--- You will conduct :
   - Each Case with have either **10** or **15 trials**:
      - Each student will complete a total of 5 trials each, with:
        - Groups of 2 --- 10 trials
        - Groups of 3 --- 15 trials
  - Visualize a
  !!!!!!!!!!!!!!!!!!!!!!!! UPDATE !!!!!!!!!!!!!!!!!
  --->

```{admonition} OVERVIEW
:class: note
   - Experimentally investigate the relationship between electric force and applied voltage to determine the electric constant $\varepsilon_0$.
  - In this experiment, you will:
    - Use telescope and scale to determine equilibrium position and separation distance between the parallel plates, $d$
    - Conduct **3 rounds** of replacing equilibrium mass with a series of smaller masses (less gravitational force)
      - Increase electric force by applying the necessary voltage $V$ to the plates such that they return to equilibrium separation distance $d$ (i.e. parallel)
      - Note: under these conditions, the electric force required to maintain the separation $d$ will be equivalent to the difference of the gravitational force of the equilibrium and smaller applied mass.
    - Determine $\varepsilon_0$ for each trial (ignroing equilibrium mass) and its uncertainty
    - Determine average $\varepsilon_0$ of all your trials (ignroing equilibrium mass) and its uncertainty
    - Determine $\varepsilon_0$ from plotting of all your data (including equilibrium mass) as $F_E\,\text{vs.}\,V^2$
    - Compare your results from both analysis methods to the accepted $\varepsilon_{0\text{,accepted}}$.
```

```{admonition} Additional Tips
:class: tip
- Do the rounds sequentially (e.g. 50, 40, 30... then repeat 50, 40, 30... mg) rather than all trials of a single applied mass at once to ensure you catch and correct any significant errors early (e.g. if the apparatus is bumped out of alignment) rather than having to do all 18 trials again. 
- Reminder, 50 mg is equilibrium mass when the power supply if off (i.e. applied voltage is zero).
```

```{admonition} Combining results from today's lab with future $\mu_0$ lab for **speed of light** $c$
:class: note
You will experimentally determine $\varepsilon_0$ today; a few weeks from now in Lab: {ref}`Magnetic Force & the Determination of μ₀ <magnetic-force-mu0-overall>`, you will determine its magnetic equivalent, $\mu_0$. Using both in that later lab, we will determine the speed of light (i.e. magnitude of the velocity of propagation of an electromagnetic wave). You will want to make sure to take note of your value $\varepsilon_0$ for future use.
``` 


(demo-video-electric-constant)=
### Demo Video

<div style="text-align: center;">
  <iframe
    width="80%"
    height="315"
    src="https://www.youtube.com/embed/2GMHmCrCKLQ"
    title="YouTube video"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
  <figcaption>Demonstration video. Reviews overall setup and procedure. *No audio*</figcaption>
</div>

If embedding is broken, follow: <a href="https://www.youtube.com/watch?v=2GMHmCrCKLQ" target="_blank" rel="noopener noreferrer">
https://www.youtube.com/watch?v=2GMHmCrCKLQ
</a>


### Preliminary Setup

**All given lengths you will use are represented in {numref}`E1Fig_01`.**

```{figure} Eps0Figures/fig_01_Apparatus_v03.png
---
width: 100%
name: E1Fig_01
---
Parallel Plate Capacitor Apparatus. 
Top-left) Schematic showing given dimensions and determined plate separation $d$. 
Top-right) Determined plate separation $d$ when parallel (i.e. at equilibrium with no applied voltage).
Middle) Example apparatus with given dimensions. 
Bottom) Example of mirror-to-scale distance.
```


1. Prepare a common data table including given values.
   Reminder -- keep variable names and units in the row and column titles, and numbers in their own Excel cells to be able to reference in your equations. Include, but not limited to:
    - $g = 9.803 \,\text{m/s}^2$: Accepted value of accel. due to garvity for Fairfield University
    - $\varepsilon_{0\text{,accepted}} = 8.8542\times 10^{-12}\,\text{C}^2 \, \text{N}^{-1} \text{m}^{-2}$: Accepted value of electric constant
    <!---   - $a \pm \delta a=0.279\pm0.001\,\meter$: Length of the frame (see Fig.~\ref{E1Fig:01}) --->
    - $a=0.279\,\text{m}$: Length of the frame from pivot to end of plate (see {numref}`E1Fig_01`)
    <!---   - $b \pm \delta b = b \pm 0.003\meter$: Mirror-to-scale distance, has already been measured and is posted on the top of the protective enclosure ({numref}`E1Fig_01` bottom) --->
    - $b$: Mirror-to-scale distance, has already been measured and is posted on the top of the protective enclosure ({numref}`E1Fig_01` bottom)
    <!---   - $A \pm \delta A =0.0161\pm0.0002\,\meter^2$: Plate area ({numref}`E1Fig_01`) --->
    - $A=0.0161\,\text{m}^{2}$: Plate area ({numref}`E1Fig_01`)
    - $m_0 = 50\,\text{mg}$: Equilibrium mass (plates are parallel when this amount of mass applied).
    - $F_0 = m_0 g$: Equilibrium force
    - $S_{0}$: Scale reading at equilibrium (m)
    - $S_{1}$: Scale reading when plates are in contact (m)
    - $d$: Separation distance between the plates when the top plate is **parallel** to the bottom plate when equilibrium mass ($50\,\text{mg}$) is placed on the top plate (see examples in {numref}`E1Fig_01` top-right and {numref}`E1Fig_02` middle)



    ```{admonition} Calculations in Spreadsheet
    :class: tip
    Run all your calculations in your Excel sheet so your instructor can see how you arrived at your final results.
    ```



    ```{admonition} Power Supply
    :class: warning
    Do not turn on the power supply until told to do so in the steps below.
    ```

2. Note the center marking "**+**" on the top of the movable plate where masses must be placed using the tweezers (see {numref}`E1Fig_03`).

```{figure} Eps0Figures/fig_03_MassPlacement.png
---
width: 80%
name: E1Fig_03
---
Example of masses to use (milligrams). Placement location marked by the +.
```

3. Investigate the use of the telescope and scale so that the rotation of the balanced frame can be measured in terms of scale divisions (see {numref}`E1Fig_02`). Numbers are in cm, small lines in mm.

```{figure} Eps0Figures/fig_02_MeasuringApparatus_v02.png
---
width: 80%
name: E1Fig_02
---
Top-left) Schematic of the Measuring Apparatus. Top-right) Example of $S_{0}$ and $S_{1}$ on the scale. Bottom) Example of the plates and cross-hairs through the telescope for finding $S_{0}$, $S_{1}$, and scale difference $D$. Note for the $S_{0}$ and $S_{1}$ readings, the scale numbers are black and red, respectively; this indicating we crossed the zero line and changed signs.
```


```{math}
:label: eq_distance_d
d = \frac{D a}{2 b}
```

<!---  <a id="procedure-epsilon0-step-s0-s1"></a> --->
(procedure-epsilon0-step-s0-s1)=
4. Review the {ref}`demo-video-electric-constant`. Determine separation distance $d$ of the plates when they are essentially parallel with $50\,\text{mg}$ applied. To do so, perform a geometrical analysis of similar triangles that describes the vertical displacement of the plate as given by {eq}`eq_distance_d`. $D$ is the change in scale reading between when the equilibrium mass is on the plate and when the plates are in contact (example shown in {numref}`E1Fig_02`) and $a$ and $b$ as described earlier (further described in {numref}`E1Fig_01`). The factor of 2 results from the fact that the optical path reflected off of the mirror to the scale rotates through an angle twice that of the beam holding the movable plate. Determine $D = | S_1 - S_0 |$ from two scale readings (reminders: absolute value there is to represent the total distance between $S_0$ and $S_1$. If your crosshair crosses 0, make sure to consider the negative). Perform the following:
   - The first scale reading, $S_0$, is made when the separation of the plates is such that the plates are essentially parallel. This should happen when an applied mass of $50\,\text{mg}$ is centered on the movable plate. If not, call over an instructor.
   - The second scale reading, $S_1$, is made when the top plate contacts the bottom plate ({numref}`E1Fig_02`). Place a sufficient mass (e.g. $500\,\text{mg}$) on the movable plate to make it contact the lower, stationary plate
      - ⚠️ ***POWER MUST BE OFF FOR THIS STEP*** ⚠️
      - You will periodically verify that $S_0$ and $S_1$ are not changed throughout the experiment.
   - Record $S_0$, $S_1$, and $D = | S_1 - S_0 |$ in your common data table.
   - Also include the equilibrium mass $m_0$, the equilibrium force ${F_0 = m_0 g}$, distance $a$, and distance $b$ found on your apparatus cover.
   - Calculate the plate spacing $d$ using {eq}`eq_distance_d`.


5. We can now determine an experimental value of $\varepsilon_0$ from the values in the common data table and the experimental voltage from each trial. You will perform at least three trials for each of the six different applied masses on the movable plate (18 total trials). Set up an experimental data table to record your measurements and calculate the experimental value of $\varepsilon_0$. Include enough rows for trials and columns for:
      - Trial number
      - Lab member's initials (person looking through telescope)
      - $m_{\text{applied}}$: Applied mass
      <!---  - Applied mass uncertainty $\delta m_{\text{applied}} = 0.01 \times m_{\text{applied}}$ (i.e. 1\%) --->
      - $F_{\text{applied}}=m_{\text{applied}} g$: Applied force
      <!---   - Uncertainty in the applied force $\delta F_{\text{applied}} = (m_{\text{applied}} + \delta m_{\text{applied}})g - F_{\text{applied}}$. This comes from the difference in a maximized value for the applied force and your value for the applied force. --->
      - $F_E$: Applied electric force
      - $V_\text{min}$: Minimum voltage $V$ required to return to the equilibrium position
      - $V_\text{max}$: Maximum voltage $V$ required to return to the equilibrium position
      - $V$: Voltage $V$ required to return to the equilibrium position
      - $\delta V$: Estimated voltage uncertainty ***(to be assumed as majority source of uncertainty for today)***
      - $\varepsilon_{0\text{,experimental}}$: Experimental value of the electric constant
      - $\varepsilon_{0\text{,experimental,maximized}}$: Maximized experimental value of the electric constant based on $\delta V$
      - $\delta\,\varepsilon_{0\text{,experimental}}$: Uncertainty in experimental value of the electric constant
      - $\Delta\,\varepsilon_{0\text{,experimental}} - \varepsilon_{0\text{,accepted}}$: Magntitude of difference between experimental and accepted values of $\varepsilon_0$



(detailsteps-Epsilon0Data)=
### Experimental Data Collection

(procedure-epsilon0-trial-list)=
6. Repeat the following steps for each trial with applied masses in order (to catch any procedural issues early):
    - The order of the trials for applied masses will be
      - 50 mg, ensure $S_0$ has not changed
      - 40, 30, 20, 10, 0 mg
      - pause, change group member on telescope
      - 50 mg, check $S_0$ and $S_1$ ***with power off***, re-running {ref}`Step 4 <procedure-epsilon0-step-s0-s1>` if needed
      - 40, 30, 20, 10, 0 mg
      - pause, change group member on telescope
      - 50 mg, check $S_0$ and $S_1$ ***with power off***, re-running {ref}`Step 4 <procedure-epsilon0-step-s0-s1>` if needed
      - 40, 30, 20, 10, 0 mg
    - Replace the equilibrium mass in the center of the top plate with the mass required for each trial. The top plate will swing upwards.

```{figure} Eps0Figures/fig_04_spark.png
---
width: 75%
name: E1Fig_04
---
Safety: regarding electricity and the plates touching. 
```

7. Apply current trial's mass to top plate and record that value (reminder, use SI units; these masses are in units of milligrams).

8. Determine applied voltage required to return to equilibrium by finding a voltage range. Turn on the power supply and slowly increase the voltage until the plates return to parallel (i.e. crosshair in telescope back to $S_0$, as it was with 50 mg on the top plate). Determine this by having an observer watching the scale reading with the telescope during this process. The telescope observer should be calling out instructions to the power supply operator to slowly approach the $S_0$ value.
    - When the $S_0$ value is approximately reached, call out to the power supply operator.
    - Power supply operator shall decrease the voltage *until the telescope observer is no longer confident* the crosshair is at the $S_0$ position, at which point the telescope observer shall call for a minimum voltage reading from the multimeter (not the power supply) and record the voltage $V_\text{min}$.
    - Power supply operator shall then increase the voltage *until the telescope observer is no longer confident* the crosshair is at the $S_0$ position, at which point the telescope observer shall call for a maximum voltage reading from the multimeter and record the voltage $V_\text{max}$.
    - Calculate applied voltage $V$ as the average of the min and max voltages, $V\,=\,(\,V_\text{max}\,
    +\,V_\text{min}\,)\,/\,2$
    - Calculate applied voltage uncertainty $\delta\,V$ as half the difference between max and min voltage, $\delta\,V\,=\,(\,V_\text{max}\,-\,V_\text{min}\,)\,/\,2$


    ```{admonition} Welded Plates \& Voltmeter Timeout
    :class: tip
    - Since the electric force will increase with decreasing separation, as seen from {eq}`eq_electric_force`, the plates have a tendency to continue through the $S_0$ point towards the zero separation point $S_1$. $S_0$ is an unstable equilibrium point. This may result in the plates sticking together and sparking as seen in {numref}`E1Fig_04`. If the plates stick together, **DO NOT TOUCH THE APPARATUS TO SEPARATE THE PLATES**. Turn off the power supply and tap the table in front of the apparatus; the plates should separate themselves. Accurate readings require care that the telescope and scale are not moved during the experiment. 
    - If the voltmeter display times out and goes blank, turn it off and on and reset the voltmeter to DC volts (sleep function).
    ```

9. Reduce the voltage to zero and turn off the power supply. 

10. For current trial, calculate:
    - the applied electric force --- the difference between the equilibrium force and the applied gravitational force, $F_E=F_0 - F_{\text{applied}}$ 
    - experimental electric constant $\varepsilon_{0_\text{experimental}}$ using {eq}`eq_epsilon_0`. For $50\,\text{mg}$ trials, this can be ignored as there should be no electric force used.
    - maximized electric constant $\varepsilon_{0\text{,experimental,maximized}}$ assuming uncertainty in voltage is majority source of uncertainty using the form of {eq}`eq_epsilon_0_max`.
    - Uncertainty in experimental value of the electric constant as $\delta\,\varepsilon_{0\text{,experimental}}=\varepsilon_{0\text{,experimental,maximized}} - \varepsilon_{0\text{,experimental}}$ 
    - $\Delta\,\varepsilon_{0\text{,experimental}} - \varepsilon_{0\text{,accepted}}$: Magntitude of difference between experimental and accepted values of $\varepsilon_0$


    ```{math}
    :label: eq_epsilon_0_max
    \varepsilon_{0\text{,experimental,maximized}} = \frac{2 F_E d^{2}}{A (V - \delta V)^{2}}.
    ```

    ```{admonition} Consider: Experimental vs. Accepted
    :class: question
    How do the experimental values compare to the accepted value? Reasonable or an outlier due to possible random or systematic errors?
    ```


11. Repeat {ref}`Steps 6 through 10 <procedure-epsilon0-trial-list>` for the listed mass trials until you've completed the listed number of rounds. On the equilibrium trials, check that $S_0$ and $S_1$ have not changed during your experiment.


12. Check if all the values are reasonably consistent. Retake any data that are clearly erroneous and recalculate.


### Experimental Data Analysis

13. Calculate your average values from everyone's trials (ignoring the $50\,\text{mg}$ trials):
    - Average experimental value $\varepsilon_{0\text{,experimental-average}}$
    - Average experimental uncertainty $\delta\varepsilon_{0\text{,experimental-average}}$
    - $\overline{\Delta\,\varepsilon_{0\text{,experimental}} - \varepsilon_{0\text{,accepted}}}$, the average difference between experimental and accepted $\varepsilon_0$


    ```{admonition} Average of Uncertainties
    :class: note
    - Using the average of individual trial uncertainties is generally not statistically rigorous because independent random uncertainties should decrease as $1/\sqrt{N}$.
    - However, for simplicity in today's lab and assuming systematic errors dominate, we can use it as an acceptable conservative upper bound of our experimental average's true uncertainty.
    ```

<!---
, which this method does not account for. However, it consistently overestimates the true uncertainty, making it acceptable as a conservative upper bound when systematic effects dominate or when avoiding underestimation is more important than precision.
    ```
--->

<!---

12. Add a row to your data table for calculating:
    - Average $\varepsilon_{0_\text{experimental-average}}$
    - Average $\delta\varepsilon_{0_\text{experimental-average}}$
    <!---   - Standard deviation $\sigma_{\varepsilon_{\text{0-experimental-average}}}$ (treating this as your overall uncertainty of your average value, e.g. avg ± σ. *Consider: does your experimental value ± range overlap with the accepted value of $\varepsilon_{0}$?*

--->


14. **Graphical Analysis:** The graphical display of data permits the comparison of all the values and associated errors at once. Points that depart markedly from the general trend of the data are quickly detected. We expect from theory {eq}`eq_electric_force` that electric force and voltage are related like:

    ```{math}
    :label: eq_force_voltage
    F_E = \alpha V^{2}.
    ```

    Using **all** of your data points from **all rounds and trials**, including those at equilibrium ($50\,\text{mg}$) that you should have ignored earlier when you calculated $\varepsilon_0$ for each individual trial and the overall average:

      1. ***SCATTER PLOT*** $F_E$ vs. $V^{2}$ (i.e. $F_E$ as ordinate ($y$) and $V^{2}$ as abscissa ($x$)). Fit a trend line through the all these points, display the trendline equation on the chart, and confirm the slope of the line $\alpha$ matches what you found with the `LINEST()` function (for review, see {ref}`data-acquisition-plotting-in-excel`). From {eq}`eq_electric_force`, the value of $\alpha$ is given by

      ```{math}
      :label: eq_alpha
      \alpha = \varepsilon_0\frac{A}{2 d^2}.
      ```

      A slope-derived $\varepsilon_0$ can now be determined by rearranging {eq}`eq_alpha` and using this experimentally determined value $\alpha$. Thus

      ```{math}
      :label: eq_epsilon_from_alpha
      \varepsilon_{0\text{,slope-derived}} = \frac{2 \alpha d^2}{A}.
      ```

      - Calculate $\varepsilon_{0\text{,slope-derived}}$
      - Similar to earlier, calculate $\delta\,\varepsilon_{0\text{,slope-derived}}$ by maximizing the slope by the slope uncertainty (output from the `LINEST()` function), and subsequently taking the difference: $\delta\,\varepsilon_{0\text{,slope-derived}} = \varepsilon_{0\text{,slope-derived,max}} - \varepsilon_{0\text{,slope-derived}}$
      - Also calculate the difference between the slope-derived and accepted electric constant.

      2. ***SCATTER PLOT*** $F_E$ vs. $V$. Fit a quadratic trend line, and display the equation.

    ```{admonition} Discussion Point: Linear vs. Quadratic
    :class: question
    Notice the shape of the data. How does this compare to your first plot?
    - What is the physical relationship between $F_E$ and $V$? What does it mean for electric force when voltage is doubled?
    - Would you expect the linear fit to go through the **origin** of the $F_E$ vs. $V^2$ plot? 
    ```

<!---    !!!!! CUT OUT DOING THE Y-INTERCEPT ~~~~~!!!!!!!!!!


    b. Your best fit line to $F_E$ versus $x=V^{2}$ should theoretically pass though the origin. Change the fit to force the line to have a $y$ intercept of 0. Recalculate your value of $\varepsilon_0$ as above. 

    !!!!! CUT OUT DOING THE Y-INTERCEPT ~~~~~!!!!!!!!!!
--->

15. Create a summary table of your data (e.g. average and slope-derived values with their uncertainties, difference between experimental and accepted value)


## Post-Lab Submission --- Interpretation of Results

### Finalized Spreadsheets

  - Make sure to submit your finalized data table (Excel sheet).
  - Please include relevant plot(s) including:
    - $F_E$ vs. $V^2$ with all data points across all trials, including those at equilibrium ($m = 50\,\text{mg}$).
    - $F_E$ vs. $V$ with all data points across all trials, including those at equilibrium ($m = 50\,\text{mg}$).


### Post-lab Writeup

- In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
  - What is the precision of your equipment?
  - What are possible sources of systematic (i.e. affecting accuracy) and random (i.e. affecting precision) errors?
  - What are your measurement uncertainties, and where do they come from?
  - How do your final results for $\varepsilon_0$ change based on your uncertainties (e.g. maximizing/minimizing voltage values)? Make sure to have completed error propagation calculations (described in the procedure) in your spreadsheet.

- In a **paragraph**, summarize the results you have determined, including both analysis methods. Consider:
  - What was the point of today's lab; what did we aim to discover?
  - Do your experimental results (average and slope-derived experimental values with their uncertainties) agree with the accepted value for $\varepsilon_0 = 8.8542 \times 10^{-12} \,\text{C}^2/\text{N}/\text{m}^2$?
  <!---- Does your linear (Y-int calculated normally) or linear-through-origin (Y-int = 0) plot more accurately represent the physical relationship between electric force and potential difference? --->
  - What is the physical relationship between $F_E$ and $V$?
  - What physically causes the top (movable) plate to feel an electric force?
  - Explain physically why you would expect the linear fit to go through the **origin** of the $F_E$ vs. $V^2$ plot?




## The Whiteboard

```{figure} Eps0Figures/eps0_2025_Spring_01_v01.jpg
:name: eps0_whiteboard_01
:width: 100%
:align: center

Overview. `LINEST()` function.
```

```{figure} Eps0Figures/eps0_2025_Spring_02.jpg
:name: eps0_whiteboard_02
:width: 100%
:align: center

Examples of balancing the plates --- 1) equilibrium (50 mg); 2) less applied mass, not parallel; 3) voltage applied, electric field generated,  pulls plates back together to parallel.
```