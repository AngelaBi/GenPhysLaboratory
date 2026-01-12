(simple-pendulum-g-lab-overall)=
# Determination of Acceleration due to Gravity, *g*, with Simple Pendulum

## Background

```{admonition} OVERALL GOALS
:class: note
Investigate the simple harmonic motion of a simple pendulum by:
- Examining the relationship between a simple pendulum's length and period
- Determining acceleration due to g
```

In this lab, the acceleration due to gravity is determined by measuring the parameters of the nearly simple harmonic motion of a simple pendulum.  The construction of the pendulum and restrictions on the motion of the pendulum permit some simplifying assumptions to be used to derive a relationship for $g$ in terms of easily measured parameters.

The gravitational attraction of the Earth on any massive body provides a force, which can accelerate a mass free to move under the influence of this force.  This acceleration $g$ is dependent on the mass of the earth and inversely on the distance of the mass from the center of the earth.  The value of $g$ is usually assumed to be constant over small vertical distances, i.e. distances that are small with respect to the distance to the center of the earth. Thus we will compare our results to the accepted value of $g$ at in Fairfield, CT ($g = 9.803\,{\rm m}/ {\rm s^2}$).

A pendulum is a massive body suspended such that it can swing freely.  In the general case, the mass of the pendulum is an extended mass and is called a physical pendulum.  An example of a physical pendulum might be a long piece of lumber, which is suspended from a nail through a hole near one end of the wood. This pendulum, when displaced sideways from its rest position, will swing back and forth under the influence of gravitational force which acts to restore the pendulum to its stationary hanging position.  The harmonic motion of the swinging pendulum must be analyzed carefully by considering torque on the pendulum and the pendulum's inertia.  The torque is the turning force produced by gravity and its inertia is the total effect of all the mass parts of the pendulum resisting rotation around the pivot.  The torque and inertia are exactly analogous to force and mass in the linear motion case described by Newton's Second Law, $F = m a$.

When all of the mass of the pendulum can be considered at a common distance from the pivot, then the physical pendulum is a ***simple pendulum***.  An example of a simple pendulum is a relatively small, massive object suspended from a long, nearly massless connection to a pivot like a short, heavy bolt, tied to a pivot with a thin thread.

Under the assumption of a simple pendulum, the analysis of the motion can be carried out using Newton's Laws of Linear Motion that we have seen in class. {numref}`M03_pendulum_Fig01` illustrates a simple pendulum at some arbitrary point in its swinging motion back and forth. We define this point by the angle of the thread with the vertical, indicated by the dashed line. The forces acting on the mass are its weight straight down and the tension in the thread. The weight can be resolved into a component along the direction of the thread and a component perpendicular to the thread, i.e. along the tangent of the arc of the swing.

```{figure} PendulumFigures/M10_figure1_squish_v01.jpg
:name: M03_pendulum_Fig01
:width: 70%
:align: center

Force Diagram and variables used in the pendulum experiment.
```

$F_{1}$, the force along the direction of motion, is equal to $F \sin(\theta) = m g \sin(\theta)$.  We will now make a further simplifying assumption which is to assume that the maximum angular displacement, i.e. the maximum value of $x$, is small.  If the value of $x$, and therefore $\theta$, is small, then the magnitude of both the $\sin(\theta)$ and $\tan(\theta)$ are essentially equal to $\theta$, measured in radians. 

```{admonition} Small-Amplitude Approximation
:class: note
For small angles, the value of the $\sin(\theta) = x/L$.  
```

The implication of this small-angle assumption is that the pendulum never swings very far from the vertical. Therefore the restoring force, i.e. the force that is acting to return the pendulum to its equilibrium vertical position, is assumed to be acting *horizontally*.  This is clearly never true except at the equilibrium position where the restoring force is zero.  The implication of this assumption is that the actual restoring force is always *less* than the value we assume it to be.

<!--- check on this ^^^ --->

The period of the pendulum is the time it takes to swing through a complete cycle, or one complete swing out and back to the starting point. Using the small angle assumption described above, we can write the restoring force as

```{math}
F = -m g \sin(\theta) = -m g \frac{x}{L}.
```

The minus sign means that the restoring force is in the opposite direction from the displacement $x$. When the restoring force of a system is of the form $F = -k x$, the system will oscillate in simple harmonic motion.

To see what this motion looks like we will use Newton's Second Law,

```{math}
:label: M03_pendulum_Eq01
F = -m g \frac{x}{L} = m a
```

