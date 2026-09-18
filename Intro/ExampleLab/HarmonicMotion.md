# || Example Lab: Simple & Damped Harmonic Motion with Springs & Glider on Level Air Track

```{admonition} Review Post-lab Interpretation Questions before lab
:class: important
**❓❓ See {ref}`postlabs_accelGTrack` ❓❓**
```

## Background

### ● Background Overview

```{admonition} OVERALL GOALS
:class: note
Use an frictionless airtrack to:
- Investigate simple harmonic motion
- Investigate damped harmonic motion
```

When the magnitude of the net force acting on a body is linearly related to the displacement of the body and is acting in a direction opposite to the displacement, the body will oscillate in simple harmonic motion around the point where the net force is zero. We will investigate the one-dimensional motion of a mass which is constrained by a net force $F = -k x$. This linearly related force is said to be obeying Hooke's Law. That is to say, if the mass is displaced a distance $x$, a restoring force will act in a direction opposite to the displacement with a magnitude equal to the spring constant, $k$, times the magnitude $x$. The independence of the period on the amplitude and the effect of energy loss mechanisms on the motion will also be examined.

Consider the system illustrated in {numref}`harmonic_motion_Fig01`. The mass is assumed to be resting on a frictionless surface and is constrained by the two springs shown.



```{figure} HarmonicMotionFigures/Figure01.png
:name: harmonic_motion_Fig01
:width: auto
:align: center

System sketch for Harmonic Motion experiment.
```



The springs each apply a force according to Hooke's Law as follows

```{math}
:label: harmonic_motion_F1F2
\begin{aligned}
F_1 &= -k_1 x - F_0\\
F_2 &= -k_2 x + F_0
\end{aligned}
```

When $x = 0$, each spring pulls an equal and opposite amount $F_0$ resulting in a net force of $F = F_1 + F_2 = 0$ at the center equilibrium position.

When the mass is displaced to some point $x$, the net force $F(x)$ is given by

```{math}
:label: harmonic_motion_F1F2combined
F(x) = F_1(x) + F_2(x) = -(k_1 + k_2) x
```

These two springs acting together in this manner produce a force $F(x) = -k_\text{eff} x$, where $k_\text{eff} = k_1 + k_2$, or we can say that the force on the mass acts as if one spring was tied to it with an effective spring constant $k_\text{eff}$.

If we displace the mass to some position $x = A$ and release it at time $t = 0$, we can determine how the mass will move as a function of time under the influence of the restoring force $F(x)$. Using Newton's Second Law and the definition of the acceleration $a$, we can write

```{math}
:label: harmonic_motion_Faccel
F(x) = m a = m \frac{{d}^{2}x}{{d} t^{2}} = -k x
```

In order to find a solution to this equation, we need to find a function $x(t)$ whose second derivative is the same as the function itself, give or take a constant or two. One such function $x(t)$ is


```{math}
:label: harmonic_motion_cosomega
x(t) = A \cos\left(\omega t \right).
```

where $A$ and $\omega$ are constants. In order to evaluate these constants, we observe what the function $x(t)$ must be at known points. One such point is $t = 0$ where $x = A$, that is the release point of the displaced mass. If we substitute the function $x(t)$ into {eq}`harmonic_motion_Faccel`, we will find that it satisfies the equation if

```{math}
:label: harmonic_motion_omega
\omega = \sqrt{\frac{k}{m}}.
```

The quantity $\omega$ is called the angular frequency. From {eq}`harmonic_motion_cosomega`, we see that the position of the mass oscillates between the points $+A$ and $-A$ as the cosine function oscillates between $+1$ and $-1$ as a function of time. The cosine makes one complete oscillation from $+1$ to $-1$ to $+1$ when the quantity $\omega t$ goes through $2\pi$ radians. The elapsed time for this one complete oscillation is $T$, the period. Thus $\omega T = 2 \pi$, or

```{math}
:label: harmonic_motion_omegaperiod
\omega = \frac{2\pi}{T}.
```

If the period is the time it takes the mass to make one complete cycle, the frequency will be $f = (1/T)$ or $\omega = 2\pi f$. Using {eq}`harmonic_motion_omegaperiod` we can write the period as

```{math}
:label: harmonic_motion_period
T = 2 \pi \sqrt{\frac{m}{k}}.
```

*Note* that the **period of oscillation $T$ is independent of the amplitude $A$** of the oscillation for this case where there are *no energy loss mechanisms.*


