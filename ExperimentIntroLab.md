# Introductory Lab: Domino Size & Density

## Background

### Measurements

Physical measure;oiupdfsljkigsfholjiugsdf;ouisfgth;ouisdfgments are more than a simple numerical value. They are specified by:

1. A physical dimension which is a product of powers of base physical dimensions such as length, time, and mass. Other dimensions include, for example, electric charge.

2. A choice of units. Usually we use SI units: meter (m), second (s), and kilogram (kg).

3. A numerical value that depends on the choice of units.

4. A range of the numerical value depending on the accuracy of measurements.

Calculations performed using physical quantities follow certain rules:

1. Scalar physical quantities can be added or subtracted only if they have the same units.
2. Scalars can be multiplied (or divided). The same action must be performed on the values and on the units.


Volume $V$ and mass $m$ are two measures of the size of an object. If an object is made of a uniform material, then doubling the amount of material will double both its mass and its volume.
Density $\rho$ is ratio of mass to volume.

```{math}
:label: M00_intro_Eq01
\rho=\frac{m}{V}.
```

Density is a material property, independent of the amount of material or shape of the object.
The volume of a rectangular parallelepiped shape, i.e., a box, is the product length times width times height $V=l\cdot w\cdot h$.


### Estimating Error

The accuracy of a measurement depends on the limits of the instrument, and on skill in using the instrument.
One estimate of the accuracy of a measurement is to independently repeat the measurement multiple times and observe the **range and standard deviation of the results**. Another approach is to determine the **instrument tolerance or precision**.

Measurement errors change calculated or derived results in different ways, depending on how the quantities enter equations.
For example, if the measured mass is larger than the actual mass, then the calculated density will also be larger.
Suppose, on-the-other-hand, that the measured volume is larger than the actual volume. Because the volume appears in the denominator of {eq}`M00_intro_Eq01`, the calculated density will be reduced. 


## Experimental Procedure

```{figure} /ExperimentIntroLabFigures/M0_dominos.jpg
:name: M00_intro_Fig01
:width: 80%
:align: center

Left) Dominoes provided. Right) Relevant length, width, height dimensions of the dominoes.
```

```{admonition} OVERALL GOALS
:class: note
- Understand how to take length and mass measurements.
- Understand how to characterize measurement uncertainties with standard deviation.
- Understand how to characterize measurement uncertainties due to instrument precision.
- Each member of the lab group will independently measure the mass, length, width, and height of four provided dominoes per group (i.e. each group gets a pink, green, orange, and blue domino).
```

*NOTE:* It is good practice to **complete the analysis of trials as you do the experiment**. If there is some error in your experimental method or in your calculation, you can correct it before completing all the other trials. The formulas of the rows for later trials can be created by copying the first trial.

The density of the dominoes' plastic and water are roughly the same. Estimate the value you expect in SI units (kg/m³).

- Create a Common Data Table for values used in all the trials. In this case, include the instrumental tolerance of the lab scale and the Vernier caliper.
- Create a row for each domino trial. A trial is the measurement by one lab group member of one domino color.
- Create a Data Table with columns for:
  - Initials of the experimenter
  - Color of the domino
  - Measured length $l$, width $w$, height $h$ measured with Vernier calipers and mass $m$ measured with the triple-beam balance in the instruments' units (e.g. mm, g, etc.)
  - $l$, $w$, $h$, and $m$ converted to SI units
  - Calculated volume $V_\text{color}$ for the trial in SI units
  - Calculated density $\rho_\text{color}$ for the trial in SI units

Create a Data Analysis table including:

- Analysis Table 1:
  - Average and standard deviation of the $l_\text{avg.}$ length, width, height, volume, and density of each color of domino.
  - Maximum and minimum values of the density and volume based on your experimental value and the instrumental tolerance (i.e. $\pm$ values). **NOTE:** To maximize Volume $V$, maximize $l$, $w$, $h$. To maximize density $\rho$, maximize $V$ and minimize $m$.
  
- Analysis Table 2:
  - Average of the length, width, height, volume, and density of the color set measured by each lab group member.

## Post-Lab Submission --- Interpretation of Results

- Make sure to submit your finalized data table (Excel sheet).
- Discuss: Are the densities of all the different colored dominoes the same (within experimental uncertainty based on measurement uncertainties)? Example, do all the $\rho_{\text{blue-person1}}$, $\rho_{\text{blue-person2}}$, etc. agree?
- Discuss: Are the average densities of all four dominoes as measured by each person consistent (within experimental uncertainty based on measurement uncertainties)? Example, do all the $\rho_{\text{blue-person1}}$, $\rho_{\text{green-person1}}$, etc. agree?
- Discuss: Do you expect the dominoes to float in water (at room temperature)?
- What was the precision of your equipment (calipers, triple-beam balance, etc.)?
- What are possible systematic errors of the experiment?
