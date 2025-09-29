(simple-projectile-motion-overall)=
# Simple Projectile Motion

## Background

```{admonition} OVERALL GOALS
:class: note
In this lab, you will:
- Understand and apply kinematic equations to one- and two-dimensional projectile motion.
```

**Projectile motion** is the motion of an object thrown or projected into the air, subject only to acceleration as a result of gravity. The applications of projectile motion in physics and engineering are numerous. Some examples include meteors as they enter Earth's atmosphere, water in a water fountain, and the motion of any ball in sports. Such objects are called *projectiles*, and their path is called a **trajectory**.

We can represent a projectile's motion through kinematics which utilize its position, time, velocity, and acceleration. The kinematic equations we will use during this lab assume both ***constant acceleration*** effects of air resistance are ***negligible*** (generalized in the next four equations with $x$ representing position along any given dimension): 

```{math}
:label: eq-M03-Kinematic-01
v = v_{0} + at
```

```{math}
:label: eq-M03-Kinematic-02
x = x_{0} + v_{0}t + \frac{1}{2}at^{2}
```

```{math}
:label: eq-M03-Kinematic-03
v^{2} = v_{0}^{2} + 2a(x - x_{0})
```

```{math}
:label: eq-M03-Kinematic-04
x = x_{0} + \frac{1}{2}(v_{0} + v)t
```



Today, we will analyze both one- and two-dimensional trajectories, where $x$ will represent the horizontal direction, and $y$ the vertical. Gravity (which pulls objects down towards the center of the Earth) will be assumed to be the only source of acceleration acting on our projectiles; as such, the acceleration of a projectile is $a_{y} = -g$ and $a_{x} = 0$. Since horizontal acceleration terms are zero, we can represent horizontal motion by:

```{math}
:label: eq-M03-horizontal-Kinematic
v_{0x} = v_{x} = \text{constant velocity},~~~ x = x_{0} + v_{x}t
```

Then, depending on the information we have available to us, we can represent vertical motion by:

```{math}
:label: eq-M03-Kinematic-vertical-01
v_{y} = v_{0y} - gt
```

```{math}
:label: eq-M03-Kinematic-vertical-02
y = y_{0} + v_{0y}t - \frac{1}{2}gt^{2}
```

```{math}
:label: eq-M03-Kinematic-vertical-03
v_{y}^{2} = v_{0y}^{2} - 2g(y - y_{0})
```

```{math}
:label: eq-M03-Kinematic-vertical-04
y = y_{0} + \frac{1}{2}(v_{0y} + v_{y})t
```







### Free Fall / Downward Trajectory (First experiment)

In the previous lab, we determined the acceleration due to gravity via the tilted air track to take advantage of a longer time frame to measure a small fraction of the acceleration due to gravity. This week, we will determine the acceleration due to gravity more directly by considering a one-dimensional trajectory (i.e. free fall).

The experimental setup will involve a free-fall timer where a metal ball is dropped from a release mechanism as shown in {numref}`M03-simpleProjectileLauncher-Exp1`. When the metal ball is in then mechanism, it provides a closed circuit; once the ball is released and the circuit opens, the computer automatically starts timing $t_{\text{initial}}$. The ball then hits the receptor pad on the floor, closing the circuit and stopping the timer at $t_{\text{final}}$. Using the recorded time difference $t = t_{\text{final}} - t_{\text{initial}}$, and the initial height $y_{0}$ as measured from the bottom of the ball to the top of the receptor plate (which is at the final height $y = 0\,\text{m}$), we can rearrange {eq}`eq-M03-Kinematic-vertical-02` to determine acceleration due to gravity.

```{math}
:label: eq-M03-Kinematic-freefall-g
0 = y_{0} + 0 - \frac{1}{2}gt^{2}~~~=>~~~\frac{2y_{0}}{t^2} = g
```

```{figure} SimpleProjectileFigures/M3_Exp1.jpg
:name: M03-simpleProjectileLauncher-Exp1
:width: 500px
:align: center

Example of the free fall apparatus used in Exp. 1. Note the release screw will be what you tighten or loosen to hold or release the ball from the release mechanism.
```

### Horizontal Trajectory (Second experiment)

