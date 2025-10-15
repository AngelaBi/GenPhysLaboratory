(centripetal-force-lab-overall)=
# Centripetal Force with Mass on Rotating Arm

## Background

```{admonition} OVERALL GOALS
:class: note
In this lab, you will:
- Investigate centripetal forces and determine mass of a object rotating in uniform circular motion by measuring the centripetal force across different, constant, tangential velocities and compare to actual mass from triple-beam balance.
```


Acceleration is the rate of change of velocity. An object moving in a circle of radius $R$ is always being accelerated even if its speed remains constant. This is because velocity is a vector quantity whose direction is continuously changing. This rotational change in direction requires a centripetal force that is pointed in towards the axis of rotation (center-seeking). The corresponding centripetal acceleration also points toward the axis of rotation with a magnitude $a_\text{c} = v^{2}/R$. For an object of mass $M_\text{object}$, the required force for this circular motion is thus related quadratically to the speed of the object and inversely to its radius of curvature:

```{math}
:label: eq-centripetal-force
F_{c} = M_\text{object} \frac{v^2}{R}
```

For each case, the object’s mass $M_\text{object}$ and radius $R$ are set by attaching small masses to a freely-sliding holder on the rotating arm (shown in {numref}`M04Fig01`). The tangential speed of the object $v$ is obtained from the rate at which a small white-ish pin beneath the fixed-in-place counterweight holder passes through the photogate. The centripetal force is determined by measuring the force in the cable with a force sensor (seen later in {numref}`M04Fig02`). Subsequently, the $M_\text{object}$ is determined from graphs relating $F$ vs. $v^2$ and $F$ vs. $v$. The procedure is repeated for different masses and radii to study how centripetal force depends on velocity.

```{figure} CentripetalForceFigures/Figure01a_v2025-02.png
:name: M04Fig01
:width: 100%
:align: center

Experimental Setup showing the rotating arm and the attached masses. The photogate to measure the speed is shown as well. The small white-ish pin attached underneath the fixed-counterweight mass holder is used to determine the speed $v$ of the mass.
```



## Experimental Procedure


```{admonition} OVERVIEW
:class: note
- Investigate how tangential velocity and centripetal forces are related.
- Experimentally determine the mass of a rotating object by measuring the centripetal forces and determining the tangential velocities.
- Conduct 4 cases based on 2 applied masses and 2 radii.
  - Each case will have a total of 3 trials.
- Compare the experimental results to the actual values as measured with triple-beam balance.
```

```{admonition} Notes
:class: note
- Time measured by PASCO photogate for velocity calculation in **Capstone** (stated precision of 0.0001 seconds).
- Force measured by PASCO High-Resolution Force Sensor (stated precision of 0.002 N).
- The relevant Capstone file will be on the desktop. Please ***DO NOT*** save when you are done, just exit without saving, thanks.
```

(centripetal-force-experimentPrep)=
### Preliminary Setup

```{figure} CentripetalForceFigures/Figure02_v2025-02.png
:name: M04Fig02
:width: 100%
:align: center

Experimental Setup for the centripetal force experiment
```

1. The experiment should already be setup for you as shown in {numref}`M04Fig02` with masses attached to both the freely-sliding and fixed-counterweight mass holders a s well as already being hooked up to the computer interface and power supply. Reminder, the relevant Capstone file will be on the desktop (e.g. {numref}`M04Fig07`).

    ```{figure} CentripetalForceFigures/Figure07_v2025-01.png
    :name: M04Fig07
    :width: 80%
    :align: center

    Example of today's **Capstone** layout. Review notes for helpful info.
    ```

2. Create a common data table including (but not limited to):
    - the mass of the freely-sliding mass holder holder (kg)
    - uncertainty of the mass of the freely-sliding mass holder holder (kg)

3. Remove the freely-sliding mass holder and measure its mass with a triple-beam balance. Record this in your data sheet. Put the freely-sliding mass holder back on the rotating arm in the order shown in {numref}`M04Fig04`.

    ```{figure} CentripetalForceFigures/Figure04_v2025-02.png
    :name: M04Fig04
    :width: 100%
    :align: center

    Reassemly procedure for reattaching the freely-sliding mass holder
    ```


