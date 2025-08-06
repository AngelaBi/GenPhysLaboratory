# Force Table with 3 Vectors at Equilibrium

## Background

```{admonition} OVERALL GOALS
:class: note
Use a "force table" to study:
- how vectors are added
- the concept of force vectors in equilibrium
```


There are two types of physical quantities: ***scalars*** and ***vectors***. The number of attributes required to define a scalar and a vector distinguishes them. A ***scalar*** has just a **magnitude** telling us how large or small something is (or positive or negative); an example of a scalar quantity is temperature or speed (m/s)

A ***vector***, meanwhile, is a quantity that is described by both a **magnitude** ***and*** **direction**. Examples of vectors are velocity (speed but with a direction; m/s at some angle) or force (a push or pull on an object with a specific magnitude at some direction).

A force example: a force may be 100 N in magnitude with direction 90° counterclockwise from the $x$-axis. This force vector is written as 100 N @ 90°. We will use bold face type to indicate a vector ($\vec{F_i}$) while the regular typeface will indicate scalar magnitudes and the components of a vector ($F_i$).

When several vectors act on an object, it is generally desirable to determine the sum of these vectors, called the **resultant vector**. Suppose force vectors $\vec{F}_1$ and $\vec{F}_2$ act on a body. The resultant $\vec{R}$ is defined by the vector sum of the two forces, thus

```{math}
:label: eq-M01-resultant-two-forces
\vec{R} = \vec{F}_1 + \vec{F}_2.
```

If many forces act on the body, then we sum all the forces together

```{math}
:label: eq-M01-resultant-sum
\vec{R} = \sum_{i=1}^N \vec{F}_i.
```
The resultant force is a single force which can completely represent a number of individual forces acting. When the resultant force is zero, the object is said to be in equilibrium.

There are two methods of vector addition to consider:

- The graphical method (reviewed here, but not conducted during lab today)
- The method of components (conducted during lab today)

### Graphical Method

Vectors $\vec{F}_1$ and $\vec{F}_2$ ({numref}`M01Fig01`) are added graphically as follows:
Beginning at a convenient point on a piece of graph paper, usually at the origin of a rectangular coordinate system draw one of the vectors as an arrow to scale and pointing in the proper direction. Place the second vector with its tail at the tip of the first, again drawn to scale and pointing in the proper direction. The resultant $\vec{R}$ is the vector drawn from the tail of the first vector to the tip of the second. The process is illustrated in {numref}`M01Fig02` demonstrating the addition operation does not depend on the order of addition. Thus, like scalar addition,

```{math}
:label: eq-M01-vector-addition-commutative
\vec{F}_1 + \vec{F}_2 = \vec{F}_2 + \vec{F}_1 = \vec{R}.
```

```{figure} ExperimentVectorTableFigures/M1_ForceTable_01.jpg
:name: M01Fig01
:width: 300px
:align: center

Two force vectors $\vec{F}_1$ and $\vec{F}_2$
```

```{figure} ExperimentVectorTableFigures/M1_ForceTable_02.jpg
:name: M01Fig02
:width: 500px
:align: center

Adding 2 vectors $\vec{F}_1$ and $\vec{F}_2$, using the graphical ("tail-to-tip") method.
```

It is important that an appropriate scale be selected with which the vectors are drawn (e.g. 1 N = 10 cm). The magnitude of $\vec{R}$ is determined using a ruler, and the angle $\theta$ is measured using a protractor. Since the negative of a vector is merely the vector pointing in the opposite direction, subtraction is addition with the negative vector pointing in the opposite direction. Errors can be significantly reduced by using a scale that makes the drawing as large as possible. Neatness counts!

### Method of Components

The method of components is a much more useful and quantitatively accurate method of vector addition. Each vector is resolved into components along the $x$- and $y$-axes. That is to say, the vector addition of the two components of the vector is the vector itself. Thus if two vectors are to be added, we add the components along each axis to form the components of the resultant.

```{figure} ExperimentVectorTableFigures/M1_ForceTable_03.jpg
:name: M01Fig03
:width: 500px
:align: center

Adding 2 vectors $\vec{F}_1$ and $\vec{F}_2$ using the method of components.
```