```{figure} SimpleProjectileFigures/M3_ExpOptions_quarter_size.jpg
:name: M03-simpleProjectileLauncher
:width: 90%
:align: center

Left) Position of launcher for lower height in Experiment 2. Right) Position of launcher for higher height in Experiment 2. Right) Position of launcher for angled launches in Experiment 3 where the ball's initial position is the same as the higher height position.
```

Note: For this experiment as well as the third experiment later on, while we could use our determined value for gravity, for simplicity, we will instead use the accepted value of $g = 9.803\,\text{m/s}^2$ for Fairfield, CT.

In this second experiment, we will **1)** first investigate the horizontally launched trajectory of the same metal ball used in the first experiment (launched at 90° relative to $g$, or 0° relative to the floor). Then **2)** we will attempt to estimate where the ball will land when launched from a different height and see how accurate we are.

This setup will involve a marble launcher that can slide into a large holder at different initial heights $y_{0}$ (and later for the third experiment, different angles, see {numref}`M03-simpleProjectileLauncher`). Height $y_{0}$ will be measured from the bottom of the ball (effectively the bottom inside of the launcher's barrel) to the floor. Once the ball is released, it will begin a two-dimensional trajectory accelerated solely by gravity in the $y$ direction.

**-1-)** The distance in the $x$ direction will be measured from the center of the ball in the uncocked position (a plum bob can be used to find the ball's initial position on the floor) to the average landing position on the floor after the given number of trials. The ball will mark up paper with carbon paper; we will circle this scatter shot and estimate the average position of all trials from the given case, and then measure the distance with a 1 or 2 meter stick to determine $x$.

After investigating how far the ball travels in the $x$ direction from a given height, we can determine characteristics about the launcher-and-ball system to estimate how far in the $x$ direction we may expect the ball to travel in the second part of this experiment when we launch it from a different initial height. To estimate how far the ball will travel, we can use {eq}`eq-M03-horizontal-Kinematic` to determine $x$. However, to do so, we will need to for how long and how fast it was moving (distance traveled = speed × time). Since we know the initial height $y_{0}$ of the ball, we can determine the time $t$ it took to fall to the floor in the $y$ direction due solely to gravity $g$ by rearranging {eq}`eq-M03-Kinematic-vertical-02` to solve for $t$, knowing that $v_{0y} = 0\,\text{m/s}$ and treating the floor as $y = 0\,\text{m}$:

```{math}
:label: eq-M03-Kinematic-vertical-time
0 = y_{0} + 0 - \frac{1}{2}gt^{2}~~~=>~~~\sqrt{\frac{2y_{0}}{g}} = t
```

Now that we know the time $t$ of the trajectory, and treating the uncocked position as $x_{0} = 0\,\text{m}$, we can use {eq}`eq-M03-horizontal-Kinematic` to determine the horizontal velocity $v_{x}$ when released:

```{math}
:label: eq-M03-Kinematic-horizontal-velocity-01
x = 0 + v_{x}t~~~=>~~~\frac{x}{t} = v_{x}
```

**-2-)** For the second part of this experiment, we move the launcher to the higher 0° slot (~20 cm higher), and we want to determine how far it will travel in the $x$ direction. This leads us back to {eq}`eq-M03-horizontal-Kinematic` where we want to solve for $x_{\text{higher height}}$ (where again, $x_{0} = 0\,\text{m}$ in the uncocked position):

```{math}
:label: eq-M03-Kinematic-horizontal-velocity-02
x = 0 + v_{x}t~~~=>~~~x_{\text{higher height}} = v_{x}t_{\text{higher height}}
```

We know the ball's velocity $v_{x}$, but we no longer know the time. However, similar to before, we can solve for $t_{\text{higher height}}$ by plugging $y_{0\text{,higher height}}$ into {eq}`eq-M03-Kinematic-vertical-time`:

```{math}
:label: eq-M03-Kinematic-vertical-time-higher-height
\sqrt{\frac{2y_{0\text{,higher height}}}{g}} = t_{\text{higher height}}
```

This subsequent value for time $t_{\text{higher height}}$ can be used in {eq}`eq-M03-Kinematic-horizontal-velocity-02` to then calculate a theoretical distance $x_{\text{higher height, theoretical}}$. We will then launch the ball from this higher height see how accurate we estimated $x_{\text{higher height, theoretical}}$. The experimentally determined $x_{\text{higher height, experimental}}$ will be measured in the same way as the first part of this experiment (circling and estimating the center of the scattershot).



