(rotational-dynamics-moi-angmom-lab-overall)=
# Rotational Dynamics with Moment of Inertia & Angular Momentum

## Background

```{admonition} OVERALL GOALS
:class: note
Conduct two experiments to investigate:
- ***Moment of inertia*** by determining angular acceleration for:
  - two point masses (mounted on a rod)
  - thick ring (placed on a disk)
- ***Conservation of Angular Momentum*** by determining angular velocity for:
  - thick ring dropped centered on axis of rotation
  - thick ring dropped off-axis
```

The motion of an object can be divided into two, completely independent parts: the **linear** (translational) motion of the center of mass and the **rotational** motion of the object around an axis *through the center of mass*. The linear motion is explained by Newton's 2nd Law of motion: a net force $F_{net}$ acting on an object of mass $m$ will cause the object to experience a linear acceleration $a$ given by

```{math}
F_{net} = m a
```

Rotational motion can be described in a very similar manner, but the quantities involved need to be changed to rotational quantities. These quantities are described and explained in detail in the following paragraphs.

### Moment of Inertia

In rotational motion the moment of inertia (usually denoted by $I$) takes the role of mass. An object with a large value of $I$ will be reluctant to change its rotational motion. Just as mass this quantity is a scalar, meaning that it has no direction. The moment of inertia of a system of objects can be determined easily by adding the moment of inertia of each of the different components making up the entire system. The moment of inertia depends not only on the mass of the object but also on how the mass is distributed with respect to the axis of rotation. The further the mass is away from the axis of rotation, the higher the moment of inertia will be. For a ***point mass*** (an object that can be considered small with respect to its distance from the axis of rotation) the moment of inertia is defined as

```{math}
:label: M08_rotation_Eq01
I = m\, R^{2}
```

where $m$ is the mass of the object and $R$ is the distance of the object from the axis of rotation. 

The calculation of the moment of inertia for more complex objects is a rather straightforward process, but can be very tedious. In most cases simple expressions can be found to calculate the value of $I$. The list below gives the moment of inertia for a few objects used in this lab:

- **Multiple point masses** of mass $M_{i}$ and radius $R_{i}$ considered as a single object, the moment of inertia can be represented as the sum of $N$ point masses:

```{math}
:label: M08_rotation_Eq01_multi
I_\text{allPointMasses} = \sum_{i=1}^N I_i = \sum_{i=1}^N M_i\,R_i^{2}
```

- A **thin rod** of mass $M_{rod}$ and length $L_{rod}$ rotating about an axis through its center:

```{math}
:label: M08_rotation_Eq02_rod
I= \frac{1}{12} M_{rod} \, L_{rod}^{2}
```

- A **solid disk** of mass $M_{D}$ and radius $R_{D}$ rotating about an axis through its center:

```{math}
:label: M08_rotation_Eq02
I= \frac{1}{2} M_{D} \, R_{D}^{2}
```

- A **thin-walled ring** of mass $M_{R}$ and radius $R_{R}$ rotating about an axis through its center:

```{math}
:label: M08_rotation_Eq03
I= M_{R} \, R_{R}^{2}
```

- A **thick ring** mass $M_{R}$ and inner radius $R_{i}$ and outer radius $R_{o}$ rotating about an axis through its center:

```{math}
:label: M08_rotation_Eq04
I=\frac{1}{2} M_{R} \, \left(R_{i}^2 + R_{o}^2\right)
```

### Torque

A force by itself is not enough to determine whether an object will start to rotate (just think about how a force that is applied to the hinges of a door will not rotate the door). Instead we define a new quantity, called torque $\tau$, which combines the force and the distance from the axis of rotation (also called the lever arm). This quantity is a vector quantity, meaning that it does have a direction

```{math}
:label: M08_rotation_Eq05
\vec{\tau} = \vec{F}_{\perp} \times \vec{d}.
```

Here $\vec{d}$ denotes the lever arm (directed outward from the center) and $\vec{F}_{\perp}$ is the component of the force perpendicular to the lever arm.

### Newton's 2nd Law for Rotational Motion

With the above definitions we can now formulate a rotational version of Newton's 2nd Law. An object with moment of inertia $I$ will experience an angular acceleration $\vec{\alpha}$, if a net torque $\vec{\tau}_{\text{net}}$ acts on it

