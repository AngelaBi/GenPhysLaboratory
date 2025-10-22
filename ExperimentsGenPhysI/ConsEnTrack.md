(cons-energy-glider-track-lab-overall)=
# Conservation of Energy with Glider on Tilted Air Track

## Background

```{admonition} OVERALL GOALS
:class: note
In this lab, you will use an inclined, frictionless airtrack to:
- Investigate energy conservation by determining potential and kinetic energies of a glider.
```


**Energy cannot be created nor destroyed.** All that can really happen is a change in its form. We shall consider the conservation of mechanical energy, in particular, the sum of the kinetic energy and potential energy of a mass. The kinetic energy is due to the motion of the mass and the potential energy is due to the relative position of the mass in the earth's gravitational field. This total mechanical energy can only change if nonconservative forces are acting on any part of the system. We will examine the exchange of kinetic and potential energy and the conservation of mechanical energy under the presumption of no nonconservative forces acting. If the mechanical energy is not conserved we will attempt to determine potential sources of nonconservative work being done that would change the mechanical energy.

The **work** done by a force acting on a mass is the magnitude of the force acting in the direction of motion times the distance the mass moves. Work is only done when the mass moves. (In other words, you can push as hard as you like on a brick wall, but if the wall doesn't move, you didn't do any work!) Assume for the moment that we have a mass $m$ moving on a frictionless, horizontal surface. Assume a force acts on the mass from the position $x = 0$ to $x = x_1$ as illustrated in {numref}`M05Fig01`. At position $x = 0$ it is moving with a velocity $v_{0}$ and at $x = x_1$ the velocity is $v_1$.

```{figure} ConsEnTrackFigures/Figure01.jpg
:name: M05Fig01
:width: 500px
:align: center

Explanation of the variables needed to calculate the amount of work done on a mass
```

The work done by the force is $W_F = \vec{F} \cdot \vec{x_1}$. Using Newton's second law it can easily be shown that the work done by the force changes a quantity we call the *kinetic energy*, $K = \frac{1}{2} m v^2$. Using the example illustrated in {numref}`M05Fig01`,

```{math}
\vec{F} \cdot (\vec{x}_1 - \vec{0}) = \frac{1}{2} m v_1^2 - \frac{1}{2} m v_0^2
```

In this case, the force is acting in the direction of the motion and thereby increases the kinetic energy. If the force were acting in the direction opposite to the motion, then the kinetic energy would be decreased. If friction were present, it would act in the direction opposite to the direction of motion and thereby reduce the kinetic energy. In this simple analysis, we have made no assumption as to the nature of the force.

A force like friction is a non-conservative force. The work done by it not only depends upon the path the mass takes but is also not completely recoverable. However, the work done on a mass by a conservative force can be completely returned to the mass as mechanical energy. Thus work done by a conservative force can be represented by a potential energy function and depends only on the end points of the process. The gravitational force is a conservative force and is assumed constant in the vicinity of the surface of the earth. The potential energy function is merely the work done by gravity on the way up or the way down and is equal to the gravitational force (the weight $m g$) times the change in height, $h$. The gravitational potential energy, $U$, is given by

```{math}
U = m g h
```

The work done by this conservative force, like all conservative forces, only depends on the end-points of the path. The gravitational potential energy is a relative quantity, i.e., it is a change in energy because of a change in elevation. Thus we can choose a zero level arbitrarily.

If there are no non-conservative forces acting, then a mass moving only under the influence of gravity merely exchanges its kinetic and potential energy while the total energy remains constant. For a mass stationary at some height, $h$, above the ground, all of its energy is potential energy of value $mgh$ with respect to the ground. As the mass begins to fall under the influence of gravity, it loses $U$ and gains $K$. When it reaches the ground, the $U$ is zero with respect to the ground and the $K$ is a maximum, equal to the original $U$ at the top. If the mass were a roller coaster, the coaster could climb back up to its original height where all the energy would be $U$ at which point it would momentarily stop, i.e., no $K$. This assumes that neither friction nor any other nonconservative force is acting. In general, we have

```{math}
W_{N.C.} = \Delta K + \Delta U
```

where $W_{N.C.}$ is the work done by non-conservative forces. If there are no non-conservative forces acting, then

```{math}
:label: eq:total-energy
\Delta K + \Delta U = 0
```