where $a$ is the acceleration of the mass in the $x$-direction.

```{admonition} Deriving Period $T$
:class: note
The following steps reviews the derivation of the pendulum's period for small angles. This is good for review, however you can jump to {eq}`M03_pendulum_Eq02`.
```

Substituting the definition of acceleration

```{math}
a = \frac{{\rm d}^2 x}{{\rm d} t^{2}}
```

into {eq}`M03_pendulum_Eq01` yields an equation for displacement, $x$, as a function of time, $t$, namely

```{math}
-\frac{mg}{L} x(t) = m \frac{{\rm d}^2 x}{{\rm d} t^{2}}.
```

Upon simplifying, the mass, $m$, disappears, yielding

```{math}
x(t) = -\left(\frac{L}{g}\right) \frac{{\rm d}^2 x}{{\rm d} t^{2}}.
```

This second order, linear, differential equation has a solution

```{math}
x(t) = A \cos\left(2\pi \frac{t}{T} \right)
```

where the amplitude $A$ is the maximum value of $x$; $T$ is the period; and the motion is such that at $t = 0$, the pendulum is at its maximum displacement, i.e. $x = A$. Note that the motion is independent of the mass. Substitution of this solution into the differential equation yields an expression for the period of a small-amplitude pendulum as

```{math}
:label: M03_pendulum_Eq02
T = 2\pi \sqrt{\frac{L}{g}}.
```

Rearranging this expression we can similarly obtain a small-amplitude-approximated value

```{math}
:label: M03_pendulum_Eq03
g = 4\pi^2 \frac{L}{T^2}
```

and, for our uses of plotting our experimental data later on,

```{math}
:label: M03_pendulum_Eq07
T^2 = \frac{4\pi^2}{g} L
```

Had we not constrained the motion of the pendulum to small amplitudes, the expression for the period would be given by the small-amplitude approximation multiplied by an infinite Taylor Series of additional, smaller correction terms

```{math}
:label: M03_pendulum_Eq04
T = 2\pi \sqrt{\frac{L}{g}}  \left[ 1 +
  \frac{1}{ 4} \sin^2\left(\frac{\theta}{2}\right) +
  \frac{9}{64} \sin^4\left(\frac{\theta}{2}\right) + \ldots \right]
```

Thus as the angle gets larger, the period increases as those additional terms become significant. You can see example of this by the slightly longer period of the large angle example in {ref}`SimplePendulumDemoVideo-01`. 

For our uses today, we will only focus on the first three terms of the Taylor Series, and call everything in the brackets our ***Taylor Series correction factor***, denoted as $C_\text{Taylor}$, such that

```{math}
:label: M03_pendulum_Eq08
C_\text{Taylor} = \left[ 1 +
  \frac{1}{ 4} \sin^2\left(\frac{\theta}{2}\right) +
  \frac{9}{64} \sin^4\left(\frac{\theta}{2}\right) \right]
```

simplifies our equation for the period to

```{math}
:label: M03_pendulum_Eq09
T = 2\pi \sqrt{\frac{L}{g}} \times C_\text{Taylor}
```

When the pendulum swings with very small angles, the period is essentially independent of the amplitude.  However, from the more precise expression above for the period, this is not strictly true.  An amplitude decrease could result from the effects of friction in the pivot or air drag of the thread and mass.  Pendulum clock makers go to great pains to not only keep the length constant, but the amplitude of the swing as well.  Since we will average over many cycles, we must also assume that the amplitude does not change as we measure the period.  In our experiment, we might be tempted to average a very large number of cycles to reduce measurement errors.  However the necessarily larger initial amplitude together with the decreasing amplitude caused by friction effects would change the average period.  For the last case, we will do just that by deliberately starting with a large amplitude and observe whether there is an increase in the measured period.
















## Experimental Procedure



```{admonition} OVERVIEW
:class: note
   - We study simple harmonic motion of a simple pendulum to derive acceleration due to gravity by comparing and contrasting the lengths and periods through 5 Cases of different-length pendulums:
   - Each Case with have either **10** or **15 trials**:
      - Each student will complete a total of 5 trials each, with:
        - Groups of 2 --- 10 trials
        - Groups of 3 --- 15 trials
```

```{admonition} Additional Tips
:class: tip
- The pendulum today is the combination of both the string and the ball. The pendulum length is the distance from the pivot point to the center of mass of the pendulum (i.e. the center of where force of gravity is overall acting upon --- therefore **center of the ball** since the string is much less massive).
```