```{math}
:label: M08_rotation_Eq06
\vec{\tau}_{\text{net}} = I \vec{\alpha}.
```

### Calculating the Moment of Inertia

One can use Newton's 2nd Law for Rotational Motion to calculate the moment of inertia of an object from the angular acceleration $\alpha$ and the net torque acting on the object.

```{math}
I = \frac{\left|\vec{\tau}_{\text{net}}\right|}{\left|\vec{\alpha}\right|}
```

The simplified sketch in {numref}`M08_rotation_Fig01` shows the setup used in this lab.
The net torque acting on the pulley can be written as

```{math}
|\vec{\tau}_{\text{net}}| = T \, R_{P}
```

where $T$ is the tension in the string and $R_{P}$ is the radius of the 3-step pulley. Since the tension is not known it has to be determined from the linear acceleration a of the hanging mass, using the net force acting on the mass $m_\text{hanger}$ (see force diagram in the sketch):

```{math}
F_{\text{net}} = m_\text{hanger} g - T = m_\text{hanger} a.
```

In addition the linear acceleration $a$ is related to the angular acceleration $\alpha$ by

```{math}
a = \alpha R_{P}.
```

Using this set of equations one can now solve for the moment of inertia, $I$,

```{math}
:label: M08_rotation_Eq07
I = \frac{m_\text{hanger} \left(g  R_{P} - \alpha R_{P}^2\right)}{\alpha}.
```

```{figure} RotationalMotionFigures/Figure01_v2025_02.png
:name: M08_rotation_Fig01
:width: 60%
:align: center

Left: Sketch of a pulley of mass $M$ and radius $R$ being accelerated by a hanging mass $m_\text{hanger}$. Note that the pulley in the lab is actually horizontal, but is drawn vertically here for simplicity. Right: Force diagram for the hanging mass $m_\text{hanger}$.
```




### Angular Momentum

A similar derivation as above can be used to define the quantity of angular momentum $\vec{L}$ from the definition of linear momentum ($\vec{p} = m \vec{v}$)

```{math}
|L| = I \omega
```

Angular momentum is conserved (meaning it will not change its value) if there is no external torque acting on a system

```{math}
\vec{L}_i = {L}_f.
```

This can be used to determine the angular velocity of a system if the moment of inertia changes

```{math}
:label: M08_rotation_Eq08
I_i \omega_i = I_f \omega_f.
```

**THE PARALLEL AXIS THEOREM** is used to calculate the moment of inertia of an object of mass $M$ rotating about a rotation axis that does not pass through the center of mass (e.g. the ring on top of the apparatus is off center). The moment of inertia for the axis ${I_{axis}}$ is

```{math}
:label: M08_rotation_Eq09
{I_{axis}} = {I_{ring}} + M d_{cm}^2
```

where ${I_{cm}}$ is the moment of inertia about an axis through the center of mass parallel to the rotation axis. The distance between the parallel axes is ${d_{cm}}$. In the Conservation of Angular Momentum experiment you drop the ring on the rotating apparatus. Although you try to drop the ring centered on the axis of rotation, it often lands off center. You will run a case where you try to center it, and then another case where you purposefully drop it off center.


## Experimental Procedure

### Preliminary Setup
The lab today makes use of a rotary sensor, which is able to detect and measure angular displacement, angular velocity, and angular acceleration. This Rotary Motion Sensor (RMS), with a **stated uncertainty of 0.09°**, is attached to a vertical rod and has a 3-step pulley affixed to its axle (see {numref}`M08_rotation_Fig02`). Objects with different moments of inertia can be mounted onto the 3-step pulley and their rotational motion be measured. A second, black pulley (called a Super Pulley) is attached ***at an angle*** to the RMS to allow a string to spool off the 3-step pulley as shown in {numref}`M08_rotation_Fig02`. A weight hanger of known mass $m_\text{hanger}$ is attached to the free end of the string and provides an accelerating ***torque*** to the 3-step pulley and therefore to the object mounted on it.

The objects to be mounted are either a rod with point masses in {numref}`M08_rotation_Fig04` and a disk with an accompanying thick ring in {numref}`M08_rotation_Fig03`.

