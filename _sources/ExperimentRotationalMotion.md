# Rotational Dynamics with Moment of Inertia & Angular Momentum

## Background

The motion of an object can be divided into two, completely independent parts: the linear (translational) motion of the center of mass and the rotational motion of the object around an axis through the center of mass. The - Part 1: How do the values of both the **ring's** and **two-point masses'** measured I compare to the "predicted (from geometry)" value? Treating your standard deviations as your uncertainty, do your results span the difference between experimental and theoretical, thereby agreeing?inear motion is explained by Newton's 2nd Law of motion: a net force $F_{net}$ acting on an object of mass $m$ will cause the object to experience a linear acceleration $a$ given by

```{math}
F_{net} = m a.
```

Rotational motion can be described in a very similar manner, but the quantities involved need to be changed to rotational quantities. These quantities are described and explained in detail in the following paragraphs.

### Moment of Inertia

In rotational motion the moment of inertia (usually denoted by $I$) takes the role of mass. An object with a large value of $I$ will be reluctant to change its rotational motion. Just as mass this quantity is a scalar, meaning that it has no direction. The moment of inertia of a system of objects can be determined easily by adding the moment of inertia of each of the different components making up the entire system. The moment of inertia depends not only on the mass of the object but also on how the mass is distributed with respect to the axis of rotation. The further the mass is away from the axis of rotation, the higher the moment of inertia will be. For a point mass (an object that can be considered small with respect to its distance from the axis of rotation) the moment of inertia is defined as

```{math}
:label: M08_rotation_Eq01
I = m\, R^{2}
```

where $m$ is the mass of the object and $R$ is the distance of the object from the axis of rotation.
The calculation of the moment of inertia for more complex objects is a rather straightforward process, but can be very tedious. In most cases simple expressions can be found to calculate the value of $I$. The list below gives the moment of inertia for a few objects used in this lab:

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

With the above definitions we can now formulate a rotational version of Newton's 2nd Law. An object with moment of inertia $I$ will experience an angular acceleration $\vec{\alpha}$, if a net torque $\vec{\tau}_{\mbox{net}}$ acts on it

```{math}
:label: M08_rotation_Eq06
\vec{\tau}_{\mbox{net}} = I \vec{\alpha}.
```

### Calculating the Moment of Inertia

One can use Newton's 2nd Law for Rotational Motion to calculate the moment of inertia of an object from the angular acceleration $\alpha$ and the net torque acting on the object.

```{math}
I = \frac{\left|\vec{\tau}_{\mbox{net}}\right|}{\left|\vec{\alpha}\right|}
```

The simplified sketch in {numref}`M08_rotation_Fig01` shows the setup used in this lab.
The net torque acting on the pulley can be written as

```{math}
|\vec{\tau}_{\mbox{net}}| = T \, R_{P}
```

where $T$ is the tension in the string and $R_{P}$ is the radius of the 3-step pulley. Since the tension is not known it has to be determined from the linear acceleration a of the hanging mass, using the net force acting on the mass $m$ (see force diagram in the sketch):

```{math}
F_{\mbox{net}} = m g - T = m a.
```

In addition the linear acceleration $a$ is related to the angular acceleration $\alpha$ by

```{math}
a = \alpha R_{P}.
```

Using this set of equations one can now solve for the moment of inertia, $I$,

```{math}
:label: M08_rotation_Eq07
I = \frac{m \left(g  R_{P} - \alpha R_{P}^2\right)}{\alpha}.
```

```{figure} /ExperimentRotationalMotionFigures/Figure01.jpg
:name: M08_rotation_Fig01
:width: 60%
:align: center

Left: Sketch of a pulley of mass $M$ and radius $R$ being accelerated by a hanging mass $m$. Note that the pulley in the lab is actually horizontal, but is drawn vertically here for simplicity. Right: Force diagram for the hanging mass $m$.
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

The experiment makes use of a sensor, which is able to detect and measure angular displacement, angular velocity, and angular acceleration. This Rotary Motion Sensor (RMS), with a **stated uncertainty of 0.09°**, is attached to a vertical rod and has a 3-step pulley affixed to its axle (see {numref}`M08_rotation_Fig02`). Objects with different moment of inertia can be mounted onto the 3-step pulley and their rotational motion be measured. A second pulley (called a Super Pulley) is attached to the RMS to allow a string to spool off the 3-step pulley as shown in {numref}`M08_rotation_Fig02` and {numref}`M08_rotation_Fig03`. A weight hanger of known mass $m$ is attached to the free end of the string and provides an accelerating torque to the 3-step pulley and therefore to the object mounted on it.

In this experiment you will measure the angular acceleration from a graph of angular velocity vs. time using data recorded with the RMS. The data will be collected in **Capstone**, which also provides analysis tools. The moment of inertia of a ring and of two point masses will be determined from the angular acceleration. Finally, you will verify the validity of angular momentum conservation in an inelastic collision.

```{figure} /ExperimentRotationalMotionFigures/Figure02.jpg
:name: M08_rotation_Fig02
:width: 50%
:align: center