### Angled Trajectory (Third experiment)

The third part of this experiment is similar to the 2nd part of the second experiment in that we are staying at the higher height, but now investigating the trajectories when launched from different angles, namely, how far in the $x$ direction do they reach? The large, launcher holder is designed to hold the ball at rest (uncocked) in the same position (height) regardless of angle, so you should be able to use your previously determined $y_{0\text{,higher height}}$ as your value for the ball's initial height (see {numref}`M03-simpleProjectileLauncher` right).

By launching at an upward angle $\theta$, we are now giving some of the initial velocity to both $x$ and $y$ directions. Once again, as there is no acceleration in the $x$ direction, we will ultimately use {eq}`eq-M03-horizontal-Kinematic` to determine $x_{\theta}$. However, we need to know both $v_{x\theta}$ and $t_{\theta}$. The velocity will merely be the horizontal component of the launch angle:

```{math}
:label: eq-M03-Kinematic-horizontal-velocity-03
v_{x\theta} = v_{x}\cos{\theta}
```

```{figure} SimpleProjectileFigures/M3_Exp3_v2025-01.png
:name: M03-simpleProjectileLauncher-Exp3
:width: 80%
:align: center

Example of the upward and downward portions you'll analyze in Experiment 3 for an angled launch.
```

To solve for the time, however, we can characterize motion in the $y$ direction to determine for how long the ball is in the air.

As shown in {numref}`M03-simpleProjectileLauncher-Exp3`, we can find that total time by breaking the trajectory into parts (i.e. $t_{\theta}~=~t_{\text{up}}~+~t_{\text{down}}$) where $t_{\text{up}}$ is the time for upward travel to the peak height, and $t_{\text{down}}$ is the time for downward travel to the floor from that peak height. **UPWARD PORTION)** Starting with {eq}`eq-M03-Kinematic-vertical-01`, where we know for the upward travel portion the initial velocity in the $y$ direction is $v_{0y} = v_{0y\text{ higher height}} = v_{x}\sin{\theta}$ and at the peak of the trajectory (end of the upward travel) $v_{y} = v_{y\text{peak}} = 0\,\text{m/s}$, thus:

```{math}
:label: eq-M03-Kinematic-vertical-time-03-v2-pt1
v_{y\text{ peak}} = v_{0y\text{ higher height}} - gt~~~=>~~~0 = v_{x}\sin{\theta} - gt_{\text{up}}~~~=>~~~\frac{v_{x}\sin{\theta}}{g} = t_{\text{up}}
```

**DOWNWARD PORTION)** Then for the downward travel, we need to first know how high we travelled during the upward portion (i.e. $y_{0\text{,higher height}} \text{ to } y_{\text{ peak}}$) so we can use {eq}`eq-M03-Kinematic-vertical-02` later to determine the time it took to fall from $y_{\text{ peak}} \text{ to } y_{\text{ floor}}$. Since we know our initial height $y_{0} = y_{0\text{,higher height}}$, initial velocity $v_{0} = v_{0y\text{ higher height}} = v_{x}\sin{\theta}$, and the time it took to get $t_{\text{up}}$ there from {eq}`eq-M03-Kinematic-vertical-time-03-v2-pt1`, we can use {eq}`eq-M03-Kinematic-vertical-02` to solve for the final height of the upward travel $y_{\text{peak}}$:

```{math}
:label: eq-M03-Kinematic-vertical-time-03-v2-pt2
y_{\text{peak}} = y_{0\text{,higher height}} + v_{x}\sin{\theta}t_{\text{up}} - \frac{1}{2}gt_{\text{up}}^{2}
```

Now that we know $y_{\text{peak}}$, we can use {eq}`eq-M03-Kinematic-vertical-02` to solve for $t_{down}$, this time with the final height $y_{\text{floor}} = 0\,\text{m}$, initial height of $y_{\text{peak}}$, and the initial velocity $v_{y\text{ peak}} = 0\,\text{m/s}$.

```{math}
:label: eq-M03-Kinematic-vertical-time-03-v2-pt3
y_{\text{floor}} = y_{\text{peak}} + v_{y\text{ peak}} - \frac{1}{2}gt_{\text{down}}^{2}~~~=>~~~0 = y_{\text{peak}} + 0 - \frac{1}{2}gt_{\text{down}}^{2}~~~=>~~~\sqrt{\frac{2y_{\text{peak}}}{g}} = t_{\text{down}}
```