### Preliminary Setup


1. **Five Cases:** For this experiment, you will use approximate pendulum lengths as listed in {numref}`tab-five-pendulum-length-cases`. You don't have to set the lengths to be exactly those lengths. The point here is to cover a wide range to investigate how the motion is dependent on pendulum length. Get close and make sure to measure the thread length carefully; record the measured value, and determine the total pendulum length for the given case. For each case, perform the following steps listed in {ref}`detailsteps-ConsEnTrack` and record the data appropriately in your spreadsheet.

    ```{table} Five experimental pendulum-length cases
    :name: tab-five-pendulum-length-cases
    | Case | Rough Pendulum Length | Angle Size |
    |:----:|:----------------:|:----------:|
    |  1   |     50 cm        |   small    |
    |  2   |    100 cm        |   small    |
    |  3   |    130 cm        |   small    |
    |  4   |    170 cm        |   small    |
    |  5   |    170 cm        |   LARGE    |
    ```

2. **NOTE ON NUMBER OF TRIALS:** For each of the five cases, each person will perform 5 time trials. Everyone can record at roughly the same time, but don't worry if you aren't all timing the exact same swings (i.e. someone starts a half or whole cycle late); just make sure to time a total of 10 cycles for each trial. By everyone taking data for 5 time trials each, and doing so simultaneously, a two-person group will end up with 10 total data points, and a three-person group will have 15 total data points for each case, etc. while saving time running the lab.


3. Create a data table for the given case (this table can be copied/pasted for the additional cases):
    - *Common data for the entire experiment* including the ball radius and the accepted $g = 9.803\,\text{m/s}^2$ for Fairfield.
    - *Common data for each individual case* including:
      - The case number
      - The case description
      - $y$: Measured thread length
      - $L$: Calculated pendulum length
      - $\delta L$: Estimated uncertainty in length
      - $\theta_\text{displacement}$: Approximate angle of displacement
    - *Data table* including, but not limited to:
      - Enough **rows** to include all time trials for your group
      - For each case, include **columns** for
        - Trial number
        - Lab member's initials
        - $t_{10\text{cycles}}$: Measured **total time** of the 10 cycles (swing out and back to initial position)
        - $\delta t_{10\text{cycles}}$: Estimated uncertainty in total time
        - $T$: Period of a single swing as determined from your measured time
        - $\delta T$: Uncertainty of the period similarly determined from $\delta t_{10\text{cycles}}$
        - $g_\text{small-amp}$: Experimental value of small-amplitude-approximated acceleration due to gravity
        - $\delta g_\text{small-amp}$: Uncertainty of small-amplitude-approximated experimental value from error propagation
        - $Difference\,(g_{\text{small-amp}} - g)$: Magntitude of difference between $g_{\text{small-amp}}$ and the accepted $g$, i.e. how far away your small-amplitude-approximated value is from the accepted value of $g$
        - $C_\text{Taylor}$: **Taylor Series correction factor**
        - $g_\text{corrected}$: *Corrected* value of $g_\text{small-amp}$ by incorporating the additional terms of the **Taylor Series correction factor** that increases the period
        - $Difference\,(g_{\text{corrected}} - g)$: Magntitude of difference between $g_{\text{corrected}}$ and the accepted $g$, i.e. how far away your corrected value is from the accepted value of $g$
      - Include an additional row for summarizing your results including, but not limited to:
        - $T_\text{avg}$: Average $T$ from all trials of the current case
        - $g_{\text{small-amp,avg}}$: Average small-amplitude-approximated $g$ from all trials of the current case
        - $\delta g_{\text{small-amp,avg}}$: Average uncertainty of $g$ from all trials of the current cases
        - $Average\,Difference\,(g_{\text{small-amp,avg}} - g)$: Average magntitude of difference between $g_{\text{small-amp}}$ and the accepted $g$
        - $g_\text{corrected,avg}$: Average corrected values of $g$
        - $Average\,Difference\,(g_{\text{corrected,avg}} - g)$: Average magntitude of difference between $g_{\text{corrected}}$ and the accepted $g$
        - $g_\text{slope}$: Slope-derived value of $g$ from fitting a trend line to all small-amplitude data points
        - $\delta g_\text{slope}$: Uncertainty of slope-derived value of $g$, found by propagating the uncertainty of the slope of the fit
        - $Difference\,(g_{\text{slope}} - g)$: Magntitude of difference between $g_{\text{slope}}$ and the accepted $g$
      - Include an additional section for plotting and analysis
        - Columns for all $L$ and $T^2$ values from all small-amplitude trials across all relevant cases combined together for easy plotting
        - Section for `LINEST` function. Must be an empty 2 column $\times$ 5 row section in your spreadsheet as those cells will be autopopulated by the `LINEST` function later on. Used for determining the slope and the slope's uncertainty