In {numref}`M01Fig03`, the magnitudes and directions are shown for the two force vectors $\vec{F}_1$ and $\vec{F}_2$. The magnitudes of the $x$ and $y$ components are calculated for this example as follows:

```{math}
:label: eq-M01-cosSinAngle
\begin{aligned}
F_{1,x} &= F_1 \, \cos(\theta_{1}) & \qquad F_{2,x} &= F_2 \, \cos(\theta_{2}) \\
        &= 1\,\text{N} \cos(0°) = 1\,\text{N} & &= 1\,\text{N} \cos(45°) = 0.707\,\text{N} \\
F_{1,y} &= F_1 \,\sin(\theta_1) & \qquad F_{2,y} &= F_2 \,\sin(\theta_2) \\
        &= 1\,\text{N} \sin(0°) = 0\,\text{N} & &= 1\,\text{N} \sin(45°) = 0.707\,\text{N}.
\end{aligned}
```

Next, add the $x$-components

$$\vec{R}_x = F_{1,x} + F_{2,x} = 1\,\text{N} + 0.707\,\text{N} = 1.707\,\text{N}.$$

Then, add the $y$-components

$$\vec{R}_y = F_{1,y} + F_{2,y} = 0\,\text{N} + 0.707\,\text{N} = 0.707\,\text{N}.$$

The magnitude of the resultant is found using the relation

```{math}
:label: eq-M01-resultantMag
\vec{R}^2 = {\vec{R}_x}^2 + {\vec{R}_y}^2,
```

or

$$\vec{R} = \sqrt{\left(1.707\,\text{N}\right)^2 + \left(0.707\,\text{N}\right)^2} = 1.848\,\text{N}.$$

The angle $\theta$ specifies the direction of the resultant and it can be calculated by noting that

```{math}
:label: eq-M01-tan-theta
\tan\theta = R_{y} / R_{x}
```

and

```{math}
:label: eq-M01-arctan
\theta = \arctan (R_{y} / R_{x}).
```

For this example illustrated in {numref}`M01Fig04`

$$\tan \theta = (0.707\,\text{N}) / (1.707\,\text{N}) = 0.414,$$

$$\theta = \arctan(0.414) = 22.5°.$$

```{figure} ExperimentVectorTableFigures/Figure04.jpg
:name: M01Fig04
:width: 400px
:align: center

Example of $\vec{R}$, the sum of 2 vectors, illustrating $x$- and $y$-components, as well as its magnitude and angle with the $x$-axis.
```

In this laboratory, an object will be presented with two known forces acting on it. Equilibrium will be established by adding a third **equilibrant** force $\vec{F}_3$, such that the sum of the three forces is zero (at equilibrium). Thus, we must find the resultant $\vec{R}$ of the two given forces $\vec{F}_1$ and $\vec{F}_2$, and find the force $\vec{F}_3 = -\vec{R}$ --- equal in magnitude and opposite in direction to the resultant $\vec{R}$ of $\vec{F}_1$ and $\vec{F}_2$. This is illustrated in {numref}`M01Fig05`.

```{figure} ExperimentVectorTableFigures/Figure05.jpg
:name: M01Fig05
:width: 400px
:align: center

Illustration of the method to determine the force $\vec{F}_{3}$ needed to balance two given forces $\vec{F}_{1}$ and $\vec{F}_{2}$.
```

Here $\vec{F}_3$ is the equilibrant force necessary to equilibrate $\vec{F}_1$ and $\vec{F}_2$. Note that, the resultant of $\vec{F}_1+\vec{F}_2+\vec{F}_3$ is zero since the ring is in equilibrium.

Force $\vec{F}_3$ has the same magnitude as the resultant $\vec{R}$, but acts in a direction opposite to $\vec{R}$ (recall that $\vec{R}=\vec{F}_1+\vec{F}_2$). So we now have

```{math}
:label: eq-M01-equilibrant
\vec{F}_3 = -\vec{R}.
```
We conclude that the force necessary to equilibrate two or more forces is equal and opposite to the resultant of the two (or more) forces. This is additionally illustrated in an example of the force table apparatus we will use in {numref}`M01Fig06`.