In this experiment, we will use an air track to provide a nearly frictionless surface. The track will be tilted at a measurable angle. A glider will be released from rest at the top of the track and allowed to slide down and collide with a spring at the bottom. If the force of the spring on the glider is conservative, then the kinetic energy of the glider at the bottom is converted to potential energy in the compressed spring. This potential energy is given back to the glider in the form of kinetic energy as the spring expands. The glider bounces off and goes back up the track to its original height where the energy is again all $U$. If no energy is lost in the collision at the bottom, we say that the collision is completely elastic, implying that the forces involved in the collision are conservative. After the collision, the glider will rebound up the track. Getting back to its original height therefore implies no mechanical energy is lost during the entire path. If it does not, we have to look for an energy loss mechanism and some non-conservative forces acting.

The change in height from the top to the bottom is measured allowing the change in $U$ to be calculated. We will set the zero level for the potential energy at the bottom of track, at the position, $s_0$, in {numref}`M05Fig02`.

A measurement of the transit time from the top to the bottom will allow the calculation of the velocity at the bottom and therefore the $K$ at the bottom. Finally, measuring the maximum height achieved on the rebound will yield a second value of $U$.

The $K$ at the bottom of the track can be determined by measuring the average velocity from the release point at the top, $s_1$, to the collision point at the bottom, $s_0$, and then using {eq}`eq:total-energy`. From a measurement of the transit time from $s_1$ to $s_0$, the velocity of the glider at the moment of collision at the bottom, $v_b$, can be determined by using the definition of average velocity, $v_{\text{avg}}$, thus:

```{math}
\frac{\Delta s}{\Delta t}  = v_{\text{avg}} = \frac{1}{2} (v_{b}+v_1)
```

where the initial velocity, $v_1 = 0$, $\Delta s$ is the distance traveled down the track, and $\Delta t$ is the transit time of travel.

Rearranging terms we have the velocity at the bottom in terms of measurable quantities

```{math}
:label: eq:velocity-bottom
v_b = 2 v_{\text{avg}} = 2 \left(\frac{\Delta s}{\Delta t}\right)
```

Using the definition of $K$, the $K$ at the bottom is then

```{math}
:label: eq:kinetic-bottom
K_b = \frac{1}{2} m v_b^2
```

In order to calculate the potential energy, $U$ at any point, along the track we must determine the change in height between $s_1$ and $s_0$. The potential energy at any position along the track is measured with respect to the collision point at the bottom, $s_0$, which is arbitrarily assigned a value of zero potential energy. The $U$ is given by the weight of the glider, $mg$, times the change in vertical height.

{numref}`M05Fig02` is a simplified diagram of the inclined track. The distance $s$ is measured along the track by the scale attached to the side of the track. The change in elevation, $\Delta h$, of any other point $s$ along the track can now be determined from the distance $s$ and the incline angle of track, $\theta$. The incline of the track is produced by placing a spacer of known height under a leg at one end. With the height of the spacer and the distance between the legs, $D$, the angle can be calculated (See {numref}`M05Fig03`).

```{figure} ConsEnTrackFigures/Figure01_v2025-01.png
:name: M05Fig02
:width: 450px
:align: center

Schematic Drawing explaining the relationship between the track elevation $\Delta h$ and the distance $\Delta s$ for the Conservation of Energy experiment.
```

At $s_0$, $U_{b} = 0$, therefore $U_{s} = mg\, \Delta h = mg\, \Delta s \sin(\theta)$.
Referring to our schematic of the experimental setup in {numref}`M05Fig03`, we see $\sin(\theta) = \text{(height of the spacer)} / \text{(distance between legs)}$ or

```{math}
\sin(\theta) = \frac{H}{D}
```

<!--- With the very small angles of incline being used, we can safely assume that

```{math}
\tan(\theta) \sim \sin(\theta)
```
--->

therefore the potential energy, $U$, at some position, $s$, along the track is finally given by measurable quantities as

```{math}
:label: eq:potential-energy
U_s = mg \, \Delta s \frac{H}{D}
```

## Experimental Procedure

```{admonition} OVERVIEW
:class: note
- Experimentally determine potential and kinetic energies of a glider on a slightly tilted airtrack.
- Investigate how energy is converted, gained, or lost to different forms across two sequences in each trial:
  - Potential energy at the top to the kinetic energy at the bottom.
  - Potential energy at the top to the potential energy at some rebounded position.
- Conduct 4 cases based on 2 glider sizes and 2 initial heights.
  - Each case will have a total of 6 trials:
    - Groups of 2 students, each student will release the glider for 3 trials
    - Groups of 3 students, each student will release the glider for 2 trials
```

