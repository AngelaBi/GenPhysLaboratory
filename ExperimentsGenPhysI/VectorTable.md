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

A force vector example: a force may be 100 N in magnitude with direction 90° counterclockwise from the $x$-axis. This force vector is written as 100 N @ 90°. We will use typefont of (with a note that bold isn't always bold when viewing on some machines):

 - Vector --- bold, itallicised, with an arrow overhead --- $\vec{F_i}$
 - Scalar --- bold, itallicised with *no* arrow --- $m$
 - Vector component ---  bold, itallicised, with a subscript $x$ or $y$ --- $F_{i,x}$ or $F_{i,y}$

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

```{figure} VectorTableFigures/M1_ForceTable_01.jpg
:name: M01Fig01
:width: 50%
:align: center

Two force vectors $\vec{F}_1$ and $\vec{F}_2$
```

```{figure} VectorTableFigures/M1_ForceTable_02.jpg
:name: M01Fig02
:width: 90%
:align: center

Adding 2 vectors $\vec{F}_1$ and $\vec{F}_2$, using the graphical ("tail-to-tip") method.
```

It is important that an appropriate scale be selected with which the vectors are drawn (e.g. 1 N = 10 cm). The magnitude of $\vec{R}$ is determined using a ruler, and the angle $\theta$ is measured using a protractor. Since the negative of a vector is merely the vector pointing in the opposite direction, subtraction is addition with the negative vector pointing in the opposite direction. Errors can be significantly reduced by using a scale that makes the drawing as large as possible. Neatness counts!

### Method of Components

The method of components is a much more useful and quantitatively accurate method of vector addition. Each vector is resolved into components along the $x$- and $y$-axes. That is to say, the vector addition of the two components of the vector is the vector itself. Thus if two vectors are to be added, we add the components along each axis to form the components of the resultant.

```{figure} VectorTableFigures/M1_ForceTable_03.jpg
:name: M01Fig03
:width: 90%
:align: center

Adding 2 vectors $\vec{F}_1$ and $\vec{F}_2$ using the method of components.
```

In {numref}`M01Fig03`, the magnitudes and directions are shown for the two force vectors $\vec{F}_1$ and $\vec{F}_2$. The magnitudes of the $x$ and $y$ components are calculated for this example as follows:

```{math}
:label: eq-M01-cosSinAngle
\begin{aligned}
F_{1,x} &= \vec{F}_1 \, \cos(\theta_{1}) & \qquad F_{2,x} &= \vec{F}_2 \, \cos(\theta_{2}) \\
        &= 1\,\text{N} \cos(0°) = 1\,\text{N} & &= 1\,\text{N} \cos(45°) = 0.707\,\text{N} \\
F_{1,y} &= \vec{F}_1 \,\sin(\theta_1) & \qquad F_{2,y} &= \vec{F}_2 \,\sin(\theta_2) \\
        &= 1\,\text{N} \sin(0°) = 0\,\text{N} & &= 1\,\text{N} \sin(45°) = 0.707\,\text{N}.
\end{aligned}
```

Next, add the $x$-components

$$R_x = F_{1,x} + F_{2,x} = 1\,\text{N} + 0.707\,\text{N} = 1.707\,\text{N}.$$

Then, add the $y$-components

$$R_y = F_{1,y} + F_{2,y} = 0\,\text{N} + 0.707\,\text{N} = 0.707\,\text{N}.$$

The magnitude of the resultant is found using the relation

```{math}
:label: eq-M01-resultantMag
R^2 = {R_x}^2 + {R_y}^2,
```

or

$$R = \sqrt{\left(1.707\,\text{N}\right)^2 + \left(0.707\,\text{N}\right)^2} = 1.848\,\text{N}.$$

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

```{figure} VectorTableFigures/Figure04.jpg
:name: M01Fig04
:width: 70%
:align: center

Example of $\vec{R}$, the sum of 2 vectors as $x$- and $y$-components, as well as its magnitude and angle with the $x$-axis.
```

In this laboratory, an object will be presented with two known forces acting on it. Equilibrium will be established by adding a third **equilibrant** force $\vec{F}_3$, such that the sum of the three forces is zero (i.e. at equilibrium). Thus, we must first find the resultant $\vec{R}$ of the two given forces $\vec{F}_1$ and $\vec{F}_2$. Then we can determine the equilibrant, $\vec{F}_3 = -\vec{R}$, equal in magnitude and opposite in direction to the resultant $\vec{R}$. This is illustrated in {numref}`M01Fig05`.

```{figure} VectorTableFigures/Figure05.jpg
:name: M01Fig05
:width: 70%
:align: center

Illustration of the method to determine the force $\vec{F}_{3}$ needed to balance two given forces $\vec{F}_{1}$ and $\vec{F}_{2}$.
```

Here $\vec{F}_3$ is the equilibrant force necessary to equilibrate $\vec{F}_1$ and $\vec{F}_2$. Note that the resultant of all the vectors for today's lab should add up to zero, i.e.

```{math}
:label: eq-M01-allVectorsResultant
\vec{F}_{\text{total}} = \vec{F}_1+\vec{F}_2+\vec{F}_3 = 0
```

since the ring is in equilibrium.

Recall that $\vec{R}=\vec{F}_1+\vec{F}_2$, therefore the equilibrant force $\vec{F}_3$ has the same magnitude as the resultant $\vec{R}$, but acts in a direction opposite to $\vec{R}$. So we now have

```{math}
:label: eq-M01-equilibrant
\vec{F}_3 = -\vec{R}.
```
We conclude that the force necessary to equilibrate two or more forces is equal and opposite to the resultant of the two (or more) forces. This is additionally illustrated in an example of the force table apparatus we will use in {numref}`M01Fig06`.

## Apparatus

```{figure} VectorTableFigures/M1_ForceTable_06_table_v2025-01.png
:name: M01Fig06
:width: 90%
:align: center

(Left) Illustration of the force table. (Right) An example of how to determine the force $\vec{F}_{3}$ needed to balance two given forces $\vec{F}_{1}$ and $\vec{F}_{2}$.
```

The apparatus for this experiment consist of a force table, weight holders, and weights (see {numref}`M01Fig06`). The force table consists of a circular tabletop mounted on a vertical rod held in a tripod support with leveling screws. The rim of the circular top has a 360° scale engraved on it along which it is possible to clamp a number of pulleys. At the center of the table is a small ring held in place by means of a removable pin. The ends of three cords are tied to the ring with each cord leading over a pulley and ending with a weight holder tied to its other end. When the forces along the cords acting upon the small ring are balanced, or in static equilibrium, the ring remains stationary. For this lab, the force pulling on the ring is the tension of the string, which is merely translated from horizontal on the table to vertical.

Each hanging mass has an associated weight (force) due to being pulled *down* by gravity. This weight is balanced by the *upward* tension force of the vertical part of the cord which is merely translated from vertical to horizontal tension by the pulley. Thus, the force pulling the ring in the direction of the cord is

```{math}
:label: eq-M01-ForceG
\vec{F}_\text{weight} = m \cdot \vec{g} = \vec{F}_\text{tension}
```

For accurate measurements of the angles involved, each cord must be aimed directly at the peg at the center of the ring requiring that the equilibrium condition must be established when the ring is exactly centered around the pin on the table. Use consistently  the same counterclockwise protractor.



## Experimental Procedure

### Preview & Examples

For today's lab, two different cases will be assigned involving two given vectors and the **determination of the equilibrant vector**. A third case involves the **determination of the mass of two unlabeled masses** by balancing the system from a single known mass.

#### EXAMPLE --- Finding the Equilibrant (First two cases)

For each of the first two cases, you will have two given masses at given angles (direction). Each mass, consisting of a 50 g hanger plus the necessary additional mass, will be hung from a cord routed over a pulley at the assigned angular positions and finally tied to the ring. A third cord, hanger, and pulley assembly is put in place for the third, unknown force vector. Each force is the weight of the hanging mass at the pulley angle. Determine the unknown forces for each of the two cases.

If, for example, you were given the following case to work with

$$
\begin{array}{rcl}
\text{Mass 1:} & 200\,\text{g} & @\,0^\circ \\
\text{Mass 2:} & 250\,\text{g} & @\,135^\circ
\end{array}
$$

you would place a pulley at 0° and add 150 g to the 50 g weight hanger for a total 200 g. As mentioned in {eq}`eq-M01-ForceG`, the tension on the cord is the same on both sides of the pulley so that the downward pull of gravity on the hanger and masses is equal to the tension in the cord leading to the ring. Thus,

$$\vec{F_1} = m \vec{g} = 0.20\,\text{kg} \times 9.8\,\text{m/s}^2 = 1.96\,\text{N} \text{ @ } 0°.$$

Similarly, add 200 g to a 50 g weight hanger and run its cord over a pulley mounted at 135°.

$$\vec{F_2} = m \vec{g} = 0.25\,\text{kg} \times 9.8\,\text{m/s}^2 = 2.45\,\text{N} \text{ @ } 135°.$$

Having established the given magnitudes and directions for each of the given forces, $\vec{F}_{1}$ and $\vec{F}_{2}$, you would adjust both the amount of mass hanging on cord 3 and its angular position so that the ring is stationary at the center of the table. In order for angular measurements to be accurate, **each cord must be on a line that crosses through the center of the table**. Sighting *along* each cord towards the center pin can help you to easily and accurately check this.

To determine the equilibrant vector experimentally $\vec{F}_{3}$, you will record both the angular position (**direction**) and total mass (to determine **magnitude** of the balancing force from the total hanging weight) required to balance $\vec{F}_{1}$ and $\vec{F}_{2}$. You will then compare this vector to the expected vector based on your theoretical calculations.

#### EXAMPLE --- Determining 2 Unlabeled Masses (Third case)

In the third case, you will experimentally **determine two unlabeled masses** by balancing the $x$ and $y$ components of the force of a single known mass.
Place the pulley with the known mass $M_1 = 50\,\text{g}$ at $\theta_1 = 0°$.
Experimentally determine the angles $\theta_2$ and $\theta_3$ for the unlabeled masses $M_2$ and $M_3$ that result in the ring being in equilibrium. For this case, **assume angles $\theta_2$ and $\theta_3$ are actual values**.

We can calculate the theoretical unlabeled masses using the method of components.
You have to solve a pair of equations for the $x$ and $y$ components of force.
The equation for equilibrium in the $x$ direction is

```{math}
:label: eq-M01-unknownx
\sum_{i=1}^{n=3} F_{i,x} = F_{1,x} + F_{2,x} + F_{3,x} = (M_1 + M_2 \cos\theta_2 + M_3 \cos\theta_3)g = 0.
```

Similarly, the equation for equilibrium in the $y$ direction is

```{math}
:label: eq-M01-unknowny
\sum_{i=1}^{n=3} F_{i,y} = (M_2 \sin\theta_2 + M_3 \sin\theta_3)g = 0.
```

In these equations, we are assuming we know $M_1$, $\theta_1$, $\theta_2$, $\theta_3$, and that we want to determine $M_2$ and $M_3$. Of the various ways your could do this, one way is to multiply {eq}`eq-M01-unknownx` by $\sin \theta_2$ and {eq}`eq-M01-unknowny` by $\cos \theta_2$. The result is:


```{math}
:label: eq-M01-unknownxSIN
(M_1\sin\theta_2 + M_2\cos\theta_2\sin\theta_2 + M_3\cos\theta_3\sin\theta_2) = 0
```

```{math}
:label: eq-M01-unknownyCOS
(M_2\sin\theta_2\cos\theta_2 + M_3\sin\theta_3\cos\theta_2) = 0
```

You can then subtract the $y$ component {eq}`eq-M01-unknownyCOS` from the $x$ component {eq}`eq-M01-unknownxSIN`

```{math}
:label: eq-M01-unknownxSIN-unknownyCOS
(M_1\sin\theta_2 + M_2\cos\theta_2\sin\theta_2 + M_3\cos\theta_3\sin\theta_2)
- (M_2\sin\theta_2\cos\theta_2 + M_3\sin\theta_3\cos\theta_2) = 0
```
to find an equation where the only unknown is $M_3$:

```{math}
:label: eq-M01-solveM3
M_1 \sin \theta_2  + M_3 \cos \theta_3 \sin \theta_2 - M_3 \sin \theta_3 \cos \theta_2 = 0.
```

After algebraically solving for $M_3$, you can use the known values to solve for the experimental $M_3$ and enter the value in your data table for later comparisons to the actual values.

After having algebraically solved for $M_3$ with {eq}`eq-M01-solveM3`, you could plug that equation back in to {eq}`eq-M01-unknownyCOS` to eliminate $M_3$ to find an equation where the only unknown is $M_2$:

```{math}
:label: eq-M01-solveM2
M_1 \sin \theta_3  + M_2 \cos \theta_2 \sin \theta_3 - M_2 \sin \theta_2 \cos \theta_3 = 0.
```

After algebraically solving for $M_2$, you can use the known values to solve for the experimental $M_2$ and enter the value in your data table for later comparisons to the actual values.

You would then measure $M_{2,actual}$ and $M_{3,actual}$ on the scale and enter the values in the table and comare.


```{admonition} Reminder on Data Taking
:class: warning
It is good practice to **COMPLETE THE ANALYSIS OF THE FIRST CASE BEFORE CONTINUING TO THE NEXT CASE**. If you have some error in your experimental method or in your calculation, you can correct it before completing all the other cases. The layout of the data table for additional cases can then be created by copying the first case after you are confident in your results from the first case.
```

### CASE 1 & 2 -- Finding the Equilibrant Vector (Balancing Force)

```{admonition} OVERVIEW
:class: note
- Understand how to add and balance vectors using the **method of components**.
- Conduct 2 cases of two additive, known vectors (weights at given angles in Table {ref}`tab-case12`) to experimentally determine the third balancing or equilibrant vector.
- Compare the experimental results to theoretically expected vectors.
- **Assume** 0° is the +x direction, 90° is the +y direction
```

```{table} Case 1 & 2 Given Values
:name: tab-case12

| Hanger (i.e. Vector)   | Mass (g) | Angle (°) |
|----------|----------|-----------|
|    | **Case 1**           |
|  1 | 150      | 0°        |
|  2 | 150      | 70°       |
|  3 | ?        | ?         |
|    | **Case 2**           |
|  1 | 100      | 75°       |
|  2 | 200      | 115°      |
|  3 | ?        | ?         |
```

For these first two cases, with given initial values in Table {ref}`tab-case12`, experimentally determine the 3rd (equilibrant) vector and compare your results to your expected values.

```{admonition} Run First Case Calculations (Start to finish before moving on to the second case)
:class: warning
Reminder, run first case fully before moving on to additional cases. Don't just take all of your data without checking your methodology.
```

1. Create data tables for the first case. NOTE: The data layout for each of the first two cases is the same. Create for the first case and run the whole experiment, then you can copy/paste the same data table for the additional case(s).
   - Common data section with accepted value of $g$ (9.803 m/s²), mass of the hanger, list of slotted masses with their uncertainties (see table {ref}`tab-slotted` later in the procedure), and any other common values. You will reference these values in the calculations.
   - An experimental data table (e.g. {ref}`experimental-data-vectortable`) to record your experimental results with:
     - With **three rows** (1 for each of the 3 vectors).
     - Include **columns** for:
       - $m_i$: hanging mass in kilograms (kg)
       - $\delta m_i$: your estimate of the experimental uncertainty [± value] of the masses
       - $F_i$: calculated magnitude of the force in Newtons (N)
       - $\theta_i$: direction of the force vector in degrees
       - $\delta \theta_i$: your estimate of the experimental uncertainty of the angle
       - $F_{i,x}$: calculated $x$-component of each force vector
       - $F_{i,y}$: calculated $y$-component of each force vector
   - An analysis table (e.g. {ref}`analysis-vectortable-resultant-and-sum`) to analyze the results of your measurements. This is effectively one row as there would be just a single value for each of the variables. The columns should include variables:
     - $R_x$: the $x$ component of the resultant vector $\vec{R}$
     - $R_y$: the $y$ component of the resultant vector $\vec{R}$
     - $R$: magnitude of the resultant vector $\vec{R}$ in Newtons
     - $\theta_{R}$: direction of the resultant vector $\vec{R}$ in degrees
     - $F_{x\text{,total,experimental}}$ & $F_{y\text{,total,experimental}}$: total of your measured vector components. Could also be stated as the sum of the experimental $x$ and $y$ vector components from $\vec{R}$ and $\vec{F}_3$, or as $\sum_{i=1}^{n=3} F_{i,x}$ and $\sum_{i=1}^{n=3} F_{i,y}$.
     - $\vec{F}_{\text{total,experimental}}$ which we will treat as $\delta \vec{F}_3$.
   - A secondary analysis table (e.g. {ref}`analysis-vectortable-theory`) to analyze your expected values. This is also effectively one row as there would be just a single value for each of the variables. The columns should include variables:
     - $F_{3,\text{theoreticalMagnitude}}$: your expected or theoretical magnitude of the equilibrant force in N
     - $m_{3,\text{theoretical}}$: theoretical equilibrant mass in kg
     - $\theta_{3,\text{theoretical}}$: theoretical equilibrant direction in degrees

2. Starting with the first case, add slotted masses to hangers 1 & 2 to set their masses equal to the given values in Table {ref}`tab-case12`. 
```{admonition} Note
:class: note
- Hangers are 50 g.
- Slotted masses are available at the table at the front of the room.
```
3. Loosen the screws of the black pulleys to rotate them around the tabletop to their given angles and retighten.

4. With hanger 3 (unknown vector), add or subtract slotted masses and scoot the pulley with hanger and masses around the force table until the system is at equilibrium.
```{admonition} For equilibrium
:class: note
- The ring should be as perfectly centered around the center pin as possible.
- You should see all the strings point from the pulley directly towards the center pin.
```

5. Note your $m_i$ & $\theta_i$ values. 

6. Also note both of your estimated uncertainties $\delta m_i$ & $\delta \theta_i$. 
   - For $\delta \theta_i$, estimate this based on the force table's increments and your confidence that the ring is still centered on the center pin. Example: move the pulley left or right until you're no longer convinced the ring is centered; however far you've shifted it, that will be your $\delta \theta_i$ range. 
   - For $\delta m_i$, add up the total uncertainty of each of your slotted masses. For today, assume each hanger is exactly 50 g, but the list of uncertainties for the *slotted masses* is below. Example: if you had measured $123$ g from just slotted masses, you could have used one of each `100, 20, 2, 1 g`, which would end up giving an uncertainty of $123 \pm (1 + 0.2 + 0.04 + 0.03)$ g or $123 \pm 1.27$ g. :

```{table} Slotted Masses
:name: tab-slotted

| Mass (g) | Uncertainty (g) |
|:--------:|:---------------:|
|   200    |       2.0     |
|   100    |       1.0     |
|    50    |       0.5     |
|    20    |       0.2     |
|    10    |       0.1     |
|    5     |       0.1     |
|    2     |       0.04    |
|    1     |       0.03    |
```

7. Calculate the hangers' respective forces $F_i$ using {eq}`eq-M01-ForceG`.

8. Determine the hangers' respective $x$ and $y$ components $F_{i,x}$ and $F_{i,y}$. See {eq}`eq-M01-cosSinAngle`. 

```{admonition} Excel Uses Radians
:class: note
Excel functions require angles to be in radians; use `RADIANS()` function to convert.
```

9. In your analysis table, determine $R_x$ and $R_y$, the $x$ and $y$ components of the resultant of this case's two given force vectors $\vec{F}_1$ and $\vec{F}_2$.

10. Determine the magnitude $R$ of the resultant vector (see Pythagorean Theorem in {eq}`eq-M01-resultantMag`).

11. Determine the direction $\theta_R$ of the resultant vector. See {eq}`eq-M01-arctan`. Use the `ATAN2()` Excel function to get the angle as measured counterclockwise from 0°.

```{admonition} We Use Degrees
:class: note
Excel trig functions return angles in radians; use `DEGREES()` function to convert.
```

11. Determine $F_{x\text{,total,experimental}}$ & $F_{y\text{,total,experimental}}$, the sum totals of the $x$ and $y$ experimental components from $\vec{R}$ and $\vec{F}_3$ (see also {eq}`eq-M01-allVectorsResultant`).
<!---; use them to determine $\delta \vec{F}_3$.--->

12. Determine $F_{\text{total,experimental}}$, the sum total experimental magnitude of all three of your vectors determined in similar fashion to {eq}`eq-M01-resultantMag`, but with $F_{x\text{,total,experimental}}$ & $F_{y\text{,total,experimental}}$.

```{admonition} $F_3$ Error Approximation
:class: note
 - For simplicity in our error analysis, we will also treat this value as the minimum uncertainty $\delta F_3$ of the magnitude of your experimentally determined equilibrant vector such that your experimental magnitude would be $F_3 \pm \delta F_3$. 
 - ***Consider***: The **sum of all three vectors** or **total force *should* be zero** because the ring and vectors are in equilibrium with no acceleration (Newton's 2nd Law). The difference between the experimental total force (probably not zero) and theoretical total force (zero) can therefore be an approximation of the ***minimum experimental uncertainty***. Our error in reality may be larger, but our error bars are at minimum $\delta F_3$ away from zero.
```

12. In your secondary analysis table, based on your determined resultant $\vec{R}$ of the first two vectors, determine your theoretical equilibrant vector $\vec{F}_{3,\text{theoretical}}$ and its associated mass (see {eq}`eq-M01-equilibrant`):
    - magnitude $F_{3,\text{theoreticalMagnitude}}$
    - direction $\theta_{3,\text{theoretical}}$
    - mass $m_{3,\text{theoretical}}$

13. COMPARE your experimental results of hanger 3 to the theoretical values. Does $\vec{F}_3 \pm \delta \vec{F}_3$ overlap (and therefore agree) with your theoretical value $\vec{F}_{3,\text{theoretical}}$? If not, are there significant issues that may be contributing to the discrepancy? Discuss with instructor if so. To be further discussed in Section {ref}`interpretation1`.

```{admonition} Continue to additional case?
:class: warning
***If you are satisfied your calculations are complete and results seem reasonable (feel free to check with your professor), it is at this point that you may continue to the second case.***
```

14. Repeat for the second case once you are satisfied in your values and calculations.

### CASE 3 -- Determining 2 Unlabeled Masses

```{admonition} OVERVIEW
:class: note
- Understand how to determine two unknown values of a 3 vector system using the **method of components**.
- *CONSIDER*: Each vector has two pieces of information, **magnitude** and **direction** --- how many pieces of information total do we have to work from?
- Determine the masses of two figurines (one is a black Pikachu, the other is a white corgi that can each sit on their respective hangers) by balancing the force vectors. Treat Pikachu-black as $m_2$ and the corgi-white as $m_3$.
- Compare the experimental results to actual masses as measured with a triple-beam balance.
- **Assume** the angles for both Pikachu and the corgi, once found, are treated as given values (so you only have two unknowns with two equations).
```

```{table} Case 3 Given Values
:name: tab-case3

| Hanger (i.e. Vector)   | Mass (g) | Angle (°) |
|----------|----------|-----------|
|    | **Case 3**           |
|  1 (empty, $M_1$) | 50  (just hanger, no extra masses)    | 0°        |
|  2 (Pikachu-black, $M_2$) | ?        | ?         |
|  3 (corgi-white, $M_3$)| ?        | ?         |
```

Experimentally determine the mass of just the Pikachu (black figurine) and the corgi (white figurine) and compare to actual values. The angles for hangers 2 & 3 will be treated as given values once experimentally determined. ***Reminder, the hangers are 50 g each.***

1. Create data table for this case with columns for (e.g. {ref}`vectortable-case3data`):
   - Experimental and given masses $m_{i\text{,experimental}}$:
      - Given mass $m_1$ is shown in the Table {ref}`tab-case3` for the empty hanger.
      - $m_{2\text{,Pikachu-black}}$ & $m_{3\text{,corgi-white}}$ as calculated from $M_2$ and $M_3$ in {eq}`eq-M01-solveM2` and {eq}`eq-M01-solveM3`.
   - Experimental and given angles $\theta_{i\text{,experimental}}$:
      - Given angle $\theta_1$ is shown in the Table {ref}`tab-case3` for the empty hanger. 
      - $\theta_{2,\text{Pikachu-black}}$ & $\theta_{3,\text{corgi-white}}$ as experimentally determined --- **treat as actual given values once you find equilibrium. You will use these to solve for the masses later.**
   - Actual values for $m_{i\text{,actual}}$. Masses $m_{2,\text{Pikachu-black,actual}}$ & $m_{3,\text{corgi-white,actual}}$ for each figurine as measured on a triple-beam balance.
   - The % Difference of $m_{2\text{,experimental}}$ and $m_{3\text{,experimental}}$ experimentally determined values to their actual measured values (see {eq}`M1-PercentDiff` in Section {ref}`interpretation1`).

2. Place the respective masses on their hangers, with $m_1$ set to 0°

3. Unscrew the black pulleys to rotate them around the tabletop until you find equilibrium. You are only changing the angles of $\theta_{2,\text{Pikachu-black}}$ & $\theta_{3,\text{corgi-white}}$. ***NO ADDITIONAL MASS IS REQUIRED***.

4. Once you've found equilibrium, note the $\theta_{2,\text{Pikachu-black}}$ & $\theta_{3,\text{corgi-white}}$ values as actual values to use in later equations (i.e. as if they're given angles).