When the system is started, the mass was displaced a distance $A$ and then released. When the system is displaced that distance $A$, a certain energy is given to the system in the form of potential energy stored in the springs in the amount of $U=(1/2) k A^{2}$. Thereafter, this initial energy is the total mechanical energy of the system, and without any energy loss mechanisms, the total energy remains constant. Thus, as the mass moves, it exchanges potential and kinetic energy. If no energy is lost, the mass will always oscillate between the same amplitude $+A$ and $-A$. It will also have the same maximum kinetic energy which occurs at the $x = 0$, or equilibrium position. You can see from {eq}`harmonic_motion_cosomega` and its derivatives, that the displacement, velocity, and acceleration of the mass are related as:

```{math}
:label: harmonic_motion_xva
\begin{aligned}
x(t) &= A          \cos(\omega t),\\
v(t) &= -A \omega   \sin(\omega t),\\
a(t) &= -A \omega^2 \cos(\omega t).
\end{aligned}
```

The maximum values of $v(t)$ and $a(t)$ are dependent on the amplitude $A$. Assume now that there is some energy loss mechanism present as the mass oscillates, e.g.\ some friction on the surface on which the mass is sliding or some air drag on the mass. If energy is lost to such a nonconservative force, then the total energy of the system will decrease. As the total energy decreases, the amplitude, along with the maximum velocity and acceleration will also decrease. Since neither the period nor the frequency of oscillation are functions of the amplitude, they should remain constant. This kind of motion is called damped harmonic motion.

The opposite effect is also true. If a little bit of energy is added during each cycle, then the total energy of the system will increase and be manifested by an increase in amplitude and still no change in period.




## Experimental Procedure

### ● Preview

```{admonition} OVERVIEW
:class: note
- We study simple harmonic motion and investigate the independence of the period from amplitude during minimal energy loss:
  - Measuring the spring constants of two almost identical springs by applying a known force and measuring the stretching (the displacement) of each of the springs.
  - Determine effective spring constant from the two springs effectively as a single spring acting on a mass on a frictionless surface (i.e. a glider on an airtrack) as illustrated in {numref}`harmonic_motion_Fig01`.
  - Determine the masses' (gliders') periods of oscillation by releasing them from specific displacement points and timing a set of oscillations. This measured period will be compared with the expected value obtained from {eq}`harmonic_motion_period`.
- We also investigate the damped harmonic behavior of the oscillating mass in a case where the energy loss mechanism will be dramatically increased by:
  - Placing a sail on the glider to increase the air drag.
  - Using the same starting amplitude and analyze final amplitudes over increasing time spans by counting larger number of oscillations.
- Each case with have a minimum of either **10** or **15 trials** depending on group size:
  - Each student will complete a total of 5 trials each, with:
    - Groups of 2 --- 10 trials minimum
    - Groups of 3 --- 15 trials minimum
```

```{admonition} Additional Tips
:class: tip
Each group member can measure at the same time to be able to save time while still getting 3 trials per amplitude (if there are groups of two people and you would like additional data, have someone hold two stopwatches to get 3 trials at once).
```


### ● Preliminary Setup & Spring Constants


Before assembling the glider and springs on the airtrack, we must determine the spring constants of the two springs. These very light springs are capable of stretching 20 times their rest length. **Please be very careful not to damage them through careless handling or overstretching.** Create common data table and spring data tables for each of the two springs to measure the spring constant by measuring the extension of the spring at two different displacements from $y_0$ to $\sim 0.95\,\text{m}$ and $\sim 1.55\,\text{m}$.

1. Create a common data table including:
    - $g = 9.803 \,\text{m/s}^2$: Accepted value of acceleration due to gravity for Fairfield University
    - $m_\text{glider}$: masses of large, small, small-with-sail gliders in kg
    - $\delta m_\text{glider}$: uncertainty in masses of large, small, small-with-sail gliders in kg
    - first spring's average spring contant $k_\text{avg,spring1}$ and its uncertainty $\delta k_\text{avg,spring1}$
    - second spring's average spring contant $k_\text{avg,spring2}$ and its uncertainty $\delta k_\text{avg,spring2}$
    - total effective spring constant $k_\text{eff}$ and its uncertainty $\delta k_\text{eff}$
    - expected periods $T$ and their uncertainties $\delta T$ for each of the three glider cases

2. Measure and record the mass and uncertainty with a triple beam balance for:
    - large glider
    - small glider
    - small glider with sail holder and sail
    ```{admonition} Calibration
    :class: tip
    Ensure the balance is **zeroed** before measurements. You can use the adjustment knob on the left side under the silver weighing platform to ensure the pointers at the right end are aligned. See {ref}`triple-beam-balance-overall` for review.
    ```