**HORIZONTAL DISTANCE)** Finally, we have the total time $t_{\theta}~=~t_{\text{up}}~+~t_{\text{down}}$ from {eq}`eq-M03-Kinematic-vertical-time-03-v2-pt1` and {eq}`eq-M03-Kinematic-vertical-time-03-v2-pt3` and the initial velocity $v_{x}$ from {eq}`eq-M03-Kinematic-horizontal-velocity-03` to incorporate into {eq}`eq-M03-horizontal-Kinematic` to determine the theoretical distance $x_{\theta}$ the ball with travel in the $x$ direction for any given angle $\theta$:

```{math}
:label: eq-M03-Kinematic-vertical-time-03-v2-pt4
x_{\theta} = v_{x}\cos{\theta}t_{\theta}
```



## Experimental Procedure


<iframe width="560" height="315" src="https://www.youtube.com/embed/NvrdZoWNI5Q?si=ZyCPpqmxdyTGzqpZ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### EXPERIMENT 1 -- Free Fall / Downward Trajectory

```{admonition} OVERVIEW
:class: note
- Investigate projectile motion in one-dimension ($y$).
- Conduct 5 trials of the free-fall and determine acceleration due to gravity using one-dimensional kinematics.
```
```{admonition} POINT TO CONSIDER
:class: note
Will this experiment be more or less accurate in measuring $g$ than the previous lab using gliders on a tilted air track?
```
```{admonition} NOTE
:class: note
- There are only 4 setups, please share, and once you're done taking your data, move on to ensure other groups have a reasonable chance to use the apparatus.
- PASCO TIMER Precision: 0.0001 seconds
```

1. Create a data table for this experiment:
    - Common data section with the accepted value of $g$, the ball height $y_{0}$, and the ball height's estimated uncertainty $\delta y$.
    - With **five rows** (1 for each of the 5 free-fall trials). Also include additional **rows** for the average $g$ value, the $\pm$ uncertainty in gravity $\delta g$, the magnitude difference compared to the accepted $g$ *DISCUSSION POINT for later*: How well does you average value of $g \pm \delta g$ agree with the accepted value of $g$?).
    - Include **six columns** for
        - Initial time $t_{\text{initial}}$
        - Initial time uncertainty $\delta t_{\text{initial}}$
        - Final time $t_{\text{final}}$
        - Final time uncertainty $\delta t_{\text{final}}$
        - Total elapsed time $t = t_{\text{final}} - t_{\text{initial}}$
        - Total elapsed time uncertainty $\delta t = t_{\text{final}} - t_{\text{initial}}$
        - Calculated $g$

2. CAPSTONE will be set up with the Free-Fall Adapter which, whenever the circuit opens or closes, will record the time that event occurred.

3. Place your metal ball from your marble launcher into the spring loaded holder at one of the four setups. You will need to push the metal tab in and then hand-tighten the holding/release screw to hold the ball in place.

4. Ensure the receptor pad is beneath the ball such that it hits close to the open side.

5. Measure the height the ball will fall; the initial height $y_{0}$ is measured from the bottom of the ball to the top of the receptor plate which has a final height $y = 0\,\text{m}$ if you place the meter stick on the receptor pad.

6. Press Record in CAPSTONE. You can let it run and it'll continue collecting data even when you reset the ball for additional trials; or restart for each trial, just be aware of which data points are related to your drop.

7. Unscrew the holding/release screw to allow the ball to fall.

8. Record your $t_{\text{initial}}$ and $t_{\text{final}}$ times.

9.  Repeat the drop for a total of 5 free-fall trials. Determine the total elapsed times $t$ for each trial.

10. Using {eq}`eq-M03-Kinematic-freefall-g`, calculate the value of $g$ for each of your trials (benefit here of calculating $g$ from each trial: you can more easily notice any outlier data).

11. Determine your average $g$ from the preceding values.

12. Estimate your uncertainty in $g$, as represented by $\delta g = g_\text{test} - g$, (i.e. how confident [$\pm$] you are in what you measured -- e.g. distance, time). Plug in each measurements' uncertainties to make your test value of $g_\text{test}$ as calculated with {eq}`eq-M03-Kinematic-freefall-g` as big as possible (i.e. larger numerator, smaller denominator). Determine $\delta g$.

