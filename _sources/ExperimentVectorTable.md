# Force Table with 3 Vectors at Equilibrium

<!-- Adapted from LaTeX for Jupyter Book Markdown -->

## Background


```{admonition} OVERALL GOALS
:class: note
Use a "force table" to study:

- how vectors are added
- the concept of force vectors in equilibrium
```



There are two types of physical quantities: **scalars** and **vectors**. The number of attributes required to define a scalar and a vector distinguishes them.

- A **scalar** has just a **magnitude** (how large or small something is, or positive/negative). Examples: temperature, speed (m/s).
- A **vector** is described by both a **magnitude** *and* **direction**. Examples: velocity (m/s at some angle), force (N at some direction).

A force example: a force may be 100 N in magnitude with direction 90° counterclockwise from the x-axis. This force vector is written as **100 N @ 90°**. We use boldface for vectors (**F**), and regular type for scalar magnitudes and components (F).

When several vectors act on an object, we often want the sum, called the **resultant vector**. Suppose force vectors **F₁** and **F₂** act on a body. The resultant **R** is:

$$
\vec{R} = \vec{F}_1 + \vec{F}_2
$$

If many forces act:

$$
\vec{R} = \sum_{i=1}^N \vec{F}_i
$$

When the resultant force is zero, the object is in equilibrium.

---

There are two methods of vector addition:

- The graphical method (reviewed here, but not conducted during lab today)
- The method of components (conducted during lab today)

### Graphical Method

Vectors **F₁** and **F₂** are added graphically by drawing one vector as an arrow to scale, then placing the second vector's tail at the tip of the first. The resultant **R** is the vector from the tail of the first to the tip of the second. The order of addition does not matter:

$$
\vec{F}_1 + \vec{F}_2 = \vec{F}_2 + \vec{F}_1 = \vec{R}
$$

> *Insert Figure: Two force vectors F₁ and F₂, and their graphical addition ("tail-to-tip" method).*

Choose an appropriate scale (e.g., 1 N = 10 cm). The magnitude of **R** is measured with a ruler, and the angle with a protractor. Subtraction is addition with the negative vector pointing in the opposite direction.

### Method of Components

The method of components is more accurate. Each vector is resolved into x and y components:

$$
\begin{align*}
F_{1,x} &= F_1 \cos(\theta_1) \\
F_{1,y} &= F_1 \sin(\theta_1) \\
F_{2,x} &= F_2 \cos(\theta_2) \\
F_{2,y} &= F_2 \sin(\theta_2)
\end{align*}
$$

Add the components:

$$
R_x = F_{1,x} + F_{2,x} \\
R_y = F_{1,y} + F_{2,y}
$$

The magnitude of the resultant:

$$
R = \sqrt{R_x^2 + R_y^2}
$$

The angle θ (direction):

$$
\theta = \arctan\left(\frac{R_y}{R_x}\right)
$$

> *Insert Figure: Adding 2 vectors using the method of components, showing x- and y-components.*

#### Example

Suppose:

- F₁ = 1 N @ 0°
- F₂ = 1 N @ 45°

Then:

- F₁ₓ = 1 N × cos(0°) = 1 N
- F₁ᵧ = 1 N × sin(0°) = 0 N
- F₂ₓ = 1 N × cos(45°) ≈ 0.707 N
- F₂ᵧ = 1 N × sin(45°) ≈ 0.707 N

So:

- Rₓ = 1 + 0.707 = 1.707 N
- Rᵧ = 0 + 0.707 = 0.707 N
- R = √(1.707² + 0.707²) ≈ 1.85 N
- θ = arctan(0.707 / 1.707) ≈ 22.5°

---

In this lab, an object will be presented with two known forces. Equilibrium is established by adding a third **equilibrant** force **F₃** such that the sum of the three forces is zero:

$$
\vec{F}_3 = -\vec{R}
$$

> *Insert Figure: Illustration of the method to determine the force F₃ needed to balance F₁ and F₂.*

**F₃** has the same magnitude as **R**, but acts in the opposite direction.

---

### Apparatus

> *Insert Figure: Illustration of the force table apparatus.*

The apparatus consists of a force table, weight holders, and weights. The force table is a circular tabletop with a 360° scale, pulleys, and a central ring. Each cord is tied to the ring, passes over a pulley, and ends with a weight. When the forces are balanced, the ring remains stationary.

Each hanging mass exerts a force due to gravity:

$$
\vec{F}_{\text{weight}} = m \times \vec{g} = \vec{F}_{\text{tension}}
$$

For accurate measurements, each cord must be aimed directly at the center of the ring.

---

## Experimental Procedure

### Preview

You will perform two cases involving two given vectors and determine the equilibrant vector. A third case involves determining the mass of two unlabeled masses by balancing the system from a single known mass.

#### Finding the Equilibrant (First two cases)

For each case, you will have two given masses at given angles. Each mass (50 g hanger + additional mass) is hung from a cord over a pulley at the assigned angle. A third cord is used for the unknown force vector. Each force is the weight of the hanging mass at the pulley angle.

**Example:**

- Mass #1: 200 g @ 0°
- Mass #2: 250 g @ 135°

Calculate forces:

- F₁ = 0.20 kg × 9.8 m/s² = 1.96 N @ 0°
- F₂ = 0.25 kg × 9.8 m/s² = 2.45 N @ 135°

Adjust mass and angle for cord 3 until the ring is centered. Record the angular position (direction) and total mass for the balancing force.