In this lab, you will run a ***Moment of Inertia*** experiment and an ***Angular Momentum*** experiment. You will first determine the angular acceleration from a graph of angular velocity vs. time using data recorded with the RMS. The data will be collected and analyzed in **Capstone**. The moment of inertia of both two point masses and a thick ring will be determined from those experimental angular acceleration values. Finally in the Angular Momentum experiment, you will verify the validity of angular momentum conservation in an inelastic collision, and consider the parallel axis theorem.

```{figure} RotationalMotionFigures/Figure02_v2025-01.png
:name: M08_rotation_Fig02
:width: 50%
:align: center

Rotary Motion Sensor (RMS) with 3-step pulley (transparent) and Super Pulley (black). Super pulley should be at an angle to ensure the thread lines up tangent to the 3-step pulley.
```


```{figure} RotationalMotionFigures/Figure04_v2025-03.png
:name: M08_rotation_Fig04
:width: 80%
:align: center

Sketch of the RMS apparatus setup for "point masses" on a rotating rod. Left) Just apparatus (i.e. rod), Right) total from the apparatus and point masses combined.
```

```{figure} RotationalMotionFigures/Figure03_v2025-01.png
:name: M08_rotation_Fig03
:width: 80%
:align: center

Experimental setup of the RMS apparatus with disk alone (left) and with disk and ring mounted (right). The setup varies slightly from the one used in the lab.
```


```{figure} RotationalMotionFigures/Figure07_v2025-01.png
:name: M08_rotation_Fig07
:width: 80%
:align: center

Experimental setup of the Conservation of Angular Momentum experiment with **collisions*: Left) Thick ring dropped on-axis, Right) Thick ring dropped off-axis.
```


### Part I$_\text{a}$ --- Moment of Inertia of **Two Point Masses**

```{admonition} OVERVIEW --- Moment of Inertia of Two Point Masses
:class: note
Determine the moment of inertia of the two point masses (denoted as *pointMassesOnly*) by running 3 trials of:
 - Determining the moment of inertia of the combined apparatus plus point masses (denoted as *pulleyRodPointMasses*) by measuring angular acceleration with a known torque in **Capstone**
 - Similarly determining the moment of inertia of the apparatus by itself (empty rod, no point masses, denoted as *pulleyRodOnly*)
```

- Create a *data table* to find $I_{\text{expected,pointMassesOnly}}$ including:
  - the masses $M_1$ and $M_2$
  - the radii $R_1$ and $R_2$
  - the expected moment of inertia of the point masses together $I_{\text{expected,pointMassesOnly}}$
- Create a *data table* to find $I_{\text{experimental,pointMassesOnly}}$ including:
  - the hanging mass $m_\text{hanger}$
  - the radius of the pulley $R_P$
  - the total experimental angular acceleration and moment of inertia of the apparatus with masses (pulleyRodPointMasses) 
  - the experimental angular acceleration and moment of inertia of just the apparatus (pulleyRodOnly) 
  - the experimental moment of inertia of just the point masses $I_{\text{experimental,pointMassesOnly}}$.
- Please call the lab instructor for assistance if not yet set up:
  - Mount the rod onto the pulley of the RMS by removing the screw, remounting the clear RMS pulley with the key/slot in the widest-at-top orientation (see {numref}`M08_rotation_Fig04`), and placing the rod onto the notches of the clear RMS pulley, then using the longer screw on the rod to tighten everything back together.
    ```{admonition} DO NOT FORCE THE PULLEY (it's slotted/keyed)
     :class: important
     - Be gentle when re-applying the clear RMS pulley to the RMS, the RMS axel has a slot that the clear pulley is keyed to slide into
     - **DO NOT FORCE IT**, that will break the pulley
    ```
