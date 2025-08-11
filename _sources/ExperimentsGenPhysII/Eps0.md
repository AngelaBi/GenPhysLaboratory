# Electric Force and the Determination of $\varepsilon_0$

```{danger}
**⚠️⚠️⚠️⚠️ WARNING ⚠️⚠️⚠️⚠️**

**⚠️⚠️⚠️⚠️ HIGH VOLTAGE IN USE TODAY ⚠️⚠️⚠️⚠️**

**⚠️⚠️⚠️⚠️ DO NOT TOUCH THE METAL PLATES ⚠️⚠️⚠️⚠️**

**⚠️⚠️⚠️⚠️ YOU CAN GET SERIOUSLY INJURED ⚠️⚠️⚠️⚠️**

**⚠️⚠️⚠️⚠️ WARNING ⚠️⚠️⚠️⚠️**
```

## Background

### Overall goals and overview

- **OVERALL GOALS and Overview:**
  - Experimentally determine the electric constant $\varepsilon_0$
  - Understand the relationship between electric force $F_E$ and voltage $V$ (i.e. $F_E$ vs. $V$) using a uniform electric field, reasonably produced by a parallel-plate capacitor.
  - Conduct three rounds of six trials each (total 18 trials) of applying less mass (less gravitational force) and more voltage to produce an electric field (and therefore more electric force). Do the rounds sequentially rather than all of a single applied mass in a row to ensure you catch and correct any significant errors early (e.g. if the apparatus is bumped out of alignment) rather than having to do all 18 trials again. The order of the trials for applied masses would be 50, 40, 30, 20, 10, 0, 50, 40, 30, 20, 10, 0, 50, 40, 30, 20, 10, 0 mg.
  - In this experiment, first determine the separation distance, $d$. Then replace the equilibrium mass with a series of smaller masses and apply the necessary voltage $V$ applied across the plates so they return to parallel where the separation distance returns to $d$. Under this condition, the electric force required to maintain the separation $d$ will be the difference of the gravitational force on the 50 mg mass and on the smaller mass. Then determine $\varepsilon_0$ through both averaging of all your trials and plotting of all your data (i.e. electric force vs. voltage between the plates). Comparing then your results from both analysis methods to the accepted $\varepsilon_{0\text{-accepted}}$.

The electric constant (a.k.a. vacuum permittivity, permittivity of free space, or dielectric permittivity of the vacuum), $\varepsilon_0$, is a fundamental constant of nature. It is the proportionality constant that relates the electric force between two charges. The constant $\varepsilon_0$ is also related to the constant $k$ in Coulomb's Law

```{math}
:label: eq_coulomb_basic
F = F_\text{electric} = F_E = k\frac{Q_1 Q_2}{r^2},
```

where $Q$ is the charge in Coulombs, $r$ is the separation distance in meters, and

```{math}
:label: eq_k_epsilon
k = \frac{1}{4 \pi \varepsilon_0}.
```

The subscript zero refers to the value of the permittivity of free space. **Note: You will experimentally determine $\varepsilon_0$ today;** later in Lab E-6, you will determine its magnetic equivalent, $\mu_0$. Using both, we will be able to determine the magnitude of the velocity of propagation of an electromagnetic wave, i.e., the speed of light as part of Lab E-6. In any medium, $\varepsilon$ and the speed of light $c$ will depend on the particular material.

If we apply Coulomb's law to the special case of two large, closely-spaced, parallel plates (example from setup shown in {numref}`E1Fig_00`), we can derive an expression for the electric force between the two plates. [You should review this derivation in your text and class notes.] This configuration is known as the 'parallel-plate capacitor.'

```{figure} Eps0Figures/fig_00_OverallApparatus_v02.png
---
width: 600px
name: E1Fig_00
---
Top) Example of the entire setup. Bottom) Front view of capacitor apparatus; protective box.
```

Under this assumption of a parallel-plate capacitor, the electric field is uniform with a magnitude $E = \frac{V}{d}$, with $V$ as the voltage (potential difference) between the plates, and $d$ the separation distance. The electric force of attraction between two oppositely charged plates is then

```{math}
:label: eq_electric_force
F_E = \frac{\varepsilon_0 A V^{2}}{2 d^{2}}
```

where $A$ is the area of the plates, $d$ the separation distance, and $V$ the potential difference in volts across the plates.

*{eq}`eq_electric_force` is valid only under the conditions stated of large, closely spaced plates to provide a uniform electric field and charge density so we can effectively ignore fringe fields*. The physical implications of these geometric assumptions is that the electric field is totally confined to the space between the plates and is constant in value throughout the space. You will see in Lab E-2 that the electric field always 'bulges' or fringes out at the edge. For {eq}`eq_electric_force`, the fringe field is ignored. Rewriting the expression for $\varepsilon_0$, we obtain