3. Create the spring-1 data table for the first spring with a row for each displacement trial including columns of:
    - height $y_0$ and its uncertainty of the bottom of the loop on the spring (no mass)
    - applied hanging mass (including hanger) and its uncertainty
    - gravitational force and its uncertainty due to hanging mass
    - height $y_n$ and its uncertainty at the bottom of the loop on the spring with the masses 
    - total displacement $\Delta y$ and its uncertainty due to the applied force
    - spring constant and its uncertainty


```{figure} HarmonicMotionFigures/Figure02.png
:name: harmonic_motion_Fig02
:width: auto
:align: center

Experimental method to measure $\Delta y$ for a spring.
```

4. For each spring, perform the following steps to determine its average spring constant $k_{\text{spring }n}$ from two displacement trials. Refer to {numref}`harmonic_motion_Fig02`.
    - Orient the 2-meter stick with the zero end at the top. It is only the change in $y$ with force that matters in this measurement.
    - Attach one end of the spring to the ring stand and allow the spring to hang free with no mass hanging. Record $y_0 \pm \delta y_0$.
    - Carefully hang enough mass on a weight holder on the end of the spring until it extends a total displacement of $\sim 0.95\,\text{m}$ from $y_0$ and record the exact position $y_1 \pm \delta y_1$ and hangin mass used as $m_1 \pm \delta m_1$ (don't forget the hanger is 50 grams itself). Take the measurements with the spring and any weights hanging stationary.
    - Calculate the applied gravitational force and total displacement $\Delta y_\text{1,spring1} = y_1 - y_0$
    - Calculate the spring constant $k_\text{1,spring1}$ at this first displacement using {eq}`harmonic_motion_Faccel`
    - Add a additional mass to the weight holder on the end of the spring until it extends a total displacement of $\sim 1.55\,\text{m}$ from $y_0$ and record the exact position $y_2$ and mass used as $m_2$ (don't forget the hanger is 50 grams itself). Take the measurements with the spring and any weights hanging stationary.
    - Similarly calculate the applied gravitational force and total displacement $\Delta y_\text{2,spring1}$
    - Similarly calculate the spring constant $k_\text{2,spring1}$ at this second displacement using {eq}`harmonic_motion_Faccel`
    <!---- Calculate two values of $k$ for the current spring using  for each displacement trial. The first is $k_\text{1,spring1} = m_1 g / (y_1 - y_0)$. The second is $k_\text{2,spring1} = m_2 g / (y_2 - y_0)$.--->

5. Repeat the previous steps for the second spring, creating spring-2 data table and determining $k_\text{1,spring2}$ and $k_\text{2,spring2}$ for both displacements.

6. Calculate and record to common data the average spring constants $k_\text{avg,spring1}$ and $k_\text{avg,spring2}$ for each spring.

7. Calculate and record to common data the effective spring constant $k_\text{eff} = k_\text{avg,spring1} + k_\text{avg,spring2}$ that will be acting on the glider.

8. Calculate the expected periods for each glider from {eq}`harmonic_motion_period`.

9. Once the air supply to the airtrack is on, allow it to flow for several minutes to ensure dust and debris have cleared out.

    ```{admonition} Airtrack Air & The Gliders
    :class: warning
    **Do not put a glider on the track without air flowing. If the air supply is not yet on, please remind the instructor, thanks.**
    ```

10. **Level the airtrack.** Without the springs attached and the air track resting directly on the tabletop (with the black circle feet), place one of the gliders on the track (somewhere near center) and note any preferential drift of the glider. Adjust the height of the single leg (screw clockwise in to shorted or counter-clockwise out to lengthen) until the air track is level, as indicated by no preferential drift. Check both orientations of the glider on the track to check if the car is asymmetric and has a significant preferential drift on an otherwise level track. If this occurs, make sure to note that for your discussion purposes. 

    ```{admonition} Drift
    :class: tip
    There will inevitably be some drift as these airtracks are not perfect, but as a general rule of thumb, if it takes more than $\sim 10$ seconds to drift just 5 cm, you should be pretty good.
    ```


11. Now that the springs are characterized and air track is level, assemble the larger glider on the track and attach the springs to the glider and the ends of the track as in {numref}`harmonic_motion_Fig01`. **Again please be careful not to overstretch the springs or allow them to snap back. Keep towards center.**

(hamronic-motion-case1)=
### ● CASE 1: Large Glider


12. Create a data table for the measurement of oscillations of the large glider on the air track. You can copy and paste for later cases after you confirm all calculations and methods are accurate. Create enough rows for as many trials --- (e.g. three repetitions (trials) for each of the five initial amplitudes would be 15) including columns for:
    - Trial number
    - Lab member's initials
    - $x_0$: Equilibrium position on track scale
    - $x_A$: Starting position on track scale at amplitude (that achieves a $\sim0.10, 0.15, 0.2, 0.25, 0.3\,\text{m}$ displacement from equilibrium)
    - $A$: Starting amplitude (displacement from equilibrium) in meters
    - Time for ten cycles
    - $T$: Determined period
    - Additional rows for mean and standard deviation of the period


    ```{admonition} Position Measurements
    :class: tip
    There is a ruler built into the airtrack. Use that scale and a consistent corner of the glider to determine various displacements along the track
    ```



13. To determine the period of oscillation of the mass:
    - Displace the mass an amplitude of $A \approx 10\,\text{cm}$ from its equilibrium position, record this position $x_A$, calculate and confirm the starting amplitude from $A = |x_A - x_0|$.
    - Satisfied with your displacement position, release the glider. When the mass returns to its starting point, start the stopwatch ***(available at front table)*** at the zero velocity point (e.g. $A$). Allow the mass to oscillate through 10 complete cycles and stop the stopwatch at the zero velocity point at the end of the tenth cycle (essentially the same position as the starting point). Record the time for the ten cycles and divide by the number of cycles counted to obtain the period. **NOTE:** Each group member will measure at the same time to be able to save time while still getting 3 trials per amplitude (if there are groups of two people and you would like additional data, have someone hold two stopwatches to get 3 trials at once).

      ```{admonition} Suggestion for Counting: Index at 0
      :class: tip
      If you index your counting by starting at 0, where you would start the stopwatch when you say zero, and stop the stopwatch when you say ten, you will have counted 10 full cycles.
      ```

14. Use the same glider and repeat for $A \approx 15, 20, 25, 30\,\text{cm}$ starting amplitudes.

15. Compare your experimentally determined periods for different starting amplitudes to the large glider's expected period.

    ```{admonition} Continue to additional case?
    :class: warning
    ***If you are satisfied that all your calculations are complete and results seem reasonable (feel free to check with your professor), it is only at this point that you should continue to the next case.***
    ```


### ● CASE 2: Small Glider

16. Reassemble the system with the smaller glider ***without*** the sail assembly on the track ({numref}`harmonic_motion_Fig01`).
17. As in {ref}`hamronic-motion-case1`, build a data table and use the same measuring techniques to determine the period for starting amplitudes of $A \approx 10, 15, 20, 25, 30\,\text{cm.}$ Record the time for ten cycles and divide by the number of cycles counted to obtain the period.
18. Again, compare your experimentally determined periods for different starting amplitudes to the small glider's expected period.


### ● CASE 3: Small Glider with Sail

**The third experiment in this lab focuses on measuring the damped oscillation of the small glider WITH A SAIL.** Instead of starting at different amplitudes, you will start from the same starting amplitude $A \approx 25\,\text{cm}$. You will count across a range of oscillations, from 5 up to 30 oscillations, to determine how much the final amplitude changes over time.

19. Create a data table for the measurement of oscillations of the small glider ***with a sail*** on the air track. There will be 6 trials, one for each range of oscillations $(n_\text{cycles} = 5, 10, 15, 20, 25, 30)$. Create enough rows for as many trials including:
    - $n_\text{cycles}$: number of cycles
    - $x_0$: equilibrium position
    - $x_A$: starting position
    - $A$: starting amplitude $\sim 25\,\text{cm}$
    - $x_\text{final}$: final position after $n$ cycles
    - $A_\text{final}$: final amplitude (final position minus equilibrium position)
    - the total time
    - the average period



20. Place the paper sail assembly on the small glider. **Only 1 trial needed per number of cycles.**

21. Use a single starting amplitude of $\sim25\,\text{cm}$ from the equilibrium position. Record both the equilibrium position and your starting position; determine and record the amplitude from $A = |x_A - x_0|$ (should be $\sim 25\,\text{cm).}$ Each of the following steps will be started from this same starting position and amplitude.

22. Displace the glider with its sail to the starting position and release it. 
    - When the mass returns to its starting point, start the stopwatch at the zero velocity point (e.g. $A$). 
    - At the end of the fifth cycle, stop the stopwatch and capture the glider by gently pressing your finger on the edge of the glider as gets to its maximum amplitude point, i.e. when $v = 0$. **Note:** Be sure to use the same point on the glider that you used to determine the equilibrium point and the $25\,\text{cm}$ starting point.
    - Record the final position and calculate the final amplitude $A_\text{final}$.
    - Record the total time for the current trial, divide by the $n_\text{cycles}$ measured to obtain the average period. 
    - Compare this with the expected period from {eq}`harmonic_motion_period`, remembering the total mass of the glider plus sail assembly.

23. Repeat previous steps five more times, each time starting the glider from the same starting amplitude, and allow the glider to oscillate five additional cycles more than the previous measurement. **Only 1 trial needed per number of cycles.**


### ● Graphical Analysis

24. For Case 1 and 2, plot the period $T$ ($y$-axis) vs. the *starting* amplitude $A$ ($x$-axis). Include trendline.

25. For Case 3
    - Plot the period $T$ ($y$-axis) vs. the *final* amplitude $A_\text{final}$ ($x$-axis). Include trendline.
    - Plot the *final* amplitude $A_\text{final}$ vs. $n_\text{cycles}$.

<!---
     Use the starting amplitude $A_0$ as the value for zero cycles.
- Draw a line-of-best-fit through the data points for each plot.
--->


### ● Summary & Cleanup

26. Create a summary table of your data (e.g. relevant final result values, averages, and differences from each case).

27. When you are finished, reset your experimental setup before leaving.

    ```{admonition} CLEAN UP
    :class: important
    Please return your experimental station back to the way you found it or better:
      - Remove gliders and springs from the airtrack
      - Remove sail from small glider
      - Re-hang springs up on the main pole
      - Return stopwatches, masses, hangers to front table
      - Return 2 m rulers back to front wall
    ```




## Post-Lab Submission — Interpretation of Results

```{admonition} Defend your conclusions with your data
:class: important
Defend why your data agrees with or disagrees with the actual value of $g$ and pendulum physics. Use error propagation from your uncertainties and precision of your equipment to help your argument.
```


### ● Finalized Spreadsheets

  - Make sure to submit your finalized data table (Excel sheet).
    - Please include relevant plot(s) including:
      - Cases 1 & 2:
        - $T$ vs. $A$
      - Case 3:
        - $T$ vs. $A_\text{final}$
        - $A_\text{final}$ vs. $n_\text{cycles}$


### ● Post-lab Writeup

- In a **paragraph**, summarize your error analysis. Be both qualitative and quantitative.
  - What is the precision of your equipment?
  - What are possible sources of systematic (i.e. affecting accuracy) and random (i.e. affecting variance) errors?
    - Discuss those from spring characterization
    - Discuss those in the *undamped* cases
    - Discuss those in the *damped* case
  - How do your measured uncertainties in hanging mass and spring constants affect your expected periods; by how much; which showed a larger impact?

  
- In a **paragraph**, summarize the results you have determined in each case. Consider:
  - For all three cases, how do the the measured periods of the glider compare to expected periods? I.e. do they agree within uncertainty and standard deviation ranges?
  - Comment (qualitatively) on the behavior of the curves from each plot. Do the trends make sense? Explain with physical concepts.
    - From the damped-oscillator plot, what do you expect amplitude of the glider to be after 50 cycles?
  - Does the amplitude affect the period? Why or why not? Argue a physical answer supported by your data; discuss whether your data supports the theory for:
    - An *undamped oscillator*
    - An *damped oscillator*
  - How does the period depend on the mass of the glider? Is this expected?
  - How does an increased air drag affect the result for the period?
  - How does the amplitude depend on the number of cycles (relate this to energy conservation)?




## The Whiteboard


```{figure} HarmonicMotionFigures/2024_Fall_SHM_01.jpg
:name: harmonic_motion_whiteboard_01
:width: auto
:align: center

Overview for spring constants.
```

```{figure} HarmonicMotionFigures/2024_Fall_SHM_02.jpg
:name: harmonic_motion_whiteboard_02
:width: auto
:align: center

Overview for oscillations of simple harmonic motion and damped harmonic motion.
```

```{figure} HarmonicMotionFigures/2024_Fall_SHM_03.jpg
:name: harmonic_motion_whiteboard_03
:width: auto
:align: center

Amplitude measured from equilibrium $A_0$ in image, $x_0$ position used in procedure. Cycle counting suggestions.
```