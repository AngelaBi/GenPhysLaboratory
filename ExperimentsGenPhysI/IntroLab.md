(intro-lab-dominos-overall)=
# || Lab 0 | Introductory Lab: Domino Size & Density


```{admonition} GROUP Post-lab Writeup<br>Review Post-lab Interpretation Questions before lab
:class: important
- Today's lab will have a 🔵 🔵 ***GROUP*** 🔵 🔵 post-lab write-up. Please thoroughly discuss and review with your lab group members before submission.
- **❓❓ See {ref}`postlabs_intro_dominoes` ❓❓**
```



## Background

### ● Background Overview

```{admonition} OVERALL GOALS
:class: note
Review and understand:
- How to take length and mass measurements
- Characterizing measurement uncertainties (delta $\delta$) due to instrument precision
- Characterizing measurement uncertainties and variations with standard deviation (sigma $\sigma$)
```


#### ○ Measurements

Physical measurements are more than a simple numerical value. They are specified by:

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
\rho=\frac{m}{V}
```

Density is a material property, independent of the amount of material or shape of the object.
The volume of a rectangular parallelepiped shape, i.e., a box, is the product length times width times height, i.e.:

```{math}
:label: M00_intro_Eq02
V=l \cdot w \cdot h
```


#### ○ Estimating Error

The accuracy of a measurement depends on the limits of the instrument, and on skill in using the instrument.
One estimate of the accuracy of a measurement is to independently repeat the measurement multiple times and observe the **range and standard deviation of the results**. Another approach is to determine the **instrument tolerance or precision** to help determine individual measurement uncertainties.

Measurement errors change calculated or derived results in different ways, depending on how the quantities enter equations.
For example, if the measured mass is larger than the actual mass, then the calculated density will also be larger that the actual density.
Suppose, on-the-other-hand, that the measured volume is larger than the actual volume. Because the volume appears in the denominator of {eq}`M00_intro_Eq01`, the calculated density will be reduced. 


## Experimental Procedure

### ● Preview

```{admonition} PROCEDURE OVERVIEW
:class: note
- Each member of the lab group will independently:
    - Use {ref}`Vernier Calipers<vernier-calipers-overall>` to measure the *length*, *width*, *height* and a {ref}`Triple Beam Balance<triple-beam-balance-overall>` to measure the *mass* of four provided dominoes per group (i.e. each lab group gets one pink, one green, one orange, and one blue domino, see {numref}`M00_intro_Fig01`).
    - Determine measurement uncertainties from tool limitations (precision).
    - Propagate measurement uncertainties into derived density calculations.
- And as a group:
    - Characterize uncertainties with standard deviation.
    - Organize the dominoes by person or by color.
    - Compare the dominoes to water (should be roughly the same).
```

<!--- add exapmle of % difference or % change to know what it is, or not yet?--->

```{admonition} Good Practice
:class: tip
 It is good practice to **complete the analysis of trials or cases as you do the experiment**. If there is some error in your experimental method or in your calculations, you can correct it before completing all the other trials. The rows with their Excel formulas for later trials can be created by copying the first trial.
```

```{figure} IntroLabFigures/M0_dominos.jpg
:name: M00_intro_Fig01
:width: auto
:align: center