13. Compare your average $g$ to the accepted value of $g = 9.803\,\text{m/s}^2$; what is the total difference?

14. Does you average $g \pm \delta g$ cover the difference from the accepted value and agree, or not?


### Horizontal Trajectory (Second experiment)

```{admonition} OVERVIEW
:class: note
- Investigate projectile motion in two-dimensions when launched horizontally.
- For simplicity and to decrease error propagation, **for the rest of lab, assume and use** the accepted value of $g = 9.803\,\text{m/s}^2$ for Fairfield, CT rather than your previously determined value.
- Characterize the trajectory from the marble launcher at initial height.
- Calculate the theoretical trajectory (distance $x$) for a different height; place a bullseye at your expected location and compare your experimental landing scattershot to the theoretical distance.
- Conduct 20 launches for each height; estimate the experimental landing scattershot by circling your carbon-paper dots and estimating the center of the scattershot.
```

2. Create a data table for this experiment:
    - Common data section with the accepted value of $g$.
    - Section for the case at a the lower initial height containing:
        - the ball height $y_{0}$
        - the ball height's estimated uncertainty $\delta y_{0}$
        - distance $x$
        - distance uncertainty $\delta x$ based on the radius of the circle you draw around the scattershot
    - Additional sections for derived time of the trajectory $t$ and velocity $v_{x}$
    - Additional sections for:
        - Height of the ball at the higher $0°$ slot height $y_{0\text{,higher height}}$
        - Time of the trajectory from a higher height $t_{\text{higher height}}$
        - Theoretical distance $x_{\text{higher height, theoretical}}$ (calculated with {eq}`eq-M03-Kinematic-horizontal-velocity-02`)
        - Experimentally measured distance $x_{\text{higher height, experimental}}$
        - Estimated uncertainty in the experimental distance $\delta x_{\text{higher height, experimental}}$ (essentially $\pm$ the radius of the circle drawn around your scattershot)
        - Difference (magnitude) between the theoretical and experimental $x$ distances

3. Place the marble launcher in the holder in the lower $0°$ slot (uncocked to represent where the ball will be once the piston is no longer accelerating the ball up to speed)

4. Measure the height the ball will fall; place the metal ball into the launcher as the initial height $y_{0}$ is measured from the bottom of the ball to the floor (though the bottom of the inside of the barrel can also be used as the bottom of the ball location if that is easier to measure).

5. Conduct a couple test launches by pulling the piston to the first or second notches (whichever position provides the shorter, $\sim 1\,\text{m}$, $x$ distance). Take mental note of where the ball is generally landing.

6. Get a piece of paper and tape it in the approximate location, and place (no tape needed) a piece of carbon paper on top (no need to tape that one) so the ball can mark up the paper when it lands.

7. Conduct **20 launches** onto the paper/carbon paper.

8. Put aside the carbon paper and mark the dots with a marker or something else that makes it apparent which dots are your data points for this height. Draw a rough circle surrounding the scattershot and visually estimate the center by drawing a cross hair to represent the center of the scatter.

9. Measure the experimental distance $x$ from the center of the ball at rest in the barrel (uncocked) to the cross hair center that you drew in your scatter shot on the floor. To translate the initial location of the ball in the barrel to the floor, you can use a plum bob to make a straight line down to the floor, from which you can more easily measure $x$

10. From your circle around your scattershot, estimate your uncertainty in distance $\delta x$

11. Move the marble launcher to the higher $0°$ slot and remeasure the initial height $y_{0\text{,higher height}}$

12. Now calculate the theoretical distance $x_{\text{higher height, theoretical}}$ using {eq}`eq-M03-Kinematic-vertical-time` -- {eq}`eq-M03-Kinematic-vertical-time-higher-height`

13. Repeat steps 5 to 10 to determine experimentally the distance with its uncertainty at the higher height (i.e. $x_{\text{higher height, experimental}}$ and $\delta x_{\text{higher height, experimental}}$). **ADDITIONALLY: Before any launches from the higher height, draw a bullseye at the theoretical distance you expect the balls at the higher height to land to visually see how close we get. You can draw both a cross hair for the distance and estimate how big the scatter will be (to discuss later in {ref}`interpretation3`).**

14. Calculate the difference between you theoretical and experimental values of $x$ at the higher height.