## Apparatus

```{figure} ExperimentVectorTableFigures/M1_ForceTable_06_table.jpg
:name: M01Fig06
:width: 500px
:align: center

Illustration of the force table, and an example of how to determine the force $\vec{F}_{3}$ needed to balance two given forces $\vec{F}_{1}$ and $\vec{F}_{2}$.
```

The apparatus for this experiment consist of a force table, weight holders, and weights (see {numref}`M01Fig06`). The force table consists of a circular tabletop mounted on a vertical rod held in a tripod support with leveling screws. The rim of the circular top has a 360° scale engraved on it along which it is possible to clamp a number of pulleys. At the center of the table is a small ring held in place by means of a removable pin. The ends of three cords are tied to the ring with each cord leading over a pulley and ending with a weight holder tied to its other end. When the forces along the cords acting upon the small ring are balanced, or in static equilibrium, the ring remains stationary. For this lab, the force pulling on the ring is the tension of the string, which is merely translated from horizontal on the table to vertical.

Each hanging mass has an associated weight (force) due to being pulled *down* by gravity. This weight is balanced by the *upward* tension force of the vertical part of the cord which is merely translated from vertical to horizontal tension by the pulley. Thus, the force pulling the ring in the direction of the cord is

```{math}
:label: eq-M01-ForceG
\vec{F}_\text{weight} = m \cdot \vec{g} = \vec{F}_\text{tension}
```

For accurate measurements of the angles involved, each cord must be aimed directly at the peg at the center of the ring requiring that the equilibrium condition must be established when the ring is exactly centered around the pin on the table.



## Experimental Procedure

### Preview

For today's lab, two different cases will be assigned involving two given vectors and the **determination of the equilibrant vector**. A third case involves the **determination of the mass of two unlabeled masses** by balancing the system from a single known mass.

#### Finding the Equilibrant (First two cases)

For each of the first two cases, you will have two given masses at given angles (direction). Each mass, consisting of a 50 g hanger plus the necessary additional mass, will be hung from a cord routed over a pulley at the assigned angular positions and finally tied to the ring. A third cord, hanger, and pulley assembly is put in place for the third, unknown force vector. Each force is the weight of the hanging mass at the pulley angle. Determine the unknown forces for each of the two cases.

If, for example, you are given the following case to work with

