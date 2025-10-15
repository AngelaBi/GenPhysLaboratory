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

1. The experiment should already be setup for you as shown in {numref}`M04Fig02` with masses attached to both the freely-sliding and fixed-counterweight mass holders as well as already being hooked up to the computer interface and power supply. Reminder, the relevant Capstone file will be on the desktop (e.g. {numref}`M04Fig07`). Prepared are relevant notes, a stopwatch, and two graphs:
   - $F$ versus $v^2$
   - $F$ versus $v$

    ```{figure} CentripetalForceFigures/Figure07_v2025-01.png
    :name: M04Fig07
    :width: 80%
    :align: center

    Example of today's **Capstone** layout. Review notes for helpful info.
    ```

2. Create a overall common data table including (but not limited to):
    - the mass of the freely-sliding mass holder (kg)
    - uncertainty of the mass of the freely-sliding mass holder (kg)

3. Remove the freely-sliding mass holder and measure its mass with a triple-beam balance. Record this in your data sheet. Re-attach the assembly to the rotating arm with one plastic washer below the arm and one above. Then the silver nut, tightened down enough to prevent tipping, but the assembly must slide freely. Then the cable loop. Then use the black nut to attach the applied disk masses above the loop. See order in {numref}`M04Fig04`.

    ```{admonition} Calibration
    :class: note
    *Reminder: ensure the balance is zeroed before measurements. You can use the adjustment knob on the left side under the silver weighing platform to ensure the pointers at the right end are aligned*.
    ```

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
    |  1   |   5     |   LONG ($\sim95-105$)      |
    |  2   |   15     |    LONG ($\sim95-105$)      |
    |  3   |    5      |   short ($\sim60-70$)      |
    |  4   |    15      |    short ($\sim60-70$)      |
    ```


    ```{admonition} Reminder, Run First Case Fully
    :class: warning
    Reminder, run your first case completely **before** moving on to additional cases. Don't just take all of your data without checking your methodology. If you have some error in your experimental method or in your calculations, you can correct it before completing all the other cases and finding out you have to completely redo the whole lab. The data tables for additional cases can be created by copying the first case **after** you are confident in and can explain your results from the first case.
    ```

(detailsteps-centripetal-force)=
### Experimental Data Collection


5. For each case, construct:
    - A common data table for the current case including (but not limited to):
        - $M_\text{applied}$: mass of applied disk masses (kg)
        - $M_\text{object,actual}$: actual mass of the rotating, freely-sliding object 
        - $R$: the radius (m)
        - $\delta R$: your estimate of the uncertainty in the radius (m) (i.e. $\text{radius} \pm \delta R$)
    - A data table with a row for each trial and average values as well as columns (but not limited to):
        - $m$: fit parameter $m$ from the $F_\text{c}$ vs. $v^2$ (linear fit)
        - $M_\text{object,experimental,linear}$: the mass determined from $F_\text{c}$ vs. $v^2$
        - the difference between $M_\text{object,experimental,linear}$ and $M_\text{object,actual}$
        - $A$: fit parameter $A$ from the $F_\text{c}$ vs. $v$ (quadratic fit)
        - $M_\text{object,experimental,quadratic}$: the mass determined from $F_\text{c}$ vs. $v$
        - the difference between $M_\text{object,experimental,quadratic}$ and $M_\text{object,actual}$
        - $\delta M_\text{object,experimental}$ the uncertainty in the mass from the centripetal force due to your estimated radius uncertainty (*Point to consider*: how much does the derived mass change if you change your value for radius in **Capstone calculator** by the amount of your estimated radius uncertainty?)

6. Attach the necessary applied masses for the current case as listed in {numref}`tab-four-centripetal-force-cases` following steps depicted in {numref}`M04Fig04`. Record $M_\text{applied}$. Calculate the total mass of the rotating object $M_\text{object,actual}$ --- the sum total of the freely-sliding mass holder and the applied mass.


7. Set radius $R$ to the value listed in {numref}`tab-four-centripetal-force-cases` for the current case; it just needs to be within the range listed. Do this by raising or lowering the force sensor (see bar & clamp holding force sensor in {numref}`M04Fig02`). It is important that the force sensor be ***exactly above the center of the apparatus.*** To check this, pull on the freely-sliding mass to put tension in the cable. Then observe the cable from the front and side of the system to verify it is parallel to the L-stand's vertical rod and perpendicular to the rotating arm. Adjust the horizontal rod holding the force sensor until that is that is achieved. Ensure the force sensor is still pointed downwards towards the pulley at the axis of rotation. *Any time you change the position of the Force Sensor, you will have to **repeat** this step.*


8. Measure and record radius $R$. Pull the mass to tighten the cable to determine the actual radius to the nearest millimeter. You can do this using the scale attached to the side of the apparatus. 

    ```{admonition} Discussion Point: Why tighten?
    :class: note
    Why do we measure the radius when the cable is taut?
    ```

9. Estimate $\delta R$, your estimated uncertainty in the radius. Remember, this is a bit subjective relating to how confident you are that the freely-sliding object is at your stated radius, not soley the precision of your tools. It essentially becomes how far you could move the object a bit towards or away from the axis of rotation, and still be confident in saying your radius measurement is accurate.

10. Set the radius in **Capstone's Calculator** which is set up to determine instantaneous tangential velocity. Select **Calculator** in the menu on the left-hand side (example shown in {numref}`M04Fig03`). In line 1, replace the `0.###` value with the value that you actually measured in the previous step. Click the **Calculator** again to close it. *Any time you change the radius, you will need to **update** the value in **Calculator.***

    ```{figure} CentripetalForceFigures/Figure03_v2025-01.png
    :name: M04Fig03
    :width: 80%
    :align: center

    Calculator setup in **Capstone** to determine the speed of the rotating objects. Make sure to adjust the value for the radius in this window to the actual value used in your experimental setup.
    ```