- Determine the masses of the two brass weights (with screws) and note the result as $M_1$ and $M_2$ in your Data Table.
- Mount the masses into the end of the rod and fasten them with the screws. Measure the distance of the center of the masses from the center of the rod. Note the results as $R_1$ and $R_2$ in your Data Table.
- Calculate the expected moment of inertia of just the two points masses, using {eq}`M08_rotation_Eq01` and {eq}`M08_rotation_Eq01_multi` given in the Introduction. Note your result as $I_{\text{expected,pointMassesOnly}}$ in your Data Table.
- Note the mass of the hanger as $m_\text{hanger}$ in your Data Table.
- Using the calipers measure the radius $R_{P}$ of the middle pulley of the RMS and note your result in your data table. NOT THE EDGES, MAKE SURE THE CALIPER FITS IN THE GROOVE. THERE IS AN ADDITIONAL EMPTY CLEAR PULLY IN YOUR BOX YOU CAN MEASURE FOR EASE OF USE (and for the angular momentum lab later on).
- Wind the string, with the mass hanger attached, clockwise onto the middle pulley of the RMS. You need to make sure that the string is wound nicely onto the clear middle pulley of the RMS, leaves tangentially from the clear pulley straight in line with and over the black Super Pulley (reminder, see off angle orientation noted in {numref}`M08_rotation_Fig02`).
- Measure the angular acceleration of the whole system $\alpha_{\text{experimental,pulleyRodPointMasses}}$ (i.e. of the two masses plus the apparatus):
  1. Make sure that in **Capstone** you have a graph of angular velocity ($y$-axis) vs. time ($x$-axis) open; same plot as seen in {numref}`M08_rotation_Fig05`.
  2. Before releasing the mass hanger press the **Record** button on **Capstone**.
  3. Release the mass hanger and observe the recorded data points/graph.
  4. Press the **Record** button again right before the string is completely unwound from the pulley to stop recording any more data points.
  5. Discuss (among yourselves and with your instructor) the resulting graph before continuing.
  6. Using the **Fit** option in **Capstone**, fit a straight line (linear fit) to the data, in the region where the system is accelerating (highlight the data region in the graph you want to fit).
  7. The slope of this graph is the angular acceleration $\alpha_{\text{experimental,pulleyRodPointMasses}}$.
  8. Note your result in your Data Table.
- Calculate the moment of inertia of the apparatus plus the two point masses, using {eq}`M08_rotation_Eq07` given in the Introduction. Note your result as $I_{\text{experimental,pulleyRodPointMasses}}$ in your Data Table.
- Remove the two point masses from the apparatus and repeat the above steps to determine the moment of inertia of the apparatus without the two masses. Note the result as $I_{\text{experimental,pulleyRodOnly}}$ in your Data Table. Please note that you need to again discuss the collected data points/graph with your lab instructor.

    ```{admonition} Constant or Variable Angular Acceleration? Linear vs. Non-linear?
    :class: question
    Notice that the rod turns quite fast and that the angular acceleration decreases as the speed increases (see plot in Capstone). Why does this happen?
    
    Discuss the collected data points/graph with your lab group and lab instructor
    ```

- To determine the moment of inertia of the two point masses subtract $I_{\text{experimental,pulleyRodOnly}}$ from $I_{\text{experimental,pulleyRodPointMasses}}$. Note your result as $I_{\text{experimental,pointMassesOnly}}$ in your Data Table.
- Repeat the above measurements for a total of 3 trials.
- Calculate averages and standard deviations $\sigma(I)$ for the moments of inertia.
- Compare the difference between your expected value and the experimental value with the standard deviation treated as your uncertainty range.


### Part I$_\text{b}$ --- Moment of Inertia of a **Thick Ring**

```{admonition} OVERVIEW --- Moment of Inertia of a Thick Ring
:class: note
Determine the moment of inertia of the ring (denoted as *ringOnly*) by running 3 trials of:
 - Determining the moment of inertia of the combined apparatus plus ring (denoted as *pulleyDiskRing*) by measuring angular acceleration with a known torque in **Capstone**
 - Similarly determining the moment of inertia of the apparatus by itself (disk only, no ring, denoted as *pulleyDiskOnly*)
```

- Create a *data table* to find $I_{\text{expected,ringOnly}}$ including:
    - the ring mass $M_{\text{ring}}$
    - the inner and outer radii of the ring ($R_i$, $R_o$)
    - the expected moment of inertia of the ring $I_{\text{expected,ringOnly}}$
