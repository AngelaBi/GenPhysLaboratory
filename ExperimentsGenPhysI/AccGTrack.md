# Acceleration due to Gravity, *g*, with Glider on Tilted Air Track

```{admonition} OVERALL GOALS
:class: note
Use an frictionless airtrack to:
- Measure acceleration due to gravity.
```

## Background

By measuring the acceleration of a mass moving under the influence of just the gravitational attraction of the earth, namely its weight, we can determine the acceleration due to gravity, usually denoted by $g$.  The mass will be allowed to accelerate down a presumed frictionless, inclined plane.  Measurement of the acceleration along the plane is directly related to the acceleration due to gravity by a simple trigonometric relationship.  The use of the plane permits the convenient measurement of a small, measurable fraction of the acceleration due to gravity.  This of course is in lieu of the much more difficult measurement of a vertically falling mass.


Near the surface of the earth, the attractive force of the earth on a mass can be considered a constant over a reasonable range of elevation. This force is commonly called the weight of the object and, from Newton's Second Law, the weight is the mass $m$ times the acceleration due to gravity $g$. Using {numref}`M02Fig01` and the derivation following, we can see that the value of $g$ can be easily determined by a few simple measurements.

```{figure} AccGTrackFigures/Figure01_v2025-02.png
:name: m02fig01
:width: 500px
:align: center

Force Diagram and variables used in Vector Table Experiment.
```

The displacement along the track is $S$, the component of the weight along the track is $F_s$, and the component of acceleration $a_s$ along the track is

$$
a_s = \frac{F_s}{m} = \frac{m g \sin(\theta)}{m} =  g \sin(\theta).
$$

If the mass is released from *rest* near the top of the inclined air track and allowed to accelerate down the air track with a magnitude $a_s$, then by measuring the transit time down the track over a measurable distance $S$, we can determine the value of $g$.

Since the acceleration $a_s$ is constant as gravity itself is constant, the displacement $S$ as a function of time $t$ is:

$$
  S = \frac{1}{2} a_s t^2 = \frac{1}{2} g t^{2} \sin(\theta).
$$

Solving for $g$, we obtain

```{math}
:label: eq-M02-g-basic
  g = \frac{2 S}{t^2 \sin(\theta)}.
```

where, based on our schematic of the experimental setup in {numref}`M02Fig02`, we see $\sin(\theta) = \frac{H}{D}$.
Making this substitution for the $\sin(\theta)$, we have the value of $g$ in terms of easily measurable quantities, namely

```{math}
:label: eq-M02-g-value
  g = \frac{2 S D}{H t^2}
```

where $H$ is the vertical rise in the horizontal distance $D$. $D$ is the distance between the legs of the air track, and $t$ is the transit time of the mass, starting from zero velocity and accelerating down the plane a distance $S$ along the plane.



















## Experimental Procedure

```{admonition} OVERVIEW
:class: note
- Experimentally determine the acceleration due to gravity $g$ by using a slightly tilted airtrack.
- Investigate how $g$ is affected by the mass of an object and angle of the track (i.e. initial height of that object).
- Conduct 4 cases based on 2 glider sizes and 2 initial heights.
- Compare the experimental results to the expected value of $g$ at Fairfield, CT, of $9.803\,\text{m/s}^2$.
```

```{admonition} Notes & Assumptions
:class: note
- The presumed frictionless inclined plane will be an air track.
- The mass will be a glider, which floats on the air track.
- Placing a spacer of height $H$ under the leg at one end of the track, which is a distance $D$ from the leg(s) at the opposite end, will incline the track.
- Time measured by PASCO photogates (stated precision of 0.0001 seconds) PASCO's data logging and visualization software, **Capstone**, installed on the lab computers. The relevant Capstone file will be on the desktop. Please ***DO NOT*** save when you are done, just exit without saving.
```



```{figure} AccGTrackFigures/Figure02_v2025-02.png
:name: M02Fig02
:width: 100%
:align: center

Experimental Setup.
```



1. **Do not put a glider on the track without air flowing.**
2. Create a common data table including:
    - the masses of each of the gliders in kg
    - the distance $D$ between the legs of the air track in meter (m)
    - the heights $H$ of the two spacers in m

3. Measure and record the mass of both the big and small glider with the triple-beam-balance.
    ```{admonition} Calibration
    :class: note
    *Reminder: ensure the balance is zeroed before measurements. You can use the adjustment knob on the left side under the silver weighing platform to ensure the pointers at the right end are aligned*.
    ```

4. **Level the airtrack.** Without the spacer present and the air track resting directly on the tabletop (with the black circle feet), place one of the gliders on the track (at either end and center) and note any preferential drift of the glider. Adjust the height of the single leg (screw clockwise in or counter-clockwise out) until the air track is level, as indicated by no preferential drift. Check both orientations of the glider on the track to check if the car is asymmetric and has a significant preferential drift on an otherwise level track. If this occurs, request the use of another glider and we can provide you a different one.

    ```{admonition} Note on drift
    :class: note
    There will inevitably be some drift as these airtracks are not perfect, but if it takes more than 10 seconds to drift just 5 cm, you should be good.
    ```

5. Measure and record the distance $D$. This is the center-to-center distance between the legs. 1 m and 2 m long meter sticks are available for this measurement, with additional meter sticks at the front wall of the room.