11. To avoid wobbling, tighten an identical fixed-counterwieght mass to the opposite side of the rotating arm such that it is as far from the axis of rotation as your previously measured $R$. Tighten so it doesn't move --- **DON'T OVERTIGHTEN, THIS CAN DAMAGE THE RUBBER WASHERS.**

    ```{admonition} Discussion Point: Counterweight
    :class: note
    Why should there be the same mass on the fixed-counterweight mass holder as compared to the freely-sliding mass holder? What might you expect to see in your data if the fixed-counterweight and freely-sliding masses and radii were not comparable?
    ```

12. ***ZERO*** the force sensor: 
     - Press *Record.* Wiggle the rotating arm such that the white pin underneath the counterweight passes back and forth through the photogate. It is likely the force sensor is not calibrated yet, and you might see values for the force on the left-hand linear graph not plot on the $0\,\text{line}$. 
     - **ZERO** the force sensor with the physical *ZERO* button on the force sensor while ensuring the connecting cable is slack. 
     - You can check the force sensor is now zeroed out by again wiggling the rotating arm to cross the photogate and find that the data points are now plotting on the  $0\,\text{line}$. If this is not the case, try again until it does. 
     - You can stop recording and ignore that data.
     - Double check the force sensor calibration at least for each case.

12. Start the data acquisition on **Capstone** by pressing the **Record** button.
   You should notice that the program might not show values; this is normal as it will only record a value once the photogate has been crossed by the white pin underneath the fixed-counterweight.

    ```{admonition} ⚠️⚠️⚠️ CAUTION: ROTATING ARM WILL BE FAST ⚠️⚠️⚠️
    :class: warning
    The next step will cause the apparatus to begin rotation. Be sure it can do so without hitting anything or anybody as it will reach damaging speeds.
    ```

13. Over the course of about 60 seconds (see stopwatch in top right of {numref}`M04Fig07`), slowly increase the voltage on the power supply from $0\,\text{V}$ to $10\,\text{V}$. The metal arm will begin to rotate, and you will notice the graphs display the data as it is collected. You may notice kinks in the data (e.g. {numref}`M04Fig08`); that is alright as some power supplies may have small jumps in the voltage as it switches to different internal circuits. Just focus on slowly and consistenty increasing the voltage.

    ```{admonition} Voltage Limits
    :class: warning
    Do not exceed $10\,\text{V}$, we don't want to burn out the motor --- only rated for $12\,\text{V}$
    ```

    ```{figure} CentripetalForceFigures/Figure08_v2025-01.png
    :name: M04Fig08
    :width: 60%
    :align: center

    Example of kink in the data due to possible irregularities or voltage jumps in the power supplies.
    ```