```{math}
:label: eq_epsilon_0
\varepsilon_0 = \frac{2 F_E d^{2}}{A V^{2}}.
```

By measuring electric force, voltage, and geometry of the apparatus, $\varepsilon_0$ can be determined.


```{figure} Eps0Figures/fig_01_Apparatus_v03.png
---
width: 600px
name: E1Fig_01
---
Parallel Plate Capacitor Apparatus. Top-left) Schematic showing dimensions. Top-right) Plate separation when parallel. Middle) Example apparatus with dimensions. Bottom) Example of mirror-to-scale distance.
```

### Equipment

Depicted in {numref}`E1Fig_00` -- {numref}`E1Fig_02`.

- Telescope with crosshair & centimeter-scale ruler (a.k.a. scale) on vertical pole
- High voltage DC power supply, 0 -- 500 V
- Fluke multimeter -- set to read DC voltage
- Small masses of 1 -- 500 mg, plastic tweezers
- Parallel-plate capacitor apparatus:
  - Bottom plate held in static position on lower plate adjustment towers
  - Balance beam balancing on thin, conductive, knife edges with:
        \begin{itemize}
            \item Top plate with a ``$+$" for where to place applied masses. Can swing up or down when changing amount of applied mass or voltage. Set up to be parallel (at equilibrium) to bottom plate when holding 50~\milli\gram
            \item Mirror to view the scale (ruler) via telescope to determine angle and distance $d$ between plates
            \item Beam lift knobs to reset top plate position
            \item High impedance $1~\mega\ohm$ resistor to limit current (contained in long gray box, shouldn't need to touch)
        \end{itemize}
    - Leveling screws to level whole apparatus to the table
    - Metal connections to the power supply
  - x4 Banana plug wires (12 AWG) connecting power supply to voltmeter & parallel-plate apparatus
  - Protective box with the mirror-to-scale distance $b$ written on it

### Adjustment of apparatus

The apparatus has been carefully adjusted before your lab and should not require further significant adjustments. This section describes how the apparatus was prepared. If something seems to need adjusting, see the lab instructor.

1. The beam lift (knob location noted in {numref}`E1Fig_00` bottom-left) provides a definite location for the beam and thus guarantees continued alignment of the parallel plates. Use the beam lift each time you change weights or relocate the counter weight.
2. Both plates can be adjusted vertically and horizontally in order to make it possible for the plates to be parallel. The counterweight behind the mirror can be used to establish the equilibrium separation of the plates. The plates should have already been adjusted parallel with the counterweight set so the plates are essentially parallel when a 50 mg mass is placed on the movable plate. *If the plates are NOT parallel with the 50 mg mass in place, seek the instructor's help.*
3. The apparatus can be leveled with the leveling screws so that it sits flat on the table.
4. Mirror-to-scale distance was measured from rear of mirror (reflective surface) to ~center of $S_0$ and $S_1$ on the scale (ruler).

## Experimental Procedure

```{danger}
**⚠️⚠️⚠️⚠️ DO NOT TOUCH THE METAL PLATES ⚠️⚠️⚠️⚠️**
```

1. Prepare a common data table including given values.
   Reminder -- keep variable names and units in the row and column titles, and numbers in their own Excel cells to be able to reference in your equations. **Run all your calculations in your Excel sheet so your instructor can see how you arrived at your final results**. Include:
   - Accepted value of $g = 9.803 \,\text{m/s}^2$ for Fairfield University
    \item Accepted value of $\varepsilon_0 = 8.8542\times 10^{-12}\,\coulomb\squared\per\newton\per\meter\squared$
%    \item Length of the frame $a \pm \delta a=0.279\pm0.001\,\meter$ (see Fig.~\ref{E1Fig:01})
    \item Length of the frame $a=0.279\,\meter$ (see Fig.~\ref{E1Fig:01})
%    \item Mirror-to-scale distance $b \pm \delta b = b \pm 0.003\meter$, has already been measured and is posted on the top of the protective enclosure (ex. in Fig.~\ref{E1Fig:01} bottom)
    \item Mirror-to-scale distance $b$ has already been measured and is posted on the top of the protective enclosure (ex. in Fig.~\ref{E1Fig:01} bottom)
%    \item Plate area $A \pm \delta A =0.0161\pm0.0002\,\meter^2$ (see Fig.~\ref{E1Fig:01})
    \item Plate area $A=0.0161\,\meter^2$ (see Fig.~\ref{E1Fig:01})
   - Equilibrium mass $m_0 = 50$ mg (plates are parallel when this amount of mass applied).
   - Equilibrium force $F_0 = m_0 g$
   - Scale reading at equilibrium $S_{0}$
   - Scale reading when plates are in contact $S_{1}$
   - Separation distance $d$
     between the plates when the top plate is parallel to the bottom plate when a 50 mg mass is placed on the top plate (see examples in {numref}`E1Fig_01` top-right and {numref}`E1Fig_02` middle)

2. **Do not turn on the power supply until told to do so in the steps below.**
3. Note the center marking "+" on the top of the movable plate where masses must be placed using the tweezers (see {numref}`E1Fig_03`).

```{figure} Eps0Figures/fig_03_MassPlacement.png
---
width: 600px
name: E1Fig_03
---
Example of masses to use (milligrams). Placement location marked by the +.
```

4. Investigate the use of the telescope and scale so that the rotation of the balanced frame can be measured in terms of scale divisions (see {numref}`E1Fig_02`). Numbers are in cm, small lines in mm.

```{figure} Eps0Figures/fig_02_MeasuringApparatus_v02.png
---
width: 630px
name: E1Fig_02
---
Top-left) Schematic of the Measuring Apparatus. Top-right) Example of S₀ and S₁ on the scale. Bottom) Example of the plates and cross-hairs through the telescope for finding S₀, S₁, D.
```

5. Determine separation distance $d$ of the plates when they are essentially parallel. To do so, perform a geometrical analysis that describes the vertical displacement of the plate as given by

```{math}
:label: eq_distance_d
d = \frac{D a}{2 b}
```

where $D$ is the change in scale reading between when the equilibrium mass is on the plate and when the plates are in contact (example shown in {numref}`E1Fig_02`) and $a$ and $b$ as described earlier (further described in {numref}`E1Fig_01`). The factor of 2 results from the fact that the optical path reflected off of the mirror to the scale rotates through an angle twice that of the beam holding the movable plate. Determine $D = | S_1 - S_0 |$ from two scale readings (reminders: absolute value there is to represent the total distance between $S_0$ and $S_1$. If your crosshair crosses 0, make sure to consider the negative).

   - The first scale reading, $S_0$, is made when the separation of the plates is such that the plates are essentially parallel. This should happen when a mass of 50 mg is on the movable plate. If not, call over an instructor.
   - The second scale reading, $S_1$, is made when the top plate contacts the bottom plate ({numref}`E1Fig_02`). Place a sufficient mass (~500 mg) on the movable plate to make it contact the lower, stationary plate.
   - You should periodically verify that $S_0$ and $S_1$ are not changed.
   - Record $S_0$, $S_1$, and $D = | S_1 - S_0 |$ in your common data table.
   - Also include the equilibrium mass $m_0$, the equilibrium force ${F_0 = m_0 g}$, the distance $a$, the distance $b$ found on the apparatus cover.
   - Calculate the plate spacing $d$ using {eq}`eq_distance_d`.   
\item We can now determine an experimental value of $\varepsilon_0$ from the values in the common data table and the experimental voltage from each trial. You will perform at least three trials for each of six cases of different applied masses on the movable plate (18 total trials). Set up an experimental data table to record your measurements and calculate the experimental value of $\varepsilon_0$. Include enough rows for trials and columns for:
\begin{itemize}
    \item Applied mass $m_{\text{applied}}$
%    \item Applied mass uncertainty $\delta m_{\text{applied}} = 0.01 \times m_{\text{applied}}$ (i.e. 1\%)
    \item Applied force $F_{\text{applied}}=m_{\text{applied}} g$
%    \item Uncertainty in the applied force $\delta F_{\text{applied}} = (m_{\text{applied}} + \delta m_{\text{applied}})g - F_{\text{applied}}$. This comes from the difference in a maximized value for the applied force and your value for the applied force.
    \item Electric force $F_E$ as the difference between the equilibrium force and the applied force $F_E=F_0 - F_{\text{applied}}$
   - Voltage $V$ required to return to the equilibrium position
   - Experimental value of the electric constant $\varepsilon_{0\text{-experimental}}$ as calculated using {eq}`eq_epsilon_0`.

6. Repeat the following steps for each trial with applied masses in order (to catch any procedural issues early): 50, 40, 30, 20, 10, 0, 50, 40, 30, 20, 10, 0, 50, 40, 30, 20, 10, 0 mg. Replace the equilibrium mass in the center of the top plate with the mass required for each trial. The top plate will swing upwards.

```{figure} Eps0Figures/fig_04_spark.png
---
width: 600px
name: E1Fig_04
---
Safety note regarding electricity and the plates touching.
```

7. Turn on the power supply and slowly increase the voltage until the plate separation is reduced back to the equilibrium value, $S_0$, as it was with 50 mg on the top plate (determined by watching the scale reading with the telescope). The telescope observer should be calling out instructions to the power supply operator to slowly approach the $S_0$ value. When the $S_0$ value is reached, call out immediately for a voltage reading and record the voltage. Since the electric force will increase with decreasing separation, as seen from {eq}`eq_electric_force`, the plates have a tendency to continue through the $S_0$ point towards the zero separation point $S_1$. $S_0$ is an unstable equilibrium point. This may result in the plates sticking together and sparking as seen in {numref}`E1Fig_04`. If the plates stick together, **DO NOT TOUCH THE APPARATUS TO SEPARATE THE PLATES**. Turn off the power supply and tap the table in front of the apparatus; the plates should separate themselves. Accurate readings require care that the telescope and scale are not moved during the experiment. Note: If the voltmeter display times out and goes blank, turn it off and on and reset the voltmeter to DC volts (sleep function).

8. Reduce the voltage to zero and turn off the power supply. You should periodically check that $S_0$ and $S_1$ have not changed during your experiment.

9. Record the values for: the applied mass and voltage required for equilibrium. Calculate the applied force, the difference between the equilibrium force and the applied force (electric force), and the value of $\varepsilon_{0_\text{experimental}}$ calculated using {eq}`eq_epsilon_0`.

10. Repeat Steps 7 through 9 for each subsequent trial and record corresponding values.

11. Check if all the values are reasonably consistent. Retake any data that are clearly erroneous and recalculate.

12. Add rows to your data table for calculating:
    - Average $\varepsilon_{0_\text{experimental-average}}$
    - Standard deviation $\sigma_{\varepsilon_{\text{0-experimental-average}}}$ (treating this as your overall uncertainty of your average value, e.g. avg ± σ. *Consider: does your experimental value ± range overlap with the accepted value of $\varepsilon_{0}$?*

13. **Graphical Analysis:** The graphical display of data permits the comparison of all the values and associated errors at once. Points that depart markedly from the general trend of the data are quickly detected. We expect from theory (from {eq}`eq_electric_force`) that electric force and voltage are related like:

```{math}
:label: eq_force_voltage
F_E = \alpha V^{2}.
```

    a. Using **all** of your data points from **all cases and trials**, ***scatter plot*** $F_E$ as ordinate ($y$) and $V^{2}$ as abscissa ($x$). Fit a trend line through the all these points, display the trendline equation on the chart, and confirm the slope of the line $\alpha$ matches what you found with the LINEST() function. From {eq}`eq_electric_force`, the value of $\alpha$ is given by

```{math}
:label: eq_alpha
\alpha = \varepsilon_0\frac{A}{2 d^2}.
```

$\varepsilon_0$ can now be determined by rearranging {eq}`eq_alpha` and using this experimentally determined value $\alpha$. Thus

```{math}
:label: eq_epsilon_from_alpha
\varepsilon_0 = \frac{2 \alpha d^2}{A}.
```

    b. Your best fit line to $F_E$ versus $x=V^{2}$ should theoretically pass though the origin. Change the fit to force the line to have a $y$ intercept of 0. Recalculate your value of $\varepsilon_0$ as above. 

## Post-Lab Submission --- Interpretation of Results

- Make sure to submit your finalized data sheet with summarized data and cleaned-up plots (Excel sheet)
- Paragraph of your results +/- uncertainties from your data. Make sure to include discussion of the following:
  - Do your experimental results agree with the accepted value for $\varepsilon_0 = 8.8542 \times 10^{-12} \,\text{C}^2/\text{N}/\text{m}^2$?
  - Does your linear (Y-int calculated normally) or linear-through-origin (Y-int = 0) plot more accurately represent the physical relationship between electric force and potential difference?
  - Explain physically why you would expect the linear fit to go through the origin of the $F_E$ vs. $V^2$ plot?
- Paragraph of your errors and estimated measurement uncertainties. Be quantitative. Make sure to include discussion of the following:
  - Where might systematic (affecting accuracy) and/or random (affecting precision) errors be coming from?
  - What are your measurement uncertainties, and, based on these uncertainties, how do your final results change? I.e. do your different measurement and slope uncertainties make your final results of $\varepsilon_0$ larger or smaller?
  - Change different variables by your best estimation of measurement uncertainties in your Excel sheet; what variables affect the accuracy of your final results the most?
  - If larger or smaller, are your final results more or less comparable to expected values?
  - How could you improve your random errors?
  - Based on the comparison between your experimental value ± std. dev. and the accepted value, were your systematic errors significant? How could this be improved if you were to re-run this experiment?
- Reflect on this week's lab; what did you learn?