- Create a *data table* to find $I_{\text{experimental,ringOnly}}$ including:
    - the hanging mass $m_\text{hanger}$
    - the radius of the pulley $R_P$
    - the experimental angular acceleration and moment of inertia with the apparatus with the ring (pulleyDiskRing)
    - the experimental angular acceleration and moment of inertia of just the apparatus (pulleyDiskOnly)
    - the experimental moment of inertia of the ring $I_{\text{experimental,ringOnly}}$
- Please call the lab instructor for assistance:
  - Mount the disk onto the pulley of the RMS by removing the screw and rod, flipping over and remounting the clear RMS pulley with the key/slot lined up and in the smallest-at-top orientation (see {numref}`M08_rotation_Fig02` & {numref}`M08_rotation_Fig03`), and placing the disk onto the square of the clear RMS pulley, then using the shorter screw to tighten everything back together.
    ```{admonition} DO NOT FORCE THE PULLEY (it's slotted/keyed)
     :class: important
     - Be gentle when re-applying the clear RMS pulley to the RMS, the RMS axel has a slot that the clear pulley is keyed to slide into
     - **DO NOT FORCE IT**, that will break the pulley
    ```
- Determine the mass of the ring and note the result as $M_{\text{ring}}$ in your data table.
- Measure and record the inner and outer radii of the ring, using the calipers. Note the result as $R_{i}$ and $R_{o}$ in your data table.
- Calculate the expected moment of inertia of the ring, using {eq}`M08_rotation_Eq04` given in the Background. Note your result as $I_{\text{expected,ringOnly}}$ in your data table.
- Place the ring onto the disk, which should already be mounted on the Rotary Motion Sensor (RMS). The two pins of the ring should fit into the two holes on the disk.
- Note the mass of the hanger as $m_\text{hanger}$ in your Data Table.
- Note the radius $R_{P}$ of the middle pulley of the RMS in your Data Table (use the result from the previous case).
- Wind the string, with the mass hanger attached, clockwise onto the middle pulley of the RMS. You need to make sure that the string is wound nicely onto the clear middle pulley of the RMS, leaves tangentially from the clear pulley straight in line with and over the black Super Pulley (reminder, see off angle orientation noted in {numref}`M08_rotation_Fig02`).
- Measure the angular acceleration $\alpha_{\text{total,ring}}$ of the ring plus the apparatus (i.e. the disk and the RMS).
  1. Make sure that in **Capstone** you have a graph of angular velocity ($y$-axis) vs. time ($x$-axis) open.
  ```{figure} RotationalMotionFigures/Figure05_v2025-02.png
  :name: M08_rotation_Fig05
  :width: 80%
  :align: center

  Example of Page 1 in today's **Capstone** file for both ring and point mass moment of inertia cases. Review notes in the text box to assist in your data taking and analysis.
  ```
  2. Before releasing the mass hanger press the **Record** button on **Capstone**.
  3. Release the mass hanger and note that the recorded graph is a straight line.
  4. Press the **Record** button again right before the string is completely unwound from the pulley to stop recording any more data points.
  5. Using the **Fit** option in **Capstone**, fit a straight line (linear fit) to the data, in the region where the system is accelerating (highlight the data region in the graph you want to fit).
  6. The slope of this graph is the angular acceleration $\alpha_{\text{total,ring}}$.
  7. Note your result in your Data Table.
- Calculate the moment of inertia of the apparatus plus the ring, using {eq}`M08_rotation_Eq07` given in the Introduction. Note your result as $I_{\text{total,ring}}$ in your data table.
- Remove the ring from the apparatus and repeat the above steps to determine the moment of inertia of the apparatus without the ring. Note the results as $\alpha_{\text{apparatus,ring}}$ and $I_{\text{apparatus,ring}}$ in your Data Table.
- To determine the moment of inertia of the ring, subtract $I_{\text{apparatus,ring}}$ from $I_{\text{total,ring}}$. Note your result as $I_{\text{experimental,ringOnly}}$ in your Data Table.
- Repeat the above measurements for a total of 3 trials.
- Calculate averages and standard deviations $\sigma(I)$ for the moments of inertia.
- Compare the difference between your expected value and the experimental value with the standard deviation treated as your uncertainty range.