14. **Before** returning the power supply to zero, press the **STOP** button in Capstone to stop data acquisition. When you are finished taking data, you can scale both axes of either graph using the tool shown in {numref}`M04Fig06`.

    ```{figure} CentripetalForceFigures/Figure06_v2025-01.png
    :name: M04Fig06
    :width: 60%
    :align: center

    Autoscale axes tool.
    ```

15. Once you have finished your trial, **fit a straight line** to your $F$ vs. $v^2$ graph and set its y-intecept $b$ to zero.  *Note: you will need to do this for each trial as **Capstone** resets to the default settings for each trial.* For visual instructions, see {numref}`M04Fig05`. Select the fit box $\rightarrow$ select Curve Fit Editor $\rightarrow$ lock the y-intercept $b = 0$ $\rightarrow$ update the fit. Notice the change in slope $m$ when you lock $b$.

    ```{figure} CentripetalForceFigures/Figure05_v2025-01.png
    :name: M04Fig05
    :width: 70%
    :align: center

    Process for applying fits to plotted data, updating the y-intercept and other curve-fit terms, and updating sig. figs.
    ```

    ```{admonition} Discussion Point: Y-Intercept
    :class: note
    Why should the y-intercept be zero? If your fit appears to have changed a lot, why might your data not agree? Is there a step you may have missed?
    ```

16. Increase the number of significant figures in for the fit. *Note: you will need to do this for each trial.* For visual instructions, see {numref}`M04Fig05`. Select the fit box $\rightarrow$ select Curve Fit Properties (gear) $\rightarrow$ Numerical Format $\rightarrow$ Coefficients $\rightarrow$ update sig. figs. to at least **4**. 

17. Record $m$, the linear fit's slope in your data table (based on $y = mx+b$).

18. Calculate your experimental mass of the rotating object based on your linear fit $M_\text{object,experimental,linear}$ using {eq}`eq-centripetal-force`.

    ```{admonition} Discussion Point: Mass of Rotating Object
    :class: note
    How do you determine the value for the mass of the rotating object from your data?
    ```

19. Calculate the difference between your experimental $M_\text{object,experimental,linear}$ and the actual mass $M_\text{object,actual}$.


20. **Fit a quadratic curve** to your $F$ vs. $v$ graph and set its coefficients $B$ and $C$ to zero y-intecept $b$ to zero in a similar fashion to your linear plot. *Note: you will need to do this for each trial.* For visual instructions, see {numref}`M04Fig05`. Notice the change in coefficient $A$ when you lock $B$ and $C$.

    ```{admonition} Discussion Point: Quadratic fit
    :class: note
    Why should the $B$ and $C$ coefficients be zero? If your fit appears to have changed a lot, why might your data not agree? Is there a step you may have missed?
    ```

21. Increase the number of significant figures for the quadratic fit to at least **4** in a similar fashion to the linear plot. *Note: you will need to do this for each trial.* For visual instructions, see {numref}`M04Fig05`.

22. Record $A$, the first term's coefficient in your data table (based on $y = Ax^2+bx+c$).

23. Calculate your experimental mass of the rotating object based on your quadratic fit $M_\text{object,experimental,quadratic}$, again using {eq}`eq-centripetal-force`.

24. Calculate the difference between your experimental $M_\text{object,experimental,quadratic}$ and the actual mass $M_\text{object,actual}$.


25. Repeat the previous steps for the other the trials *for this current case.*

    ```{admonition} Note on data in Capstone
    :class: note
    There is a Delete Last Run button in Capstone. You *NEVER* need to press that as Capstone will just hold on to that data as a past trial that you could go back and look at as needed. When you press Record, Capstone will just create a new *Run* of data to keep track of.
    ```


(summary-step-centripetal-force)=
### Combined Results and Error Propagation For Current Case