5. Determine $m_{2,\text{Pikachu-black}}$ & $m_{3,\text{corgi-white}}$ by algebraically solving {eq}`eq-M01-solveM3` and {eq}`eq-M01-solveM2` for $M_2$ and $M_3$ and plugging in known values. There should be scratch paper and extra pens & pencils at the front of the room.

6. Using a triple-beam balance, measure directly the actual mass of $m_{2,\text{Pikachu-black, actual}}$ & $m_{3,\text{corgi-white, actual}}$.  You can include the mass of the hanger $m_1$ to double check the mass hanger.

7. COMPARE your experimental results of each of the unlabeled masses to their actual values. Calculate the % difference of $m_2$ and $m_3$ experimentally found values to the actual measured values. What may be contributing to a larger or smaller difference? To be further discussed in Section {ref}`interpretation1`.

(interpretation1)=
## Post-Lab Submission --- Interpretation of Results

- Make sure to submit your finalized data table (Excel sheet). 
- In a **paragraph**, summarize the results you have determined in each case, i.e. $\vec{F}_3\pm\delta \vec{F}_3$... and answer the following questions (longer does not mean better):
	- What is a vector?
  - What is the physics behind balancing our vectors today?
	- Case 1 & 2 (Finding Equilibrant):
	  - Looking at your experiment, why do the two given masses not add up to the third mass?
	  - What are your results, and how do they compare to the theoretical predictions?
	    - In other words, for each of the first two cases, COMPARE your experimental results of hanger 3 to the theoretical values for hanger 3.
	      - Does $\vec{F}_3 \pm \delta \vec{F}_3$ overlap (i.e. agree) with your theoretical value $\vec{F}_{3,\text{theoretical}}$?
	      - Does $m_3 \pm \delta m_3$ overlap with your theoretical value $m_{3,\text{theoretical}}$? 
	      - Does $\theta_3 \pm \delta \theta_3$ overlap with your theoretical value $\theta_{3,\text{theoretical}}$? 
	- Case 3 (Unlabeled Masses):
	  - How do your values for $m_\text{Pikachu-black}$ and $m_\text{corgi-white}$ compare to your actual values from the triple-beam-balance?
	  - What is the percent difference between your experimentally determined masses and their actual measured values? Calculate the % difference in each of the masses using the following relation (*Note: If you change the Excel number format of this cell to `Percentage` do not multiply by 100 as Excel will do that for you*):