```{admonition} Notes & Assumptions, Sensors & Capstone
:class: tip
- The presumed frictionless inclined plane will be an air track.
- The mass will be a glider, which floats on the air track.
- Placing a spacer (essentially a big slotted mass, see {numref}`M05Fig05`) of height $H$ under the leg at one end of the track, which is a distance $D$ from the pivoting leg(s) at the opposite end, will incline the track.
- Time measured by PASCO photogate for velocity calculation in **Capstone** (stated precision of 0.0001 seconds).
- The relevant **Capstone** file will be on the desktop. Please ***DO NOT*** save when you are done, just exit without saving, thanks.
```


```{figure} ConsEnTrackFigures/Figure02_v2025-02.png
:name: M05Fig03
:width: 100%
:align: center

Experimental setup for the Conservation of Energy experiment.
```

```{figure} ConsEnTrackFigures/Figure05_spacers_v2025-02.png
:name: M05Fig05
:width: 100%
:align: center

Example of small and large spacers used to incline the air track. The cases today will be the BIG and Stacked heights. Remember to put the black plastic footer on top of the spacers as shown in the *stacked* case.
```



(consEnTrack-experimentPrep)=
### Preliminary Setup

1. **Do not put a glider on the track without air flowing. If the air supply is not yet on, please remind the instructor.**

2. Create a common data table including:
    - accepted value of $g$ of $9.803\,\text{m/s}^2$ for Fairfield, CT
    - the masses of each of the gliders in kg
    - the distance $D$ between the legs of the air track in meter (m)
    - the heights $H$ of the two spacers (big slotted masses) in m
    - $s_1$: starting point at the top
    - $s_0$: stopping point at the bottom
    - $\Delta s_1$: distance between the photogates that the glider travels down along the track

3. Measure and record the mass of both the big and small glider with the triple-beam-balance.
    ```{admonition} Calibration
    :class: tip
    *Reminder: ensure the balance is zeroed before measurements. You can use the adjustment knob on the left side under the silver weighing platform to ensure the pointers at the right end are aligned*.
    ```

4. **Level the airtrack.** Without the spacer present and the air track resting directly on the tabletop (with the black circle feet), place one of the gliders on the track (somewhere between the photogates, center) and note any preferential drift of the glider. Adjust the height of the single leg (screw clockwise in or counter-clockwise out) until the air track is level, as indicated by no preferential drift. Check both orientations of the glider on the track to check if the car is asymmetric and has a significant preferential drift on an otherwise level track. If this occurs, make sure to note that for your discussion purposes. <!---request the use of another glider and we can provide you a different one.--->

    ```{admonition} Drift
    :class: tip
    There will inevitably be some drift as these airtracks are not perfect, but as a general rule of thumb, if it takes more than $\sim 10$ seconds to drift just 5 cm, you should be pretty good.
    ```

5. Measure and record the distance $D$. This is the center-to-center distance between the legs. 1 m and 2 m long meter sticks are available for this measurement, with additional meter sticks at the front wall of the room.

6. Measure and record the heights, $H$, of each of the two spacers (big slotted masses) with the provided Vernier caliper. If you need a refresher on using Vernier calipers, see {ref}`reading-the-vernier-scale-help`. Since we'll be stacking the spacers for some of the cases today, include a stacked spacers value in your common data table for easier use of the height later.

7. Take a look at the gliders and determine a convenient point on the glider to use with the scale ($\sim2.5$ meter ruler) attached on the side of air track. It doesn't matter what point on the glider you choose, only that you be consistent and use the same point for all determinations of distance along the track $S$ for that glider. A convenient point is the ***lower front or rear corner*** of the glider since it is a clear point on the glider that will overlap or be quite close to the length scale on the track itself (see {numref}`M05Fig04`).

```{figure} ConsEnTrackFigures/Figure04_v2025-01.png
:name: M05Fig04
:width: 60%
:align: center

Suggested points on glider to read position on airtrack scale.
```

8. Determine and record the bottom photogate position $s_0$ at the bottom end of the track. Place the glider near the bottom of the track. Move it slowly as you approach the bottom photogate. Stop the glider at the exact location when the photogate's red light comes on. Move the glider back and forth to confirm your scale reading. See {ref}`demo-video-ConsEnTrack-s0s1` for example method.


<div style="text-align: center;">

(demo-video-ConsEnTrack-s0s1)=
#### Demo Video: Photogate Positions