$$\begin{array}{rll}
\text{Mass #1:} & 200\,\text{g} & \text{@}\,0° \\
\text{Mass #2:} & 250\,\text{g} & \text{@}\,135°.
\end{array}$$

Place a pulley at 0° and add 150 g to the 50 g weight hanger for a total 200 g. As mentioned in {eq}`eq-M01-ForceG`, the tension on the cord is the same on both sides of the pulley so that the downward pull of gravity on the hanger and masses is equal to the tension in the cord leading to the ring. Thus,

$$F_1 = m g = 0.20\,\text{kg} \times 9.8\,\text{m/s}^2 = 1.96\,\text{N} \text{ @ } 0°.$$

Similarly, add 200 g to a 50 g weight hanger and run its cord over a pulley mounted at 135°.

$$F_2 = m g = 0.25\,\text{kg} \times 9.8\,\text{m/s}^2 = 2.45\,\text{N} \text{ @ } 135°.$$

Having established the given magnitudes and directions for each of the given forces, $\vec{F}_{1}$ and $\vec{F}_{2}$, adjust both the amount of mass hanging on cord 3 and its angular position so that the ring is stationary at the center of the table. In order for angular measurements to be accurate, **each cord must be on a line that crosses through the center of the table**. Sighting *along* each cord towards the center pin can help you to easily and accurately check this.

To determine the equilibrant vector $\vec{F}_{3}$, you will record both the angular position (**direction**) and total mass (to determine **magnitude** of the balancing force from the total hanging weight) required to balance $\vec{F}_{1}$ and $\vec{F}_{2}$.

#### Determining 2 Unlabeled Masses (Third case)

In this case, you will experimentally **determine two unlabeled masses** by balancing the $x$ and $y$ components of the force of a known mass.
Place the pulley with the known mass $M_1 = 50\,\text{g}$ at $\theta_1 = 0°$.
Experimentally determine the angles $\theta_2$ and $\theta_3$ for the unlabeled masses $M_2$ and $M_3$ that result in the ring being in equilibrium. For this case, **assume angles $\theta_2$ and $\theta_3$ are actual values**.

We can calculate the theoretical unlabeled masses using the method of components.
You have to solve a pair of equations for the $x$ and $y$ components of force.
The equation for equilibrium in the $x$ direction is

```{math}
:label: eq-M01-unknownx
(M_1 + M_2 \cos\theta_2 + M_3 \cos\theta_3)g = 0.
```

The equation for equilibrium in the $y$ direction is

```{math}
:label: eq-M01-unknowny
(M_2 \sin\theta_2 + M_3 \sin\theta_3)g = 0.
```

$M_2$ is eliminated by multiplying the $x$ component by $\sin \theta_2$ and subtracting the $y$ component multiplied by $\cos \theta_2$

```{math}
:label: eq-M01-solveM3
M_1 \sin \theta_2  + M_3 \cos \theta_3 \sin \theta_2 - M_3 \sin \theta_3 \cos \theta_2 = 0.
```

Using the known values, solve for $M_3$ and enter the value in the table.

Similarly, eliminating $M_3$ gives

```{math}
:label: eq-M01-solveM2
M_1 \sin \theta_3  + M_2 \cos \theta_2 \sin \theta_3 - M_2 \sin \theta_2 \cos \theta_3 = 0.
```
Using the known values, solve for $M_2$ and enter the value in the table.

Measure $M_2$ and $M_3$ on the scale and enter the values in the table.

It is good practice to **COMPLETE THE ANALYSIS OF THE FIRST CASE BEFORE CONTINUING TO THE NEXT CASE**. If you have some error in your experimental method or in your calculation, you can correct it before completing all the other cases. The layout of the data table for additional cases can then be created by copying the first case after you are confident in your results from the first case.

### CASE 1 & 2 -- Finding the Equilibrant Vector (Balancing Force)

```{admonition} OVERVIEW
:class: note
- Understand how to add and balance vectors using the **method of components**.
- Conduct 3 cases of two additive, known vectors (weights at given angles) to experimentally determine the third balancing or equilibrant vector.
- Compare the experimental results to theoretically expected vectors.
- **Assume** 0° is the +x direction, 90° is the +y direction
```
2. The first two cases are:

   **Case 1:**
   - hanger 1: 150 g @ 0°
   - hanger 2: 150 g @ 70°
   - hanger 3: ? kg @ ?°

   **Case 2:**
   - hanger 1: 100 g @ 75°
   - hanger 2: 200 g @ 115°
   - hanger 3: ? kg @ ?°

3. Create a data table for the first case. NOTE: The data layout for each of the first two cases is the same. Create for the first case and run the whole experiment, then you can copy/paste the same data table for the additional case(s).
   - Common data section with accepted value of $g$ (9.803 m/s²), mass of the hanger, and any other common values. You will reference these values in the calculations.
   - With **three rows** (1 for each of the 3 vectors).
   - Include **columns** for:
     - $m_i$: hanging mass in kilograms (kg)
     - $\delta m_i$: your estimate of the experimental uncertainty [± value] of the mass
     - $F_i$: calculated magnitude of the force in Newtons (N) (see {eq}`eq-M01-ForceG`)
     - $\theta_i$: direction of the force vector in degrees
     - $\delta \theta_i$: your estimate of the experimental uncertainty of the angle
     - $F_{i,x}$: calculated $x$-component of the force vectors (see {eq}`eq-M01-cosSinAngle`). Reminder, Excel needs angles in radians (use RADIANS() function to convert)
     - $F_{i,y}$: calculated $y$-component of the force vectors
   - Create a secondary table to analyze the results of your measurements. This is effectively one row as there would be just a single value for each of the variables. The columns should include variables:
     - $\vec{R}_x$ & $\vec{R}_y$: the $x$ and $y$ components of the resultant vector $\vec{R}$ of the two given force vectors $\vec{F}_1$ and $\vec{F}_2$
     - $\vec{R}_\text{mag}$: magnitude of the resultant force vector in Newtons (see Pythagorean Theorem in {eq}`eq-M01-resultantMag`)
     - $\theta_{R}$: direction of the resultant in degrees (see {eq}`eq-M01-arctan` which stems from trigonometry). Use ATAN2() Excel function to get angle as measured counterclockwise from 0°. Reminder, Excel returns angles in radians (use DEGREES() function to convert)
     - $\vec{F}_{x,\text{total experimental}}$ & $\vec{F}_{y,\text{total experimental}}$: the vector components of the measured total force, which is the vector sum of $\vec{R}$ and $\vec{F}_3$
     - $\vec{F}_{\text{mag,total experimental}}$ (a.k.a. $\delta \vec{F}_3$): the magnitude of the total force, determined in similar fashion to {eq}`eq-M01-resultantMag`, but with $\vec{F}_{x,\text{total experimental}}$ & $\vec{F}_{y,\text{total experimental}}$. ***Consider***: The **total force should be zero** because the ring is in equilibrium. The magnitude of the total force is therefore a measure of the *experimental uncertainty*. This effectively represents $\delta \vec{F}_3$ where your experimental result would be $\vec{F}_3 \pm \delta \vec{F}_3$.
     - Based on your determined resultant $\vec{R}$
       - $\vec{F}_{3,\text{theoretical}}$: your expected or theoretical magnitude of the equilibrant force in N
       - $m_{3,\text{theoretical}}$: theoretical equilibrant mass in kg
       - $\theta_{3,\text{theoretical}}$: theoretical equilibrant direction in deg. (e.g. $\theta_{R} + 180°$)

4. Starting with the first case, place the respective masses on their hangers 1 & 2

5. Unscrew the black pulleys to rotate them around the tabletop to their given angles

6. With hanger 3, add or subtract masses and scoot the pulley around the table until the ring is as perfectly centered around the center pin as possible to argue equilibrium

7. Note your $m_3$ & $\theta_3$ values. Also note your estimated uncertainties $\delta m_i$ & $\delta \theta_i$

8. Derive the hangers' respective forces (e.g. {eq}`eq-M01-ForceG`)

9. Determine the hangers' respective $x$ and $y$ components

10. Determine the resultant $\vec{R}$ from your derived values for $\vec{R}_x$, $\vec{R}_y$

11. Determine the resultant's angle $\theta_R$

12. COMPARE your experimental results of hanger 3 to the theoretical values. Does $\vec{F}_3 \pm \delta \vec{F}_3$ overlap (and therefore agree) with your theoretical value $\vec{F}_{3,\text{theoretical}}$? If not, are there significant issues that may be contributing to the discrepancy? Discuss with instructor if so. To be further discussed in Section {ref}`interpretation`

13. Repeat for the second case

### CASE 3 -- Determining 2 Unlabeled Masses

```{admonition} OVERVIEW
:class: note
- Understand how to determine two unknown values of a 3 vector system using the **method of components**.
- *CONSIDER*: Each vector has two pieces of information, **magnitude** and **direction** --- how many pieces of information total do we have to work from?
- Determine the masses of two figurines (one is a black Pikachu, the other is a white corgi that can each sit on their respective hangers) by balancing the force vectors. Treat Pikachu-black as $m_2$ and the corgi-white as $m_3$.
- Compare the experimental results to actual masses as measured with a triple-beam balance.
- **Assume** the angles for both Pikachu and the corgi, once found, are treated as given values (so you only have two unknowns with two equations).
```

2. The third case is:
   - hanger 1: 50 g @ 0°
   - hanger 2 (Pikachu-black): ? kg @ ?° (angle treated as given once determined)
   - hanger 3 (corgi-white): ? kg @ ?° (angle treated as given once determined)

3. Create a data table for this case:
   - Common data section with the accepted value of $g$ (9.803 m/s²), the mass of the hanger, actual values of the figurines to be determined later, and any other common values.
   - $m_1$: Given mass will be just the hanger, so 50 g (but record in kg)
   - $\theta_1$: Angle of 0° for the empty hanger
   - $\vec{F}_{x,1}$ & $\vec{F}_{y,1}$: $x$ and $y$ components of the known mass's force vector
   - $\theta_{2,\text{Pikachu-black}}$ & $\theta_{3,\text{corgi-white}}$: Experimentally determined direction of the force vector in degrees --- **treat as actual given values once you find equilibrium. You will use these to solve for the masses later.**
   - $m_{2,\text{Pikachu-black}}$ & $m_{3,\text{corgi-white}}$: the experimental values of $m_2$ and $m_3$ from {eq}`eq-M01-solveM3` and {eq}`eq-M01-solveM2`
   - $m_{2,\text{Pikachu-black, actual}}$ & $m_{3,\text{corgi-white, actual}}$: the values of $m_2$ and $m_3$ as measured on a triple-beam balance.
   - % Difference of $m_2$ and $m_3$ experimentally found values to the actual measured values (see {eq}`M1-PercentDiff` in Section {ref}`interpretation`).

4. Place the respective masses on there hangers, with $m_1$ set to 0°

5. Unscrew the black pulleys to rotate them around the tabletop until you find equilibrium. You are only changing the angles of $\theta_{2,\text{Pikachu-black}}$ & $\theta_{3,\text{corgi-white}}$. NO ADDITIONAL MASS IS REQUIRED.

6. Once you've found equilibrium, note the $\theta_{2,\text{Pikachu-black}}$ & $\theta_{3,\text{corgi-white}}$ values as actual values to use in later equations (i.e. as if they're given angles)

7. Determine $m_{2,\text{Pikachu-black}}$ & $m_{3,\text{corgi-white}}$ using {eq}`eq-M01-solveM3` and {eq}`eq-M01-solveM2`

8. Using a triple-beam balance, measure directly the actual mass of $m_{2,\text{Pikachu-black, actual}}$ & $m_{3,\text{corgi-white, actual}}$

9. COMPARE your experimental results of each of the unlabeled masses to their actual values. Calculate the % difference of $m_2$ and $m_3$ experimentally found values to the actual measured values. What may be contributing to a larger or smaller difference? To be further discussed in Section {ref}`interpretation`.

(interpreation)=
## Post-Lab Submission --- Interpretation of Results

- Make sure to submit your finalized data table (Excel sheet)
- What is a vector?
- Case 1 & 2 (Finding Equilibrant):
  - Looking at your experiment, why do the two given masses not add up to the third mass?
  - What are the uncertainties of Experiment 1?
  - What are your results, and how do they compare to the theoretical predictions?
    - In other words, for each of the first two cases, COMPARE your experimental results of hanger 3 to the theoretical values for hanger 3.
      - Does $\vec{F}_3 \pm \delta \vec{F}_3$ overlap (and therefore agree) with your theoretical value $\vec{F}_{3,\text{theoretical}}$?
      - Does $m_3 \pm \delta m_3$ overlap with your theoretical value $m_{3,\text{theoretical}}$?
      - Does $\theta_3 \pm \delta \theta_3$ overlap with your theoretical value $\theta_{3,\text{theoretical}}$?
  - How does adding a few grams (i.e. $m_3 + \delta m_3$) change your results for $\vec{F}_3$?
  - How does changing the angle (i.e. $\theta_3 \pm \delta \theta_3$) change your results $\vec{F}_3$?
- Case 3 (Unlabeled Masses):
  - How do your values for $m_\text{Pikachu-black}$ and $m_\text{corgi-white}$ compare to your actual values from the triple-beam-balance?
  - What is the percent difference between your experimentally determine masses and their actual measured values? Calculate the % difference in each of the masses using the following relation:

```{math}
:label: M1-PercentDiff
\text{% Difference} = \frac{\text{Experimental Value} - \text{Actual Value}}{\text{Actual Value}} \times 100\%.
```

  - What uncertainties might make this difference larger or smaller?
- What is the precision of your equipment (force table, masses, etc.)?
- What are possible systematic errors of the experiment?

## The Whiteboard