```{math}
:label: M1-PercentDiff
\text{% Difference} = \frac{\text{Experimental Value} - \text{Actual Value}}{\text{Actual Value}} \times 100\%.
```
- In a **paragraph**, summarize your error analysis. Be qualitative not only quantitative.
	- What are the uncertainties of Cases 1 & 2 (Finding Equilibrant)?
  - What is the precision of your equipment (force table, masses, etc.)?
  - What are possible systematic (affecting accuracy) errors of the experiment? What are possible random (affecting precision) errors?
  - Return to results section question: ''In other words, for each of the first two cases, COMPARE your experimental results of hanger 3 to the theoretical values for hanger 3.'' How does changing $m_3$ by $\delta m_3$ and $\theta_3$ by $\delta \theta_3$ change $\vec{F}_3$? Do the math in your spread sheet.
      - What uncertainties might make the difference between your final results and expected values larger or smaller?
  - For Case 3 (Unlabeled Masses), what errors may contribute to larger or smaller % differences to the actual measured-by-triple-beam-balance values?




## The Whiteboard

Example data tables are shown below to assist you in building your spreadsheet for this lab. Additionally the original whiteboard summary is at the end of this section.

(experimental-data-vectortable)=
### Case 1 & 2 Experimental Data

| Hanger/Vector   | $m$ (SI units) | $\delta m$ (SI Units) | $\vec{F}$ (SI Units) | $\theta$ ($^\circ$) | $\delta \theta$ ($^\circ$) | $F_x$ (SI Units) | $F_y$ (SI Units) |
|-------|--------|---------|-------|---------|----------|--------|--------|
| 1 |        |         |       |         |          |        |        |
| 2 |        |         |       |         |          |        |        |
| 3 |        |         |       |         |          |        |        |