Left) Dominoes provided. Right) Relevant length, width, height dimensions of the dominoes.
```


### ● Preliminary Setup



1. Create data tables (See examples in {ref}`common-data` and {ref}`trial-data`):
    - Create a ***Common Data Table*** for values used in all the trials. In this case, include 
      - the instrumental tolerance or precision of the triple beam balance
      - the instrumental tolerance or precision of the Vernier caliper
      - density room temperature water: $0.998\,\text{kg}/\text{m}^3$
      ```{admonition} Referencing unchanging values
      :class: note
      You can reference these values in these cells with dollar signs to hold the cells constant in your formulas (e.g. `$A$1`) as needed. Additional info, see {ref}`spreadsheet-data-analysis-setup`
      ```

2. Create a ***Data Table*** with 
    - Rows for each domino trial. A trial is the measurement by one lab group member of one domino color. For a group of two, there will be 8 trials; for a group of three, there will be 12 trials.
    - Columns for:
      - Trial number
      - Initials of the experimenter
      - Color of the domino
      - In the units of the instruments (e.g. mm, g, etc.):
        - Domino length $l$, width $w$, height $h$ (see {numref}`M00_intro_Fig01`) measured with Vernier calipers
        - Domino mass $m$ measured with the triple beam balance
      - Converted to SI units:
        - $l$, $w$, $h$, and $m$
      - Calculated volume $V_\text{color}$ for the trial in SI units
      - Minimum volume and maximum volume (SI units)
      - Volume uncertainty $\delta V$
      - Calculated density $\rho_\text{color}$ for the trial in SI units
      - Minimum density and maximum density (SI units)
      - Density uncertainty $\delta \rho$


### ● Experimental Data Collection

```{admonition} Run Single Trial with Calculations First (Start to finish of just one trial)
:class: warning
Each group member will independently measure each of the four dominoes (i.e. four trials per person). ***HOWEVER***, have each group member start with one domino, then go through all the steps of error propagation to minimize and maximize $V$ and $\rho$ before continuing to additional dominoes to ensure your calculations in Excel are behaving properly and that your maeasurement methods are accurate with the calipers and balance. Otherwise, you may find yourselves redoing the whole experiment if you fail to check your measurement techniques early on in the process.
```


3. Record the trial number, group member's name or initials, and the domino color
4. Using the **Vernier calipers** (reviewed in {ref}`vernier-calipers-overall`):
    - note the caliper's *measurement precision* in your **common data** table. For today, we will treat this *smallest measureable increment* as the same for each dimensional measurement uncertainty, $\delta_{\text{caliper}} = \delta_l = \delta_w = \delta_h$. NOTES: Measurement uncertainties can be larger than the precision of your tools; this will happen throughout the semester depending upon your confidence in the measurements. The Greek letter $\delta$ (said as “delta”) is representing the *measurement* uncertainty of each variable (e.g. $l \pm \delta_l$). Then measure and record, in the units of the calipers, the:
      - length $l$
      - width $w$
      - height $h$
5. Using the **triple beam balance** (reviewed in {ref}`triple-beam-balance-overall`):
    - note the balance's measurement precision (smallest *measureable* increment, $\delta_m$) in your **common data** table. Then measure & record the mass $m$, in the units of the balance (e.g. grams).

6. Convert your measurements into SI units (e.g. kilogram kg, meter m, second s, etc.).

7. Calculate volume $V$ using {eq}`M00_intro_Eq02`, and density $\rho$ using {eq}`M00_intro_Eq01`.


### ● Data Analysis --- Individual Trial Error Propagation

You will now analyze your domino measurements in a few ways, through measurement uncertainties and through average and standard deviation (i.e. the spread of the data from the average).

8. In your data table, for each trial, determine the volume and density uncertainties $\delta V$ and $\delta \rho$ by calculating the minimized and maximized values for both $V$ and $\rho$, and taking half their difference:

    - To minimize $V$, **minimize the values that go into that calculation** ($l$, $w$, $h$) by the caliper's measurement uncertainty treated, for the purposes of today, as each value's uncertainty in {eq}`M00_intro_Eq02`. This results in:

    ```{math}
    :label: M00_intro_Eq_volumeMin
    V_{\min} = (l-\delta_l)\cdot(w-\delta_w)\cdot(h-\delta_h)
    ```

    - Maximize $V$ in a similar manner, now by maximizing $l$, $w$, $h$ by their measurement uncertainty.

    - Calculate the volume's uncertainty $\delta V$ by taking half the difference between max and min volume values:

    ```{math}
    :label: M00_intro_Eq_deltaV
    \delta V = \frac{V_{\max} - V_{\min}}{2}
    ```

    - In a similar way, minimize and maximize $\rho$ by using either $V_{\max}$ or $V_{\min}$ with $m$ minimized or maximized.
      - e.g. for $\rho_{\min}$, you would minimize the numerator and maximize the denominator such as:


    ```{math}
    :label: M00_intro_Eq_densityMin
    \rho_{\min} = \frac{m_{\min}}{V_{\max}} = \frac{m-\delta_m}{V_{\max}}
    ```

    - Calculate the density's uncertainty $\delta \rho$ by similarly taking half the difference between max and min values.



9. At this point, you should have a complete trial with a range of densities based on your measurement uncertainties. 

10. ***Consider:*** Does this range appear far from your estimated densities from the prior knowledge that these dominoes' densities are close to that of water? Or, do your results between each person significantly disagree? If so, this is a good time to double check any of your measurements that may seem like an outlier or any of your calculations that may have been entered into Excel incorrectly.

    ```{admonition} Continue to additional trials?
    :class: warning
    ***If you are satisfied, it is at this point that each person can now continue measuring the other dominoes.***
    ```

### ● Data Analysis --- Color & Group Member Comparisons


Up to this point, each individual trial has its own range of densities based on the measurement uncertainties. If we were only analyzing individual trials, this can be satifactory for error analysis. However, each person measured each color domino. We can therefore also analyze the repeated measurements by looking at the average densities and the spread or variation of the data from that average value (i.e. standard deviation, often denoted as the Greek letter sigma, $\sigma$).

11. We will analyze the data in two ways, first by sorting your data by domino color (across all group members) and by person (across all domino colors). To do so, create two Data Analysis tables including:
    - Analysis Table 1 (by color, e.g. {ref}`analysis-table-1-by-color`):
      - Average and standard deviations of the length, width, height, mass, volume, and density of each color of domino.
    - Analysis Table 2 (by person, e.g. {ref}`analysis-table-2-by-person`):
      - Average and standard deviations of the length, width, height, mass, volume, and density of the color set measured by each lab group member.

    ```{admonition} Excel Averages & Standard Deviations
    :class: tip
    In Excel, calculate the average using the function: `=AVERAGE(referenced cells)` and standard deviations using the function: `=STDEV(referenced cells)` or `=STDEV.S(referenced cells)`
    ```

    ```{admonition} Domnios vs. Water?
    :class: attention
    Based on your data, do you expect some or all of the dominoes to float, sink, or stay neutrally buoyant in room-temperature water? Before you leave, there should be a bucket of water near the front of the lab, test it out!
    ```


(postlabs_intro_dominoes)=
## Post-Lab Submission --- Interpretation of Results
<!---
- Make sure to submit your finalized data table (Excel sheet).
- Discuss: Are the densities of all the different colored dominoes the same (within experimental uncertainty based on measurement uncertainties)? Example, do all the $\rho_{\text{blue-person1}}$, $\rho_{\text{blue-person2}}$, etc. agree?
- Discuss: Are the average densities of all four dominoes as measured by each person consistent (within experimental uncertainty based on measurement uncertainties)? Example, do all the $\rho_{\text{blue-person1}}$, $\rho_{\text{green-person1}}$, etc. agree?
- Discuss: Do you expect the dominoes to float in water (at room temperature)?
- What was the precision of your equipment (calipers, triple beam balance, etc.)?
- What are possible systematic errors of the experiment?
--->


```{admonition} Defend your conclusions with your data
:class: important
Defend why your data agrees with or disagrees between each domino characterization. Use error propagation from your uncertainties and precision of your equipment to help your argument.
```


### ● Finalized Spreadsheets

  - Make sure to submit your finalized data table (Excel sheet).

### ● Post-lab Writeup

- In a **paragraph**, summarize your error analysis. Be both qualitative and quantitative.
	- What was the precision of your equipment (calipers, triple beam balance, etc.)?
  <!--- - What are possible systematic errors for today’s experiments? --->
  - What are possible sources of systematic (i.e. affecting accuracy) and random (i.e. affecting variance) errors? How would they change your final results (larger, smaller, more varied)?
  - What are your measured uncertainties, and, based on these uncertainties, how do your final results of $\rho$ change based on those uncertainties?
  - How does the range of densities for an individual domino trial based on measurement uncertainties (i.e. $\rho_{\text{min}}$ and $\rho_{\text{max}}$) compare to the range of densities given by the standard deviation $\sigma$ across colors or across group members? 
     - Larger or smaller? What does this comparison imply about the main sources of error in this experiment?

- In a **paragraph**, summarize the results you have determined in each case. Consider:
  - What were your densities for each of the **different colored dominoes** (based on Analysis Table 1), and did each color agree (within experimental uncertainty assuming the use of standard deviation $\sigma$ as our uncertainty)? In other words, do all the $\rho_{\text{blue-person1}}\pm\sigma_{\text{blue-person1}}$, $\rho_{\text{blue-person2}}\pm\sigma_{\text{blue-person2}}$, etc. agree?
  - Are the average densities of all four dominoes as measured by **each person** consistent (within experimental uncertainty assuming the use of standard deviation $\sigma$ as our uncertainty)? (i.e. do all the $\rho_{\text{blue-person1}}$, $\rho_{\text{green-person1}}$, etc. agree?)
  - Based on your measurements, did you expect the dominoes to float in water (at room temperature)? Did you test it? What did you find, confirmation or disconfirmation of your predictions?

  




## The Whiteboard & Supplemental Info.

Example data tables are shown below to assist you in building your spreadsheet for this first lab. Additionally the original whiteboard summary is at the end of this section.

(common-data)=
### ● Common Data

| Variable (units) | Value |
|------------------------|---|
| Mass precision (SI units) |   |
| Caliper precision (SI units)|   |

---

(trial-data)=
### ● Trial Data

| Trial number | Group Member Initials | Color  | Length (measurement units, mm) | Width (measurement units, mm) | Height (measurement units, mm) | Mass (measurement units, g) | Length (SI units) | Width (SI units) | Height (SI units) | Mass (SI units) | Volume (SI units) | Min Volume (SI units) | Max Volume (SI units) | Volume Uncertainty $\delta V$ (SI units) | Density (SI units) | Min Density (SI units) | Max Density (SI units) | Density Uncertainty $\delta \rho$ (SI units) |
| ------------ | --------------------- | ------ | ------------------------------ | ----------------------------- | ------------------------------ | --------------------------- | ----------------- | ---------------- | ----------------- | --------------- | ----------------- | --------------------- | --------------------- | ------------------ | ------------------ | ---------------------- | ---------------------- | ------------------- |
| 1            | AB                    | pink   |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 2            | AB                    | green  |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 3            | AB                    | orange |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 4            | AB                    | blue   |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 5            | CD                    | pink   |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 6            | CD                    | green  |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 7            | CD                    | orange |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 8            | CD                    | blue   |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 9            | EF                    | pink   |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 10           | EF                    | green  |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 11           | EF                    | orange |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |
| 12           | EF                    | blue   |                                |                               |                                |                             |                   |                  |                   |                 |                   |                       |                       |                    |                    |                        |                        |                     |

---

(analysis-table-1-by-color)=
### ● Analysis Table 1 (by color)

|                | Length (units) | Width (units) | Height (units) | Mass (units) | Volume (units) | Density (units) | Did it float? |
|----------------|--------|-------|--------|------|--------|---------|---------------|
| Avg pink       |        |       |        |      |        |         |               |
| Stdev pink     |        |       |        |      |        |         |               |
| Avg green      |        |       |        |      |        |         |               |
| Stdev green    |        |       |        |      |        |         |               |
| Avg orange     |        |       |        |      |        |         |               |
| Stdev orange   |        |       |        |      |        |         |               |
| Avg blue       |        |       |        |      |        |         |               |
| Stdev blue     |        |       |        |      |        |         |               |

---

(analysis-table-2-by-person)=
### ● Analysis Table 2 (by person)

|         | Length (units) | Width (units) | Height (units) | Mass (units) | Volume (units) | Density (units) |
|---------|--------|-------|--------|------|--------|---------|
| AB avg  |        |       |        |      |        |         |
| AB stdev|        |       |        |      |        |         |
| CD avg  |        |       |        |      |        |         |
| CD stdev|        |       |        |      |        |         |
| EF avg  |        |       |        |      |        |         |
| EF stdev|        |       |        |      |        |         |


### ● Original Whiteboard Info

```{figure} IntroLabFigures/IntroDominos_2024_Fall_01.jpg
:name: introDominoFig
:width: auto
:align: center

Original whiteboard summary
```