4. Four cases will be performed, each with 3 trials, as listed in {numref}`tab-four-centripetal-force-cases`. For each of the four cases, perform the following steps listed in {ref}`detailsteps-centripetal-force` and record the data appropriately in your spreadsheet.

    ```{table} Four experimental cases applied masses and radii
    :name: tab-four-centripetal-force-cases
    | Case | Applied Mass (g) | Radius (mm) |
    |:----:|:-----------:|:-----------:|
    |  1   |    5      |   small ($\sim60-70$)      |
    |  2   |    15      |    small ($\sim60-70$)      |
    |  3   |   5     |   BIG ($\sim95-105$)      |
    |  4   |   15     |    BIG ($\sim95-105$)      |
    ```


    ```{admonition} Reminder, Run First Case Fully
    :class: warning
    Reminder, run your first case completely **before** moving on to additional cases. Don't just take all of your data without checking your methodology. If you have some error in your experimental method or in your calculations, you can correct it before completing all the other cases and finding out you have to completely redo the whole lab. The data tables for additional cases can be created by copying the first case **after** you are confident in and can explain your results from the first case.
    ```

(detailsteps-centripetal-force)=
### Experimental Data Collection


4. For each case, construct a table with a row for each trial and columns including (but not limited to):

    - $R$: the radius (m)
    - the applied mass (kg)
    - $M_\text{object,actual}$: actual mass of the rotating, freely-sliding object 
    - $m$: fit parameter $m$ from the $F_\text{c}$ vs. $v^2$ (linear fit)
    - $M_\text{object,experimental,linear}$: the mass determined from $F_\text{c}$ vs. $v^2$
    - the difference between $M_\text{object,experimental,linear}$ and $M_\text{object,actual}$
    - $A$: fit parameter $A$ from the $F_\text{c}$ vs. $v$ (quadratic fit)
    - $M_\text{object,experimental,quadratic}$: the mass determined from $F_\text{c}$ vs. $v$
    - the difference between $M_\text{object,experimental,quadratic}$ and $M_\text{object,actual}$
    - $\delta R$: your estimate of the uncertainty in the radius (m) (i.e. $\text{radius} \pm \delta R$)
    - $\delta M_\text{object,experimental}$ the uncertainty in the mass from the centripetal force due to your estimated radius uncertainty (*Point to consider*: how much does the derived mass change if you change your value for radius in **Capstone calculator** by the amount of your estimated radius uncertainty?)


5. Set radius $R$ by raising or lowering the force sensor. Measure the radius of the freely-sliding rotating object 

3. Select **Calculator** in the menu on the left-hand side on the **Capstone** interface. This will open a window (example shown in {numref}`M04Fig03`) where you can update the radius to match the actual radius of your masses. *NOTE*: that the value for the radius will change in the experiment, and you need to adjust the value in **Capstone** when you switch to the new radius. After setting the radius in the calculator, close the setup window by clicking on the **Calculator** button again.

    ```{figure} CentripetalForceFigures/Figure03_v2025-01.png
    :name: M04Fig03
    :width: 80%
    :align: center

    Calculator setup in **Capstone** to determine the speed of the rotating objects. Make sure to adjust the value for the radius in this window to the actual value used in your experimental setup.
    ```


5. There are graphs set up for you in **Capstone** plotting
   - $F$ versus $v^2$
   - $F$ versus $v$

6. Before data recording starts
   - Zero the force sensor with the zero button (physically on the force sensor) while the connecting cable is slack

7. Start the data acquisition on **Capstone** by pressing the **Record** button.
   You should notice that the program will start to record values.

8. Slowly increase the voltage on the power supply from 0V to 10V over the course of about 30 seconds.
   The metal arm will start to rotate and you will notice the graphs display the data as it is collected.
   Do not exceed 10 V and turn off the data acquisition (by pressing the **Record** button again) **before** returning the power supply to zero.

9. Once you have finished your run, fit a line to your $F$ vs. $v^2$ graph.
   Select the fit box.
   In the Curve Fit Editor, lock the intercept $b = 0$.
   Notice the change in $m$ when you lock $b$. Record the slope $m$ in the Data Table.

10. Fit a Quadratic curve to your $F$ vs. $v$ graph.
    Fit the curve $F=A v^2$ by locking B and C to zero. Notice the change in A when you lock B and C.
    Discuss why B and C should be zero. Record A in the Data Table.