6. Measure and record the heights, $H$, of each of the two spacers with the provided Vernier caliper. If you need a refresher on using Vernier calipers, see {ref}`reading-the-vernier-scale-help`.

7. Four cases will be performed:

    ```{table} Four experimental cases with spacers and gliders
    :name: tab-four-glider-spacer-cases
    | Case | Spacer Size | Glider Size |
    |:----:|:-----------:|:-----------:|
    |  1   |    BIG      |   small     |
    |  2   |    BIG      |    BIG      |
    |  3   |   small     |   small     |
    |  4   |   small     |    BIG      |
    ```

8. Determine a convenient point on the glider to use with the scale attached on the side of track. It doesn't matter what point you choose, only that you use the same point for all determinations of $\Delta s$ for that glider. A convenient point is the lower front or rear corner of the glider since it will be very close or overlapping with the length scale on the track itself.
9. For each of the four cases, perform the steps listed in  {ref}`detailsteps` and record the data appropriately in your spreadsheet

(detailsteps)=
### Steps for each of the four cases with a tilted track

a. For each of the four cases with a tilted track create enough **rows** for the number of trials you are doing, and **columns** for each of the variables you will be measuring or deriving:
  - starting point at the top $s_1$
  - stopping point at the bottom $s_0$
  - distance between the photogates that the glider travels $S$
  - start time at the top $t_1$
  - time at the bottom $t_0$
  - time between the photogates $\Delta t$
  - calculated value of $g$ using {eq}`eq-M02-g-value` for each of the five trials
  - average value of $g$ from the five trials of each case
  - standard deviation of $g$ from the five trials of each case
  - difference between the average value of $g$ and the accepted value of $9.803\,\text{m/s}^2$ for Fairfield, CT for each case
  - similarly, the average, standard deviation, and difference for $g$ from all 20 trials across all 4 cases

b. Raise the single leg side of the track by placing a spacer under the knob.

c. Place the glider near the bottom of the track. Move it slowly as you approach the bottom photogate. Stop the glider at the exact location when the photogate's red light comes on. Record position on the scale, $s_0$.

d. Next, place the glider near the top of the track. Move it slowly as you approach the top photogate. Stop the glider at the exact location when the photogate's red light comes on. Record position on the scale, $s_1$.

e. Before you take the recorded data in the next step, take some practice runs. Your subsequent data will be much improved by your training! Press record in **Capstone** to start the timer. 

```{admonition} NOTE
:class: note
**Capstone** will display the time whenever a photogate beam is broken; the time at the higher (start) photogate $t_1$ as well as the time at the lower (end) photogate $t_0$. To determine the total transit time $\Delta t$, take the difference of the start and end times.
```   

f. Position the glider so it is blocking the top photogate and the red light is on. Place one finger on the track in front of the glider and gently move the glider up the track (to the right) until the red light on the photogate just goes out.

g. Release the glider by quickly pulling your finger away from the track and glider (MINIMIZE ANY FINGER CONTACT WITH THE GLIDER to minimize any additional push or pull on the glider to **ensure its initial velocity is zero**).

h. For each of the **5 trials per case**, release the glider from rest at the $s_1$ position. Measure and record the start time $t_1$ and end time $t_0$ to determine transit time $\Delta t$ from release at the top to bottom of the airtrack. Calculate the value of $g$ for this trial.


10.  For each the four cases:
- Calculate the average of the measured $g$
- Calculate the standard deviation of the measured $g$
- Calculate the differences between your average $g$ and the accepted value of $g$

1.   Also, using data from all trials from all the cases:
- Calculate the average of the measured $g$.
- Calculate the standard deviation of the measured $g$.
- Calculate the differences between your average $g$ and the accepted value of $g$
  


## Post-Lab Submission --- Interpretation of Results

- Make sure to submit your finalized data table (Excel sheet)
- In a **paragraph**, summarize the results you have determined in each case, ie $g\pm\sigma g$... and answer the following questions (longer does not mean better):
	- If you release the glider with an initial velocity up or down the slope, what would you expect to happen to your derived values of $g$?
	- Suppose there is a frictional force slowing the glider as it moves along the track. How would this affect the determined value of $g$? Would your result support or not support the hypothesis of that there is significant friction along the track?
	- Assume the track is not level at the beginning of the experiment. Further, assume that what you thought to be a level track was in fact slightly tipped in the same direction as your deliberate tipping via the spacers during the experiment. How would this affect the determined value of $g$? Would your result support or not support the hypothesis of the track not being level?
- In a **paragraph**, summarize your error analysis. Be qualitative not only quantitative.
	-  What are sources of uncertainty (initial v, friction, etc.)?
	- What was the precision of the instrumentation (e.g. caliper, time, distance, etc.)?
	- Compare your results ($g$ from each of the four cases and one from all 20 trials) to the accepted value. How do the standard deviations compare to the difference between your values of $g$ and the accepted value of $g$? 
      - I.e. while treating the standard deviations of your measurements as your measurement uncertainties, do your values of $g$ for each case, as well as the overall average $g$, plus or minus the standard deviations overlap (and agree) with the accepted value of $g$? 
      - What might cause your results to disagree the most?



## The Whiteboard

```{figure} AccGTrackFigures/AccelGTrack_2024_Summer_01.jpg
:name: AccelGTrack
:width: 600px
:align: center


```