15. DISCUSSION POINT (covered in {ref}`interpretation3`): Does your experimental distance of the higher height agree with what you expected from your theoretical calculation? In other words, does $x_{\text{higher height, experimental}} \pm \delta x_{\text{higher height, experimental}}$ overlap with $x_{\text{higher height, theoretical}}$ (i.e. does your uncertainty cover the difference between the experimental and theoretical values?)?










### Angled Trajectory (Third experiment)

```{admonition} OVERVIEW
:class: note
- Investigate projectile motion in two-dimensions when launched at a non-zero angle (for now, we'll use the 45° slot; if labs go well this semester, we may add additional angles).
- Calculate the theoretical trajectory (distance $x$) for a non-zero angle; place a bullseye at your expected location and compare your experimental landing scattershot to the theoretical distance.
- Compare the theoretical trajectory's $x$ distance to the experimentally determined distance.
- Conduct 20 launches for each angle; estimate the experimental landing scattershot by circling your carbon-paper dots and estimating the center of the scattershot, with your uncertainty represented by the radius of the drawn circle.
```
```{admonition} NOTE
:class: note
- Continue to use the accepted value of $g = 9.803\,\text{m/s}^2$ for Fairfield, CT rather than your previously determined value.
```

1. Create a data table for this experiment:
    - Common data section with the accepted value of $g$ and any values you will need from previous experiments to determine the theoretical distance at a given angled launch $x_{\theta}$ ({eq}`eq-M03-Kinematic-horizontal-velocity-03` to {eq}`eq-M03-Kinematic-vertical-time-03-v2-pt4`).
    - Additional sections for:
        - Theoretical distance $x_{\theta\text{, theoretical}}$ (calculated with {eq}`eq-M03-Kinematic-vertical-time-03-v2-pt4`)
        - Experimentally measured distance $x_{\theta\text{, experimental}}$
        - Estimated uncertainty in the experimental distance $\delta x_{\theta, experimental}$ (essentially $\pm$ the radius of the circle drawn around your scattershot)
        - Difference (magnitude) between the theoretical and experimental $x$ distances

2. Place the marble launcher in the holder in the 45° slot

3. Use your previously measured $y_{0\text{,higher height}}$ as the height the ball will fall for any angled launches (e.g. $y_{0\text{,higher height}} = y_{\theta\text{,higher height}}$).

4. Calculate the theoretical distance $x_{\text{, theoretical}}$ using {eq}`eq-M03-Kinematic-horizontal-velocity-03` to {eq}`eq-M03-Kinematic-vertical-time-03-v2-pt4`

5. Before any launches from the higher height, tape a paper and draw a bullseye at the theoretical distance you expect the balls at the given angle to land to visually see how close we get. You can draw both a cross hair for the distance and estimate how big the scatter will be.

6. Conduct a few test launches by pulling the piston to the same notch you've been using in Experiment 2 to be able to use the same exit velocity as previously determined

7. If need be, tape additional paper in the location from the test launches. Place (no tape needed) a piece of carbon paper on top (no need to tape that one) so the ball can mark up the paper when it lands.

8. Conduct **20 launches** onto the paper/carbon paper.

9.  Put aside the carbon paper and mark the dots with a marker or something else that makes it apparent which dots are your data points for this height. Draw a rough circle surrounding the scattershot and visually estimate the center by drawing a cross hair to represent the center of the scatter.

10. Measure the experimental distance $x$ from the center of the ball at rest in the barrel (uncocked) to the cross hair center that you drew in your scatter shot on the floor. The initial position of the ball in the $x$ direction translated to the floor should be the same as Experiment 2 (to save you some time). Remeasure if that's no longer the case (e.g. you've accidentally moved the launcher holder)

11. From your circle around your scattershot, estimate your uncertainty in distance $\delta x$

12. Calculate the difference between you theoretical and experimental values of $x$ at the given angle.

13. If there are additional angles assigned, move the marble launcher to the respective angle and repeat steps 5 to 13 if needed.

14. DISCUSSION POINT (covered in {ref}`interpretation3`): Does your experimental distance of the given angle(s) agree with what you expected from your theoretical calculation(s)? In other words, does $x_{\theta\text{, experimental}} \pm \delta x_{\theta\text{, experimental}}$ overlap with $x_{\theta\text{, theoretical}}$ (i.e. does your uncertainty cover the difference between the experimental and theoretical values?)?