4. The total pendulum length $L$ can be determined from adding together the thread length $y$ and the ball radius:

      - Measure the thread length $y$. Attach one end of the thread to the provided pendulum clamp in such a way that you can accurately measure the distance from the pivot point to the top surface of the ball. Set the length of the thread approximately to the value for the case (doesn't have to be exact, we're just looking to test across a range of lengths across the cases).

      - Measure the diameter of the ball with Vernier calipers, determine its radius, add the radius of the ball to the thread length to establish the pendulum length $L$.
    
      - Estimate and note the uncertainty in the pendulum length $\delta L$; consider both each measurement tools' precision as well as your estimated confidence in your measurements (i.e. are you as confident as the tools' precision, or might it be a bit of a larger range?).

5. Note the approximate angle of displacement $\theta_\text{displacement}$ from rest position:
   - For cases 1--4, the starting displacement should be small (e.g. $\sim 1.5^\circ$ from the inner edge of the *narrow* arm of the red protractor).
   - For case 5, use a large angle (e.g. $\sim45^\circ$ from the inner edge of the *wide* arm of the red protractor).



(SimplePendulumDemoVideo-01)=
### Demo Video: Counting & Small vs. Large Angles
<div style="text-align: center;">
  <iframe
    width="80%"
    height="315"
    src="https://www.youtube.com/embed/sgJdCovemW4"
    title="YouTube video"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
  <figcaption>Demonstration video: shows suggested counting procedure by starting your counting on 0 so when you reach 10, you've counted 10 full cycles. Example of this is presented for both small and large angles. Also shown is the effect of a large angle on a pendulum, increasing the period and causing a pendulum of the same length to become out of sync with the small-angled pendulum.</figcaption>
</div>


(detailsteps-SimplePendulumData)=
### Experimental Data Collection
For each case, perform 5 trials per person (i.e. 10 or 15 total data points per two- or three-person group as mentioned above) as follows:

6. Measure the time $t_{10\text{cycles}}$ for 10 cycles of the pendulum. One cycle is going from the pendulum's initial position, swings out, swings back to its initial position. See example in {ref}`SimplePendulumDemoVideo-01`.
    - Start and stop the stopwatch at one end of a swing where the velocity is zero. It is better not to start the watch as you release the mass, but rather at a later point where $v = 0$. This will insure that your starting point is a consistent $v = 0$ point rather than having some initial velocity given to the ball when you release it.
    - Count one cycle as the mass returns to the starting point, i.e. after one complete swing out and back.
      ```{admonition} Suggestion for Counting: Index at 0
      :class: tip
      If you index your counting by starting at 0, where you would start the  stopwatch when you say zero, and stop the stopwatch when you say ten, you will have counted 10 full cycles.
      ```
7. Estimate your trial's time uncertainty $\delta t_{10\text{cycles}}$ based on your reaction time (generally ranging ~0.100 -- 0.300 seconds) and your stopwatch precision. (i.e. results are $t_{10\text{cycles}} \pm \delta t_{10\text{cycles}}$). *CONSIDER*: Where do the uncertainties come from?

8. Determine the period $T$ for one cycle from each trial of ten cycles. (Hint: how many cycles did you observe?)

9. Similarly, determine the period uncertainty $\delta T$ for one cycle from each trial.

10. Calculate the value of $g_\text{small-amp}$ for each trial using the small-amplitude approximation, {eq}`M03_pendulum_Eq03`.

11. Similarly, determine $\delta g_\text{small-amp}$, the uncertainty of your value for $g$. Make $g$ as large as your uncertainties allow and subtract the original value; the difference is the uncertainty in $g$. In other words, 
    - Maximize $g_{\text{small-amp,max}}$ with a smaller period and larger pendulum length: using ($T - \delta T$) as the period and ($L + \delta L$) to make $g_{\text{small-amp,max}}$ bigger by dividing by a smaller period and multiplying by a longer length. 
    - Then get the uncertainty by $\delta g_\text{small-amp} = g_{\text{small-amp,max}} - g_\text{small-amp}$.