Rotary Motion Sensor (RMS) with 3-step pulley (transparent) and Super Pulley (black).
```

```{figure} /ExperimentRotationalMotionFigures/Figure03a.jpg
:name: M08_rotation_Fig03
:width: 80%
:align: center

Experimental setup of the RMS apparatus with disk alone (left) and with disk and ring mounted (right). The setup varies slightly from the one used in the lab.
```

### Moment of Inertia of the Ring

In Part 1 of the experiment you will measure the moment of inertia of the ring and of the apparatus by measuring angular acceleration with a known torque.

- Create a Part 1 Data Table for your measurements and calculations of the moment of inertia of the ring.
- Determine the mass of the ring and note the result as $M_{\mbox{ring}}$ in your Part 1 Data Table.
- Measure the inner and outer radii of the ring, using the calipers. Note the result as $R_{i}$ and $R_{o}$ in your Part 1 Data Table.
- Calculate the expected moment of inertia of the ring, using {eq}`M08_rotation_Eq04` given in the Background. Note your result as $I_{\mbox{calc}}$ in your Part 1 Data Table.
- Place the ring onto the disk, which should already be mounted on the Rotary Motion Sensor (RMS). The two pins of the ring should fit into the two holes on the disk.
- Note the mass of the hanger as $m$ in your Data Table.
- Using the calipers measure the radius $R_{P}$ of the smaller pulley of the RMS and note your result in your Part 1 Data Table.
- Wind the string with the attached mass hanger onto the smaller pulley of the RMS. You need to make sure that the string runs over the Super Pulley, is wound nicely onto the smaller pulley of the RMS, and is leaving the pulley of the RMS tangentially before it runs straight over the Super Pulley.
- Measure the angular acceleration $\alpha_{\mbox{total}}$ of the ring plus the apparatus (the disk and the RMS).
  1. Make sure that in **Capstone** you have a graph of angular velocity ($y$-axis) vs. time ($x$-axis) open.
  2. Before releasing the mass hanger press the **Record** button on **Capstone**.
  3. Release the mass hanger and note that the recorded graph is a straight line.
  4. Press the **Record** button again right before the string is completely unwound from the pulley to stop recording any more data points.
  5. Using the **Fit** option in **Capstone**, fit a straight line (linear fit) to the data, in the region where the system is accelerating (highlight the data region in the graph you want to fit).
  6. The slope of this graph is the angular acceleration $\alpha_{\mbox{total}}$.
  7. Note your result in your Data Table.
- Calculate the moment of inertia of the apparatus plus the ring, using {eq}`M08_rotation_Eq07` given in the Introduction. Note your result as $I_{\mbox{total}}$ in your Part 1 Data Table.
- Remove the ring from the apparatus and repeat the above steps to determine the moment of inertia of the apparatus without the ring. Note the results as $\alpha_{\mbox{app}}$ and $I_{\mbox{app}}$ in your Data Table.
- To determine the moment of inertia of the ring subtract $I_{\mbox{app}}$ from $I_{\mbox{total}}$. Note your result as $I_{\mbox{exp}}$ in your Data Table.
- Repeat the above measurements three times.
- Calculate averages and standard deviations $\sigma(I)$ for the moments of inertia.
- Compare the difference between your calculated value and the experimental value with its uncertainty.

### Moment of Inertia of Two Point Masses

In Part 2 of the experiment, you will measure the moment of inertia of two point masses on a rod.

- Create a Part 2 Data Table for your measurements and calculations of the moment of inertia of the point masses.
- Please call the lab instructor for this: Mount the rod onto the pulley of the RMS.
- Determine the masses of the two brass weights (with screws) and note the result as $M_1$ and $M_2$ in your Data Table.
- Mount the masses into the end of the rod and fasten them with the screws. Measure the distance of the center of the masses from the center of the rod. Note the results as $R_1$ and $R_2$ in your Data Table.
- Calculate the expected moment of inertia of the two points masses, using {eq}`M08_rotation_Eq01` given in the Introduction. Note your result as $I_{\mbox{calc}}$ in your Data Table.
- Note the mass of the hanger as $m$ in your Data Table.
- Note the radius $R_{P}$ of the smaller pulley of the RMS in your Data Table (use the result from Part 1 above).
- Wind the string with the attached mass hanger onto the smaller pulley of the RMS. You need to make sure that the string runs over the Super Pulley, is wound nicely onto the smaller pulley of the RMS, and is leaving the pulley of the RMS tangentially before it runs straight over the Super Pulley.
- Measure the angular acceleration $\alpha_{\mbox{total}}$ of the two masses plus the apparatus (the rod and the RMS):
  1. Make sure that in **Capstone** you have a graph of angular velocity ($y$-axis) vs. time ($x$-axis) open.
  2. Before releasing the mass hanger press the **Record** button on **Capstone**.
  3. Release the mass hanger and observe the recorded data points/graph.
  4. Press the **Record** button again right before the string is completely unwound from the pulley to stop recording any more data points.
  5. Discuss (among yourselves and with your instructor) the resulting graph before continuing.
  6. Using the **Fit** option in **Capstone**, fit a straight line (linear fit) to the data, in the region where the system is accelerating (highlight the data region in the graph you want to fit).
  7. The slope of this graph is the angular acceleration $\alpha_{\mbox{total}}$.
  8. Note your result in your Data Table.
- Calculate the moment of inertia of the apparatus plus the two point masses, using {eq}`M08_rotation_Eq07` given in the Introduction. Note your result as $I_{\mbox{total}}$ in your Data Table.
- Remove the two point masses from the apparatus and repeat the above steps to determine the moment of inertia of the apparatus without the two masses. Note the result as $I_{\mbox{app}}$ in your Data Table. Please note that you need to again discuss the collected data points/graph with your lab instructor.
- To determine the moment of inertia of the two point masses subtract $I_{\mbox{app}}$ from $I_{\mbox{total}}$. Note your result as $I_{\mbox{exp}}$ in your Data Table.
- Repeat the above measurements three times.
- Calculate averages and standard deviations $\sigma(I)$ for the moments of inertia.
- Compare the difference between your calculated value and the experimental value with its uncertainty.


### Conservation of Angular Momentum

In Part 3 of the experiment you will observe the conservation of angular momentum in an inelastic collision.

- Create a Part 3 Data Table for your measurements and calculations of the conservation of angular momentum.
- Please call the lab instructor for this: Mount the disk onto the pulley of the RMS.
- Copy the result of the moment of inertia of the ring ($I_{\mbox{ring}}$) from the Part 1 Data Table to your Part 3 Data Table.
- Copy the result of the moment of inertia of the apparatus, which includes the mounted disk ($I_{\mbox{app}}$) from the Part 1 Data Table your Part 3 Data Table.
- Hold the ring with the pins facing up just above the center of the disk.
- Practice the drop a few times before continuing:
  1. Give the disk a spin with your hand.
  2. Hold the ring a few millimeters above the spinning disk centered on the axis of the disk.
  3. Drop the ring onto the spinning disk, so that the ring is centered on the disk.
- Measure the angular speeds $\omega_{i}$ and $\omega_{f}$ (before and after dropping the ring onto the disk):
  1. Make sure that in **Capstone** you have two graphs of angular position ($y$-axis) vs. time ($x$-axis) and of angular velocity ($y$-axis) vs. time ($x$-axis) open.
  2. Make sure that in **Capstone** you have a data table of the angular velocity open.
  3. Give the disk a spin with your hand and press the **Record** button on **Capstone**, while still holding the ring above the (now spinning) disk.
  4. Record about 25 data points (about 2--3 seconds), then let the disk drop onto the disk.
  5. Press the **Record** button again after collecting about 25 more points (again about 2--3 seconds).
  6. Using the **Fit** option in **Capstone**, fit a straight line (linear fit) to the angular position vs. time graph, in the two data regions (highlight the data region in the graph you want to fit).
  7. The two slopes are the angular velocities $\omega_i$ and $\omega_f$.
  8. Discuss among yourselves and with your instructor why this will not be a good determination of the speeds $\omega_i$ and $\omega_f$.
  9. Among yourselves and with your instructor discuss a better way to determine the speeds (Hint: Think about the exact instant at which you need to determine the speeds). Explain why your new method is better than the one mentioned above.
  10. Note the final results for the speeds $\omega_i$ and $\omega_f$ in your Part 3 Data Table.
- Calculate the angular momentum of the disk-ring system before the ring is dropped onto the disk. Note your result as $L_i$ in your Data Table.
- Calculate the angular momentum of the disk-ring system after the ring is dropped onto the disk. Note your result as $L_f$ in your Data Table.
- Compare the difference between your calculated value and the experimental value with its uncertainty.

- Parallel Axis Theorem test:
  - Run an additional test of the angular momentum part where you drop the ring to purposefully be off center.
  - Measure the off-center distance ${d_{cm}}$ when the ring is all the way against the main axis of rotation of the metal plate (i.e. inner edge of the ring against the screw).
  - Calculate the updated moment of inertia of the ring using the parallel axis theorem, {eq}`M08_rotation_Eq09`.
  - Spin the disk as fast as possible and drop the ring off center to the point where it ends up against the screw, akin to what you just measured for ${d_{cm}}$.
  - Record both the initial and final angular velocities.
  - Calculate both the initial and final angular momentum.


\section{Data Analysis}
The first experiment determines the moment of inertia of the ring by measuring its angular acceleration.
\begin{itemize}
\item[$\triangleright$] Create a table to find $I_{\mbox{calc}}$ including
  \begin{itemize}
  \item the ring mass $M_{\mbox{ring}}$,
  \item the inner and outer radii of the ring,
  \item the calculated moment of inertia $I_{\mbox{calc}}$.
  \end{itemize}
\item[$\triangleright$] Create a table to find $I_{\mbox{exp}}$ including
  \begin{itemize}
  \item the hanging mass $m$,
  \item the radius of the pulley $R_P$,
  \item the angular acceleration and calculated moment of inertia with the ring and apparatus,
  \item the angular acceleration and calculated moment of inertia of the apparatus,
  \item the experimental moment of inertia of the ring $I_{\mbox{exp}}$.
  \end{itemize}
\end{itemize}

The second experiment determines the moment of inertia of a rod with two masses by measuring its angular acceleration.

- ▷ Create a table to find $I_{\mbox{calc}}$ including
  - the masses $M_1$ and $M_2$,
  - the radii $R_1$ and $R_2$,
  - the calculated moment of inertia of the masses $I_{\mbox{calc}}$.

- ▷ Create a table to find $I_{\mbox{exp}}$ including:
  - the hanging mass $m$,
  - the radius of the pulley $R_P$,
  - the angular acceleration and calculated moment of inertia of the apparatus (rod) and masses,
  - the angular acceleration and calculated moment of inertia of the apparatus,
  - the experimental moment of inertia of the masses $I_{\mbox{exp}}$.
The third experiment in this lab shows conservation of angular momentum by illustrating the change in angular velocity with an increase in moment of inertia.

- ▷ Create a table of common data $I_{\mbox{ring}}$ and $I_{\mbox{app}}$.
- ▷ Create a table with a row for each trial including
  - the initial angular velocity, $\omega_i$,
  - the final angular velocity, $\omega_f$,
  - the initial angular momentum, $L_i$,
  - the final angular momentum, $L_f$,
  - the change in angular momentum, $\Delta L$.


## Post-Lab Submission --- Interpretation of Results

- Make sure to submit your finalized data table (Excel sheet)
- Part 1: How do the values of both the \textbf{ring's} and \textbf{two-point masses'} measured I compare to the “predicted (from geometry)” value? Treating your standard deviations as your uncertainty, do your results span the difference between experimental and theoretical, thereby agreeing?
- Part 1 (empty rod): In the part of the experiment measuring the moment of inertia of the rod apparatus without the weights, notice that the rod turns quite fast and that the angular acceleration decreases as the speed increases (see plot in **Capstone**). Why does this happen?
- Part 2: Is angular momentum $L$ conserved? What might cause any discrepancies in the conservation of angular momentum?
- Part 2: What is the effect of dropping the ring off-center? Is L conserved when considering the off-axis portion?
- What are your measurement uncertainties for each experiment?
- What are possible systematic uncertainties for each experiment?