#### Determining 2 Unlabeled Masses (Third case)

You will determine two unlabeled masses by balancing the x and y components of the force of a known mass.

- Place the known mass M₁ = 50 g at θ₁ = 0°
- Experimentally determine the angles θ₂ and θ₃ for the unlabeled masses M₂ and M₃ that result in equilibrium

Theoretical calculation uses the method of components:

$$
(M_1 + M_2 \cos\theta_2 + M_3 \cos\theta_3)g = 0 \\
(M_2 \sin\theta_2 + M_3 \sin\theta_3)g = 0
$$

Solve for M₂ and M₃ using the measured angles.

---

> **Tip:** Complete the analysis of the first case before continuing to the next. This allows you to correct errors early.

---

### CASE 1 & 2 -- Finding the Equilibrant Vector (Balancing Force)

```{admonition} GOALS
:class: note

- Understand how to add and balance vectors using the method of components.
- Conduct 3 cases of two additive, known vectors to experimentally determine the third equilibrant vector.
- Compare experimental results to theoretical predictions.
- Assume 0° is the +x direction, 90° is the +y direction.
```

#### The first two cases are:

| Case 1                  | Case 2                  |
|-------------------------|-------------------------|
| hanger 1: 150 g @ 0°    | hanger 1: 100 g @ 75°   |
| hanger 2: 150 g @ 70°   | hanger 2: 200 g @ 115°  |
| hanger 3: ? kg @ ?°     | hanger 3: ? kg @ ?°     |

#### Data Table (for each case)

- Common data: accepted value of g (9.803 m/s²), mass of hanger, etc.
- Three rows (one for each vector)
- Columns:
    - $m_i$: hanging mass (kg)
    - $\delta m_i$: uncertainty in mass
    - $F_i$: calculated force (N)
    - $\theta_i$: direction (degrees)
    - $\delta \theta_i$: uncertainty in angle
    - $F_{i,x}$: x-component
    - $F_{i,y}$: y-component

Secondary table for analysis:

- $R_x$, $R_y$: components of resultant
- $R_{\text{mag}}$: magnitude of resultant
- $\theta_R$: direction of resultant
- $F_{x,\text{total experimental}}$, $F_{y,\text{total experimental}}$: vector sum of R and F₃
- $F_{\text{mag, total experimental}}$: magnitude of total force (should be zero at equilibrium)
- Theoretical values for F₃: magnitude, mass, direction

#### Steps

1. Place masses on hangers 1 & 2
2. Set pulleys to given angles
3. Adjust mass and angle for hanger 3 until equilibrium
4. Record $m_3$ and $\theta_3$ (and uncertainties)
5. Calculate forces and components
6. Determine resultant and compare experimental and theoretical values
7. Repeat for the second case

---

### CASE 3 -- Determining 2 Unlabeled Masses

```{admonition} GOALS
:class: note

- Determine two unknown values in a 3-vector system using the method of components.
- Determine the masses of two figurines (black Pikachu as $m_2$, white corgi as $m_3$) by balancing force vectors.
- Compare experimental results to actual masses measured with a triple-beam balance.
```

#### Third case:

- hanger 1: 50 g @ 0°
- hanger 2 (Pikachu-black): ? kg @ ?°
- hanger 3 (corgi-white): ? kg @ ?°

#### Data Table

- Common data: g, mass of hanger, actual values of figurines, etc.
- $m_1$: 50 g (record in kg)
- $\theta_1$: 0°
- $F_{x,1}$, $F_{y,1}$: components of known mass's force
- $\theta_{2,\text{Pikachu-black}}$, $\theta_{3,\text{corgi-white}}$: experimentally determined directions
- $m_{2,\text{Pikachu-black}}$, $m_{3,\text{corgi-white}}$: experimental values (from equations)
- $m_{2,\text{actual}}$, $m_{3,\text{actual}}$: measured with triple-beam balance
- % Difference between experimental and actual values

#### Steps

1. Place masses on hangers, with $m_1$ at 0°
2. Adjust angles for equilibrium (only change $\theta_2$ and $\theta_3$)
3. Record angles as actual values
4. Calculate $m_2$ and $m_3$ using equations
5. Measure actual masses
6. Compare and calculate % difference

---

## Post-Lab Submission --- Interpretation of Results

- Submit your finalized data table (Excel sheet)
- What is a vector?
- **Case 1 & 2 (Finding Equilibrant):**
    - Why don't the two given masses add up to the third?
    - What are the uncertainties?
    - Compare results to theoretical predictions:
        - Does $F_3 \pm \delta F_3$ overlap with theoretical $F_{3,\text{theoretical}}$?
        - Does $m_3 \pm \delta m_3$ overlap with $m_{3,\text{theoretical}}$?
        - Does $\theta_3 \pm \delta \theta_3$ overlap with $\theta_{3,\text{theoretical}}$?
    - How does changing $m_3$ or $\theta_3$ affect results?
- **Case 3 (Unlabeled Masses):**
    - How do $m_{\text{Pikachu-black}}$ and $m_{\text{corgi-white}}$ compare to actual values?
    - Calculate % difference:
      $$
      \% \text{Difference} = \frac{\text{Experimental Value} - \text{Actual Value}}{\text{Actual Value}} \times 100\%
      $$
    - What uncertainties might affect the difference?
- What is the precision of your equipment?
- What are possible systematic errors?

---

*Note: Replace all "Insert Figure" notes with actual images or diagrams in your Jupyter Book as needed.*