(analysis-vectortable-resultant-and-sum)=
### Case 1 & 2 Additional Data - Resultant & $\sum_{i=1}^N \vec{F}_i$
| $R_x$ (SI units) | $R_y$ (SI Units) | $R$ (SI Units) | $\theta_R$ ($^\circ$) | $F_{x,\text{total,experimental}}$ (SI Units) | $F_{y,\text{total,experimental}}$ (SI Units) | $F_{\text{total,experimental}}$ treated as $\delta F_3$ (SI Units) |
|------------------|------------------|----------------|-----------------------|---------------------------------------------|---------------------------------------------|---------------------------------------------------------------------|
|                  |                  |                |                       |                                             |                                             |                                                                     |


(analysis-vectortable-theory)=
### Case 1 & 2 Analysis - Theoretical Values
| $F_{3,\text{theoreticalMagnitude}}$ (SI Units) | $\theta_{3,\text{theoretical}}$ ($^\circ$) | $m_{3,\text{theoretical}}$ (SI Units) |
|-----------------------------------------------|--------------------------------------------|---------------------------------------|
|                                               |                                            |                                       |




(vectortable-case3data)=
### Case 3 Data

| Vector | $m_{i\text{,experimental}}$ (SI units) | $\theta_{i\text{,experimental}}$ ($^\circ$) |  $m_{i\text{,actual}}$ (SI units) | % diff. masses |
|--------|----------------------|---------|----------|----------------|
| 1 (known) |                  |         |          |                |
| 2 (Pikachu-black) |                  |         |          |                |
| 3 (Corgi-white)   |                  |         |          |                |


### Original Whiteboard Info

```{figure} VectorTableFigures/ForceTable_2025_Summer_01.jpg
:name: vectorTableWhiteboard_01
:width: 100%
:align: center

```

```{figure} VectorTableFigures/ForceTable_2025_Summer_02_v2025-01.jpg
:name: vectorTableWhiteboard_02
:width: 100%
:align: center

```