```{math}
:label: M03_pendulum_Eq05
g_{\text{small-amp,max}} = 4\pi^2 \frac{(L + \delta L)}{(T - \delta T)^2}
```

12. Calculate the magnitude of the difference between your experimental value and the accepted value of $g$ (i.e. the difference $g_{\text{small-amp}} - g$).

    ```{admonition} Discussion Point: Accuracy
    :class: question
    Did your value agree with the accepted value of $g$? I.e. was your uncertainty larger than the magnitude of the difference between your value and the accepted? If not, what errors could cause worse accuracy or disagreement between them?
    ```

13. Calculate the corrected value, $g_\text{corrected}$ by:

    - Calculating the **Taylor Series correction factor** $C_\text{Taylor}$ using {eq}`M03_pendulum_Eq08` (i.e. the first three terms of the brackets of {eq}`M03_pendulum_Eq04`).
    - Then multiplying your small-amplitude experimental value by the square of your **Taylor Series correction factor**. This is like solving {eq}`M03_pendulum_Eq09` for $g$, leading to {eq}`M03_pendulum_Eq03` becoming {eq}`M03_pendulum_Eq06`. 
    - ***Note:*** Today, we will just assume the uncertainty of the corrected value is the same as $\delta g_{\text{small-amp}}$.

    ```{math}
    :label: M03_pendulum_Eq06
    g = 4\pi^2 \frac{L}{T^2} \left[ 1 +
    \frac{1}{ 4} \sin^2\left(\frac{\theta}{2}\right) +
    \frac{9}{64} \sin^4\left(\frac{\theta}{2}\right) \right]^2
    ```

    ```{admonition} Excel Syntax
    :class: tip
    - While we normally write a trig function to some power like $\sin^2\left(\frac{\theta}{2}\right)$; Excel does not know how to interpret that.
    - `SIN()`, `COS()`, etc. are Excel *functions* which take some `input` between the parentheses (e.g. `SIN(input)`) and then returns a value such that `output = SIN(input)`. Reminder, Excel likes radians; Excel's trig functions are expecting the input to be in units of radians.
    - To square any function's output in Excel is like saying `output`$^2$. To do such a thing with a trig function (or any Excel function for that matter), we would instead type `SIN(input-in-radians)^2`.
    ```

14. Calculate the magnitude of the difference between your corrected value and the accepted value of $g$ (i.e. the difference $g_{\text{corrected}} - g$).


15. Calculate your average values from everyone's trials for the current case:
    - $T_\text{avg}$, the average value of $T$
    - $g_{\text{small-amp,avg}}$, the average value of small-amplitude experimental value of $g$
    - $\delta g_{\text{small-amp,avg}}$, the average uncertainty of $g_{\text{small-amp,avg}}$
    - $Average\,Difference\,(g_{\text{small-amp,avg}} - g)$, the average difference between small-amplitude experimental value and accepted $g$
    - $g_\text{corrected,avg}$, the average corrected value of $g$
    - $Average\,Difference\,(g_{\text{corrected,avg}} - g)$, the verage difference between corrected and accepted $g$