26. Calculate the averages of all your previously determined values in your data table for the current case.

27. Error propagation to find $\delta M_\text{object,experimental}$: 
    - Using just one of your trials from this case, determine your estimated uncertainty in the experimental mass $\delta M_\text{object,experimental}$ of the rotating object.
    - Assumption: Error in mass is primarily due to radius.
    - To do so, essentially create an additional trial for this case. Return to the calculator ({numref}`M04Fig03`) and update the radius to be either larger or smaller based on your values $R \pm \delta R$. Notice how your graphs and fits change. Use those updated values in this error propagation trial to effectively determine the range of experimental masses by finding a larger or smaller value for your object mass $M_\text{object,experimental,errorTrialLarger}$.
    - *Reminder: you updated the radius in Capstone; how did you use {eq}`eq-centripetal-force` to determine mass?*
    - Determine the uncertainty in your experimental mass $\delta M_\text{object,experimental}$ as the magnitude/absolute value of the difference between this larger or smaller value for mass and your average experimental mass from the original trials 
        ```{math}
        :label: eq-centripetal-force_errorProp
        \delta M_\text{object,experimental} = | M_\text{object,experimental,errorTrialLarger} - M_\text{object,experimental,linear} |
        ```
    - Treat this difference as your $\delta M_\text{object,experimental}$.

    ```{admonition} Discussion Point: Experimental Mass
    :class: note
    How much does the experimental mass change if you change your value for radius in **Capstone calculator** by the amount of your estimated radius uncertainty?
    ```



13. Repeat the previous steps in {ref}`detailsteps-centripetal-force` and {ref}`summary-step-centripetal-force` for the next case with the relevant applied mass and radius as listed in {numref}`tab-four-centripetal-force-cases`. Please call for help as needed for setting up next cases.

    ```{admonition} Continue to additional case?
    :class: warning
    ***If you are satisfied that your calculations and ***error propagation*** are complete and results seem reasonable (feel free to check with your professor), it is at this point that you may continue to the next case.***
    ```


29. ***BEFORE CLOSING CAPSTONE: TAKE A Screenshot or photo of at least 1 trial representative of your data for discussion later.***

    ```{admonition} Discussion Point: Graph Shape
    :class: note
    Do the graphs display the expected behavior?
    ```

    ```{admonition} Photo of Experimental Data
    :class: warning
    Take a screenshot/photo to include in your Excel datasheet / spreadsheet submission.
    ```


## Post-Lab Submission --- Interpretation of Results

```{admonition} Defend your conclusions with your data
:class: warning
Defend why your data agrees with or disagrees with the measured values for your masses. Use error propagation from your uncertainties and precision of your equipment to help your argument.
```

- Make sure to submit your finalized data table (Excel sheet).
    - Include a screenshot or photo of the linearized and quadratic plots from **Capstone** for just ***one trial*** for discussion purposes. 
- In a **paragraph**, summarize your error analysis. Be qualitative not only quantitative.
	- What is the precision of your equipment?
    - What are possible random errors for today's experiment?
	- What are possible systematic errors for today’s experiments?
	- Discuss your uncertainties (see {numref}`summary-step-centripetal-force`) and their effects
        - Sources of measured or esitmated uncertainties (values); how large are they?
        - How do they affect your final mass values; what has the largest affect?
- In a **paragraph**, summarize the results you have determined in each case. 
	- From where did you determine your experimental mass? Do your experimentally determined masses with uncertainties ($i.e. M_\text{object,experimental} \pm \delta M_\text{object,experimental}$) agree with the actual mass of the applied masses plus mass holder (i.e. range overalapping with actual value)?
    - How does the shape of the $F_\text{c}$ vs. $v^2$ plot compare to the $F_\text{c}$ vs. $v$ plot? 
        - What does this tell you about the mathematical relationship between centripetal force and velocity? 
        - For example, if the velocity is doubled, does the centripetal force also double, or does it change by a different factor? What is that change in centripetal force?
	- Why should there be the same mass on the fixed-counterweight mass holder as compared to the freely-sliding mass holder? What might you expect to see in your data if the fixed-counterweight and freely-sliding masses and radii were not comparable?



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