DISCUSSION POINT
	- Do the graphs display the expected behavior?

11. Repeat the measurement two more times.
    Calculate the average fit parameters for the three runs.

12. Determine $m$, the value of the rotating mass from both graphs and note the result in your data table.
    Explain how you determine the value from your data.
Note all results in your data table. Discuss why you also need to adjust the fixed-counterweight mass holder and not just the freely-sliding mass holder.


```{figure} CentripetalForceFigures/Figure05_v2025-01.png
:name: M04Fig05
:width: 80%
:align: center

!!!!!!!!Setup of the data acquisition system **Capstone** to measure the speed of the rotating masses. Make sure to adjust the value for the radius in this window to the actual value used in your experimental setup.
```

```{figure} CentripetalForceFigures/Figure06_v2025-01.png
:name: M04Fig06
:width: 80%
:align: center

!!!!!!!!Setup of the data acquisition system **Capstone** to measure the speed of the rotating masses. Make sure to adjust the value for the radius in this window to the actual value used in your experimental setup.
```



```{figure} CentripetalForceFigures/Figure08_v2025-01.png
:name: M04Fig08
:width: 80%
:align: center

!!!!!!!!Setup of the data acquisition system **Capstone** to measure the speed of the rotating masses. Make sure to adjust the value for the radius in this window to the actual value used in your experimental setup.
```

13. Repeat the previous steps ({ref}`detailsteps-centripetal-force`) for the next case with the relevant applied mass and radius as listed in {numref}`tab-four-centripetal-force-cases`. Please call for help as needed for setting up next cases.

    ```{admonition} Continue to additional case?
    :class: warning
    ***If you are satisfied that your calculations and ***error propagation*** are complete and results seem reasonable (feel free to check with your professor), it is at this point that you may continue to the next case.***
    ```



## Post-Lab Submission --- Interpretation of Results

```{admonition} Defend your conclusions with your data
:class: warning
Defend why your data agrees with or disagrees with the measured values for your masses. Use error propagation from your uncertainties and precision of your equipment to help your argument.
```

- Make sure to submit your finalized data table (Excel sheet).
    - Include a screenshot or photo of the linearized and quadratic plots from **Capstone** for just ***one trial*** for discussion purposes. 
- In a **paragraph**, summarize the results you have determined in each case. 
	- From where did you determine your experimental mass? Do your experimentally determined masses ± experimental uncertainty agree with the actual mass of the applied masses plus mass holder (i.e. range overalapping with actual value)?
    - How does the shape of the $F_\text{c}$ vs. $v^2$ plot compare to the $F_\text{c}$ vs. $v$ plot? 
        - What does this tell you about the mathematical relationship between centripetal force and velocity? 
        - For example, if the velocity is doubled, does the centripetal force also double, or does it change by a different factor? What is that change in centripetal force?
	- Why should there be the same mass on the fixed-counterweight mass holder as compared to the freely-sliding mass holder? What might you expect to see in your data if the fixed-counterweight and freely-sliding masses and radii were not comparable?
- In a **paragraph**, summarize your error analysis. Be qualitative not only quantitative.
	- What is the precision of your equipment?
    - What are possible random errors for today's experiment?
	- What are possible systematic errors for today’s experiments?
	- Discuss your uncertainties (see step !!!!!! TBD !!!!!!) and their effects
        - Sources of measured or esitmated uncertainties (values); how large are they?
        - How do they affect your final mass values; what has the largest affect?



<!---
        * Does graphs expected behavior question change to a discussion point in the procedure
        * From where did you determine your experimental mass? ..... does it agree quesiton
        * How does the shape of the Fc vs. v plot compare to the Fc vs. v^2 plot? What does this tell you about the mathematical relationship between centripetal force and velocity? For example, if the velocity is doubled, does the centripetal force also double, or does it change by a different factor? What is that change in centripetal force?
        * Wobbling question, include as discussion point at end of procedure
    * m mass becomes M_mass just to be super freaking clear
    * In Errors
        * Precision ? as first
        * What are possible rendom erroros
        * Discuss uncertainties, point back to step in procedure

--->


## The Whiteboard

```{figure} CentripetalForceFigures/CentripetalForce_2024_Fall_01_v2025-01.jpg
:name: centr
:width: 600px
:align: center

```