</div>
    <!--- width="560"
    height="315"
    --->
<div style="text-align: center;">
  <iframe
    width=80%
    height="315"
    src="https://www.youtube.com/embed/vij2KvbPowU"
    title="YouTube video"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
  <figcaption>Determine photogate position on air track with glider.</figcaption>
</div>

9. Similarly, determine and record the starting photogate position $s_1$ at the top end of the track, then use those values to calculate and record $\Delta s_1=s_1-s_0$. Place the glider near the top of the track. Move it slowly as you approach the top photogate. Stop the glider at the exact location when the photogate's red light comes on. Move the glider back and forth to confirm your scale reading. Ensure your scale reading on the track was based on the same location of the glider as for your $s_0$ reading (i.e. {numref}`M05Fig04`).

    ```{admonition} Accurate Photogate Positions
    :class: tip
    Be careful not to bump the photogates, as that could change their positions and lead to inaccurate distances. Check during each case; if need be, expand your common data table with additional $s_0$ and $s_1$ positions.
    ```

10. Four cases will be performed as listed in {numref}`tab-four-glider-spacer-cases-ConsEnTrack`. For each of the four cases, perform the following steps listed in {ref}`detailsteps-ConsEnTrack` and record the data appropriately in your spreadsheet. ***Note: We are not doing the small spacer by itself today.***
    ```{table} Four experimental cases with spacers and gliders
    :name: tab-four-glider-spacer-cases-ConsEnTrack
    | Case | Spacer Size | Glider Size |
    |:----:|:-----------:|:-----------:|
    |  1   |   Stacked BIG + small [see {numref}`M05Fig05`]     |   small     |
    |  2   |   Stacked BIG + small [see {numref}`M05Fig05`]     |    BIG      |
    |  3   |    BIG      |   small     |
    |  4   |    BIG      |    BIG      |
    ```


```{admonition} Reminder, Run First Case Fully
:class: warning
Reminder, run your first case completely **before** moving on to additional cases. Don't just take all of your data without checking your methodology. If you have some error in your experimental method or in your calculations, you can correct it before completing all the other cases and finding out you have to completely redo the whole lab. The data tables for additional cases can be created by copying the first case **after** you are confident in and can explain your results from the first case.
```






<!--- <iframe width="560" height="315" src="https://www.youtube.com/embed/CINQAbvNFPw?si=srqk4862Gp_MHdzu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
--->


(detailsteps-ConsEnTrack)=
### Experimental Data Collection



11. For each of the four cases, create a Data table with enough **rows** for the number of trials you are doing, and **columns** for each of the variables you will be measuring or deriving:
    - Trial number
    - Lab member's initials
    - $t_1$: start time at the top
    - $t_0$: stop time at the bottom
    - $\Delta t$: time of travel between the photogates
    - $s_2$: The rebound position partway up the track
    - $U_{\text{top}}$: Initial potential energy at top
    - $v_{\text{b}}$: The speed at the bottom
    - $K_{\text{b}}$: Kinetic energy at the bottom
    - $\Delta s_2=s_2-s_0$: Final rebounded distance
    - $U_{\text{rebound}}$: Final potential energy at the rebound position

<!---    - **Capstone** Run Number (for returning to previous trial data)
--->

12. Ensure $s_1$ and $s_0$ haven't changed.

13. Raise the single leg side of the track by placing the case-relevant spacer under the black foot as seen in {numref}`M05Fig03` and {numref}`M05Fig05`.

14. Before you take the recorded data in the next steps, take some practice runs. Your subsequent data will be much improved by your training! Review the following demo videos as well.

  <div style="text-align: center;">

  (demo-video-ConsEnTrack-gliderRelease)=
  #### Demo Videos: Glider Release and Energy Conservation Across Single Trial

  </div>

  <div style="text-align: center;">
    <figure>
      <iframe
        width=80%
        height="315"
        src="https://www.youtube.com/embed/Pow7Sllbg6o"
        title="YouTube video"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        referrerpolicy="strict-origin-when-cross-origin"
        allowfullscreen>
      </iframe>
      <figcaption>Demonstration of glider release to minimize initial velocity.</figcaption>
    </figure>
  </div>

<div style="text-align: center;">
  <iframe
    width="80%"
    height="315"
    src="https://www.youtube.com/embed/CINQAbvNFPw"
    title="YouTube video"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
  <figcaption>Demo video: Energy Conservation.</figcaption>
</div>