### Part II --- Conservation of Angular Momentum

```{admonition} OVERVIEW --- Conservation of Angular Momentum
:class: note
Confirm conservation of angular momentum by: 
  - Determining the change in angular velocity and moment of inertia

Investigate the Parallel Axis Theorem by:
  - Accounting for an object whose center of mass is not aligned with the axis of rotaion.
  - Determining the change in angular velocity and moment of inertia
```

- Create a *common data table* including $I_{\text{apparatus,ring}}$ and $I_{\text{total,ring}}$.
- Create a *data table* with a row for each trial including
  - the initial angular velocity, $\omega_i$,
  - the final angular velocity, $\omega_f$,
  - the initial angular momentum, $L_i$,
  - the final angular momentum, $L_f$,
  - the change in angular momentum, $\Delta L$.
- Please call the lab instructor for assistance:
  1. Change out the current clear RMS pulley (with a string and hanging mass) for the empty RMS pulley.
  2. Mount the disk onto the empty RMS pulley.
    ```{admonition} DO NOT FORCE THE PULLEY (it's slotted/keyed)
    :class: important
    - Be gentle when re-applying the clear RMS pulley to the RMS, the RMS axel has a slot that the clear pulley is keyed to slide into
    - **DO NOT FORCE IT**, that will break the pulley
    ```
- Copy your experimental value for the moment of inertia of the apparatus $I_{\text{apparatus,ring}}$ (i.e. just the disk) from the first experiment for use here (reminder, you can easily reference cells in Excel).
- Copy your experimental value for the moment of inertia of the ring plus apparatus $I_{\text{total,ring}}$ from the first experiment.
- Hold the ring with the pins facing up just above the center of the disk.
- **Practice** the drop a few times before continuing:
  1. Give the disk a quick spin with your hand.
  2. Hold the ring a few millimeters above the spinning disk centered on the axis of the disk.
  3. Drop the ring onto the spinning disk, so that the ring is centered on the disk (see {numref}`M08_rotation_Fig07`-left).
- Measure the angular speeds $\omega_{i}$ and $\omega_{f}$ (before and after dropping the ring onto the disk):
  1. Switch to page 2 in your **Capstone** file. You shouce have a graph of angular position ($y$-axis) vs. time ($x$-axis); see {numref}`M08_rotation_Fig06`.
    ```{figure} RotationalMotionFigures/Figure06_v2025-03.png
    :name: M08_rotation_Fig06
    :width: 80%
    :align: center

    Example of Page 2 in today's **Capstone** file for the angular momentum experiment. Review notes in the text box to assist in your data taking and analysis. Note the region in the plot *before* and *after* the collision.
    ```
  2. Press the **Record** button in **Capstone**.
  3. Give the disk a spin with your hand and notice the angular position change.
  4. Ensure you've recorded a few seconds of data, then drop the ring as centered as you can onto the disk.
  5. Press the **Stop** button after collecting a few more seconds of data.
  6. Using the **Highlight Data** tool, highlight first the data region immediately before the collision; $\sim 0.5\,\text{seconds}$.
  7. Using the **Curve Fit** tool, fit a straight line (linear fit) to that highlighted data, and record the slope as initial angular velocity $\omega_i$.
  8. Shift your data hightlight box to immediately after the collision; again covering $\sim 0.5\,\text{seconds}$.
  9. The curve fit should update, and you can record the slope as final angular velocity $\omega_f$.
- Calculate the angular momentum of the appartus before the ring is dropped onto the disk. Note your result as $L_i$ in your Data Table.
- Calculate the angular momentum of the disk-plus-ring system after the ring is dropped onto the disk. Note your result as $L_f$ in your Data Table.
- Compare the difference between your expected value and the experimental value, also compare with a percent difference.

    ```{admonition} Discussion Point: Conserved?
    :class: question
    - Is angular momentum $L$ conserved? 
    - What might cause any discrepancies in the conservation of angular momentum?
    ```