(interpretation3)=
## Post-Lab Submission --- Interpretation of Results
<!---
- Make sure to submit your finalized data table (Excel sheet)
- What type of system do the kinematic equations represent?
- Experiment 1:
  - What are your results ($g \pm \delta g$), and how do they compare to the accepted value in Fairfield, CT?
    - In other words, for Experiment 1, COMPARE your experimental result of $g$ to the accepted values. Does $g \pm \delta g$ overlap (and therefore agree) with the accepted value?
  - What are the uncertainties of Experiment 1?
  - Would a different sized marble change your derived value of $g$? Why or why not?
- Experiment 2:
  - What were your results for the horizontal trajectories at both lower and higher heights?
  - Does your experimental distance of the higher height agree with what you expected from your theoretical calculation?
    - In other words, does $x_{\text{higher height, experimental}} \pm \delta x_{\text{higher height, experimental}}$ overlap with $x_{\text{higher height, theoretical}}$ (i.e. does your uncertainty cover the difference between the experimental and theoretical values?)?
  - What uncertainties might make this difference larger or smaller?
  - Was your bullseye target accurate to the experimental results?
- Experiment 3:
  - What were your results for the trajectories from a non-zero angle(s)?
  - Does your experimental distance agree with what you expected from your theoretical calculation?
    - In other words, does $x_{\theta\text{, experimental}} \pm \delta x_{\theta\text{, experimental}}$ overlap with $x_{\theta\text{, theoretical}}$ (i.e. does your uncertainty cover the difference between the experimental and theoretical values?)?
  - What uncertainties might make this difference larger or smaller?
  - Was your bullseye target accurate to the experimental results?
- What is the precision of your equipment?
- What are possible systematic errors for today's experiments?
--->

- Make sure to submit your finalized data table (Excel sheet)
- In a **paragraph** per experiment, summarize the results you have determined in each case:
	- What type of system do the kinematic equations represent?
	- **Experiment 1:**
	  - What are your results ($g \pm \delta g$), and how do they compare to the accepted value in Fairfield, CT?
	    - In other words, for Experiment 1, COMPARE your experimental result of $g$ to the accepted values. Does $g \pm \delta g$ overlap (and therefore agree) with the accepted value?
	  - Would a different sized marble change your derived value of $g$? Why or why not?
	- **Experiment 2:**
	  - What were your results for the horizontal trajectories at lower, higher height, and higher height at an angle? Do your results overlap with your theoretical value? Why or why not?
	- **Experiment 3:**
	  - What were your results for the trajectories from a non-zero angle(s)? Do your results overlap with your theoretical value? Why or why not?
 
- In a **paragraph** per experiment, summarize your error analysis. Be qualitative, not only quantitative. 
	- What is the precision of your equipment?
	- What are possible systematic errors for today's experiments?
	- **Experiment 1:**
		- What are the uncertainties of Experiment 1?
		-  Does your experimental distance of the higher height agree with what you expected from your theoretical calculation?
			- In other words, does $x_{\text{higher height, experimental}} \pm \delta x_{\text{higher height, experimental}}$ overlap with $x_{\text{higher height, theoretical}}$ (i.e. does your uncertainty cover the difference between the experimental and theoretical values?)?
	- **Experiment 2:**
		- What uncertainties might make this difference larger or smaller?
		- Was your bullseye target (estimation) accurate to the experimental results? Back up your answer with your results.
	- **Experiment 3:**
		-  Does your experimental distance agree with what you expected from your theoretical calculation?
		    - In other words, does $x_{\theta\text{, experimental}} \pm \delta x_{\theta\text{, experimental}}$ overlap with $x_{\theta\text{, theoretical}}$ (i.e. does your uncertainty cover the difference between the experimental and theoretical values?)?
      - What uncertainties might make this difference larger or smaller?
      - Was your bullseye target (estimation) accurate to the experimental results? Back up your answer with your results.


## The Whiteboard

```{figure} SimpleProjectileFigures/ProjectileKinetmatic_2024_Fall_01.jpg
:name: pro1
:width: 600px
:align: center

```

```{figure} SimpleProjectileFigures/ProjectileKinetmatic_2024_Fall_02.jpg
:name: pro2
:width: 600px
:align: center

```