16. **Graphical Analysis:**

    - Using ***all data points*** (not just the averages) from the four small amplitude cases (Cases 1--4), plot the square of the period, $T^2$, as a function of the length $L$ (i.e. dependent variable $T^2$ on y-axis, independent variable $L$ on x-axis). **Do not** use the large angle Case 5.
      - Draw the best fit line through your data points (force the fit to pass through the origin by setting the y-intercept to 0).
      - Display the equation for the fit line on your plot.
    - Determine the slope of your graph using the `LINEST` function:
      - `=LINEST(y-values,x-values,FALSE,TRUE)`
      - where the y-values at your $T^2$ values
      - x-values are your $L$ values
      - False to set the y-intercept to zero
      - True to return statistics on the fit
      ```{table} Simplified Excel LINEST Output (showing only slope and intercept)
      :name: tab-excel-linest-simplified
      | Row | Column 1 (Slope)                         | Column 2 (Intercept)                         |
      |:---:|-------------------------------------------|-----------------------------------------------|
      |  1  | **Slope value $m$** – best-fit line slope     | **Intercept value** – y-intercept of the line |
      |  2  | **Slope uncertainty $\delta m$** – std. error of m   | **Intercept uncertainty** – std. error of b   |
      |  3  | *(Ignored)* R² and related metrics        | *(Ignored)*                                   |
      |  4  | *(Ignored)* Additional regression stats   | *(Ignored)*                                   |
      |  5  | *(Ignored)* Residual statistics           | *(Ignored)*                                   |
      ```
    - Confirm your slope shown on your plot matches that calculated by the `LINEST` function
    - From the expression for the period, the measured slope, $m$, should give you your best estimate of the value of $g$. Since the expression for $T^2$ is given by {eq}`M03_pendulum_Eq07`, the slope of your graph, $m = 4\pi^2/g$. Thus your final value for $g_\text{slope}$ is $4\pi^2/m$.
    - Determine $\delta g_\text{slope}$, the uncertainty of your slope-derived value of $g$. Propagate the uncertainty of the fit's slope to maximize $g_\text{slope,maximized} = 4\pi^2/(m - \delta m)$, and take the difference (i.e. $\delta g_\text{slope} = g_\text{slope,maximized} - g_\text{slope}$).
    - Calculate the magnitude of the difference between your slope-derived value and the accepted value of $g$ (i.e. the difference $g_\text{slope} - g$).


    ```{admonition} Discussion Point: Experimental Averages vs. Accepted
    :class: question
    - Compare your experimental values' uncertainties $\delta g$ to the difference between the average value for the case and the accepted value of $g$.
    - Do your experimental values for $g$ agree with the accepted value of $g$. In other words, does $g \pm \delta g$ overlap with the accepted value by covering the difference between the experimental and actual values?
    - Think about this for your $g_{\text{small-amp,avg}}$, $g_{\text{corrected,avg}}$, $g_{\text{slope}}$.
    ```







## Post-Lab Submission --- Interpretation of Results
<!---
- Make sure to submit your finalized data table (Excel sheet)
- What are your experimental values of g, and how do they compare to the accepted value? Do this for:
  - Case averages of $g_{\text{avg}}$, (i.e. does $g_{\text{avg}} \pm \delta g_{\text{avg}}$ overlap with the accepted value by covering the difference between the experimental and actual values?)
  - Case averaged of $g_\text{corrected,avg}$ (assuming similar uncertainty)
  - Slope-derived $g_\text{slope}$ (assuming similar uncertainty)
- Case 5 (large angle):
  - How is Case 5 (large angle) different from the previous four?
  - How does $g_\text{avg}$ of Case 5 compare to $g_{\text{avg}}$ of Case 4 (at the same $L$)?
  - How does $g_\text{corrected,avg}$ of Case 5 compare to $g_{\text{avg}}$ of Case 4 (at the same $L$)? Do they agree more or less after the consideration of additional terms.
- How do the periods relate to different lengths of pendulum?
--->

### Finalized Spreadsheets

  - Make sure to submit your finalized data table (Excel sheet).
    - Please include relevant plot(s) including:
      - $T^2$ vs. $L$ with all data points across the four small-angle cases (i.e. Cases 1 -- 4)


### Post-lab Writeup

- In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
	- What is the precision of your equipment?
  - What are your systematic and random errors?
  - What are sources of uncertainty?
  - How do your final results change based on your uncertainties (e.g. maximizing/minimizing values)?
    - Of your quantities' uncertainties, which quantity affects your final result for $g$ the most?
<!--- ~!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! make g slope unceratinty from excel--->
- In a **paragraph**, summarize the results you have determined in each case. Consider:
  - Compare your averaged values to the accepted value of $g$ for Fairfield, CT, for each length case including:
    - $g_{\text{small-amp,avg}}\pm\delta g_{\text{small-amp,avg}}$
    - $g_{\text{corrected,avg}}\pm\delta g_{\text{small-amp,avg}}$ (reminder, reusing the uncertainty here)
    - $g_{slope}\pm\delta g_{slope}$
  - Do each of the small-angle cases agree with each other (Cases 1 -- 4)? Why or why not using physical arguements?
  - How do the **uncorrected** and **corrected** accelerations due to gravity values for the large angle case (Case 5) compare to the other cases, including Case 4 of the same pendulum length?
  - What is the relationship between period and length for a simple pendulum (i.e. longer/shorter)?

## The Whiteboard

```{figure} PendulumFigures/SimplePendulum_2024_Fall_01.jpg
:name: pen1
:width: 80%
:align: center

```

```{figure} PendulumFigures/SimplePendulum_2024_Fall_02.jpg
:name: pen2
:width: 80%
:align: center

```

```{figure} PendulumFigures/SimplePendulum_2024_Fall_03_v02.jpg
:name: pen3
:width: 80%
:align: center

```