- Parallel Axis Theorem test:
  - Run an additional test of the angular momentum part where you drop the ring to purposefully be off center (see {numref}`M08_rotation_Fig07`-right).
  - Measure the off-center distance ${d_{cm}}$ when the ring is all the way against the main axis of rotation of the metal plate (i.e. inner edge of the ring against the screw).
  - Calculate the updated moment of inertia of the ring using the parallel axis theorem, {eq}`M08_rotation_Eq09`.
  - Spin the disk as fast as possible and drop the ring off center to the point where it ends up against the screw, akin to what you just measured for ${d_{cm}}$.
  - Record both the initial and final angular velocities.
  - Calculate both the initial and final angular momentum.

    ```{admonition} Discussion Point: Off-axis
    :class: question
    - What is the effect of dropping the ring off-center?
    - Is $L$ conserved when considering the off-axis portion?
    ```


14. ***BEFORE CLOSING CAPSTONE:***
    ```{admonition} Photo of Experimental Data
    :class: important
    Ensure you've taken a screenshot/photo of your graphs for your spreadsheet submission:
      - Moment of Inertia:
        - 1 plot of Angular Velocity vs. Time for disk (apparatus)
        - 1 plot of Angular Velocity vs. Time for disk plus thick black ring (total)
        - 1 plot of Angular Velocity vs. Time for empty rod (apparatus)
        - 1 plot of Angular Velocity vs. Time for empty rod plus point masses (total)
      - Angular Momentum:
        - 1 plot of Angular Position vs. Time showing changing slope before and after collision (dropping of ring)
    ```


15. ***BEFORE LEAVING LAB:***
    ```{admonition} ✨🧹 PLEASE CLEAN UP & RETURN LAB TO ORIGINAL STATE 🧹✨
    :class: important
    - Remount the rod with the clear pulley with string and hanging mass for the first experiment.
    - Put away all the other parts in the provided box.
    - Close, **DO NOT SAVE**, the Capstone file you used today.
    - Don't leave a mess, leave it better than you found it, thank you.
    ```



## Post-Lab Submission --- Interpretation of Results

This week's lab is built of essentially two different, but still related to rotational motion, experiments. To assist in your analysis and writeups, the suggested talking points below are broken up into the Moment of Inertia and Angular Momentum parts of the lab. You will still have single document for error analysis and single document for results as assignments in Blackboard.

  ### Finalized Spreadsheets
  - Make sure to submit your finalized data table (Excel sheet).
    - Please include relevant screenshots of your Capstone plots including:
      - Moment of Inertia:
        - 1 plot of Angular Velocity vs. Time for disk (apparatus)
        - 1 plot of Angular Velocity vs. Time for disk plus thick black ring (total)
        - 1 plot of Angular Velocity vs. Time for empty rod (apparatus)
        - 1 plot of Angular Velocity vs. Time for empty rod plus point masses (total)
      - Angular Momentum:
        - 1 plot of Angular Position vs. Time showing changing slope before and after collision (dropping of ring)

  ### Moment of Inertia Post-Lab
  - In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
	  - What are your measurement uncertainties for each experiment?
	  - What are possible systematic uncertainties for each experiment?
    - How do these uncertainties affect your final results for $I$?
  - In a **paragraph**, summarize the results you have determined in each case. Consider:
	  - Part 1: How do the values of both the **ring's** and **two-point masses'** measured $I$ compare to the “predicted (from geometry)” value? Treating your standard deviations as your uncertainty, do your results span the difference between experimental and theoretical, thereby agreeing?
	  - Part 1 (empty rod): In the part of the experiment measuring the moment of inertia of the rod apparatus without the weights, notice that the rod turns quite fast and that the angular acceleration decreases as the speed increases (see plot in **Capstone**). Why does this happen?


  ### Angular Momentum Post-Lab
  - In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
	  - What are your measurement uncertainties for each experiment?
	  - What are possible systematic uncertainties for each experiment?
    - How do these uncertainties affect your final results for $L$?
  - In a **paragraph**, summarize the results you have determined in each case. Consider:
	  - Part 2: Is angular momentum $L$ conserved? What might cause any discrepancies in the conservation of angular momentum?
  	- Part 2: What is the effect of dropping the ring off-center? Is $L$ conserved when considering the off-axis portion?


## The Whiteboard

```{figure} RotationalMotionFigures/RotationalDynamics_2024_Fall_01.jpg
:name: rot1
:width: 100%
:align: center

```