15. Press record in **Capstone** to start the timer.

    ```{admonition} Capstone Timer
    :class: tip
    - The timer shown is coded in Capstone; once you press record, it will take a few seconds for the timer to start, wait until you confirm the timer is ready before releasing the glider.
    - **Capstone** will display the time whenever a photogate beam is broken; the time shown is the time at the higher (start) photogate $t_1$ as well as the time at the lower (end) photogate $t_0$. To determine the total transit time $\Delta t$, take the difference of the start and end times.
    - Additional notes on the timer are in the Capstone file itself, ***please read***.
    ```  


16. For each of the **6 trials per case**, release the glider from rest at the $s_1$ position. Measure and record the start time $t_1$ and end time $t_0$ to determine transit time $\Delta t$ from the release at the top to bottom of the airtrack. Note the rebound position $s_2$ where the glider goes to rest after it rebounds up the track. Calculate the value of potential and kinetic energies, and discuss the conservation of energy throughout the experiment. To do so:

    a. Position the glider so it is blocking the top photogate and the red light is on. Use the red glider-release mechanism to hold the glider in place. ***Shift the mechanism up or down the track as necessary to move and hold the glider just before the photogate beam such that the red light on the photogate just goes out.***

    b. Check the Capstone timer is ready, then release the glider by *quickly* flipping the glider release bar to minimize any additional push or pull on the glider to **ensure its initial velocity is zero**. (reminder, see {ref}`demo-video-ConsEnTrack-gliderRelease`).

    c. Allowing the glider to rebound off the bumper, record the rebound position $s_2$. As the glider slows to a stop, capture the glider by gently pressing your finger near the lower edge of the glider just as it comes to a stop and then read $s_2$ off the scale. Use the same point on the glider to read $s_2$ that you used to read $s_1$ and $s_0$.

    c. Record the relevant $t_1$ and $t_0$ values in your spreadsheet. There is not a time for the rebound position. Calculate $\Delta t$.

    d. Calculate the relevant energies at the top starting point, the bottom of the track, and the rebound position (i.e. $U_{\text{top}}$, $K_{\text{b}}$ using the calculated veleocity at the bottom photogate $v_{\text{b}}$, $\Delta s_2=s_2-s_0$, $U_{\text{rebound}}$).

    e. Repeat for each trial of this case. Reminder, you do not need to turn off the timer, you just need the relevant times as you will be using the time difference.

    ```{admonition} Reminder: Take turns
    :class: note
    - Groups of 2 students, each student will release the glider for 3 trials
    - Groups of 3 students, each student will release the glider for 2 trials
    ```





**Data Table:**



- Create a summary table of the analysis with a row for each case including the following data:

  - The average and standard deviation of the time, $\Delta t$, for the five trials
  - The average and standard deviation of the speed at the bottom, $v_{\text{b}}$
  - The average and standard deviation of the kinetic energy at the bottom, $K_{\text{b}}$
  - The average and standard deviation of the final potential energy at the rebound position, $U_{\text{rebound}}$
  - Percent change from initial potential energy to kinetic energy at the bottom
  - Percent change from initial potential energy to final potential energy

Calculate the following:

- For each case, calculate the initial potential energy at $s_1$. Average the transit times, $\Delta t$, and calculate the velocity $v_b$ and the $K_b$.

- For each case, average the rebound position, $s_2$. Using this averaged value, calculate the final $U_2$.

- Calculate the percent change in mechanical energy from the top to the bottom.

- Calculate the percent change in mechanical energy from the initial release point $s_1$ to the final rebound point $s_2$.




## Post-Lab Submission --- Interpretation of Results

- Make sure to submit your finalized data table (Excel sheet). 
- In a **paragraph**, summarize the results you have determined in each case. Consider
	- Arguing your responses with your data ± standard deviation:
	    - Is kinetic plus potential energy conserved going from the top to the bottom?
		- Is kinetic plus potential energy conserved between the top and the rebound position?
	- Why is there a difference in energy conservation between the top/bottom and top/bottom/rebound?
- In a **paragraph**, summarize your error analysis. Be qualitative not only quantitative.
	- What is the precision of your equipment?
	- What are the effects of measured uncertainties on your determined energies?
	- What are possible systematic errors for today’s experiments?
	- How could one gain energy between top and bottom?

## The Whiteboard

```{figure} ConsEnTrackFigures/ConsOfEnergyTrack_2024_Fall_01.jpg
:name: consE
:width: 600px
:align: center

```