(wave-motion-overall)=
# Wave Motion

## Background

### ● Background Overview

```{admonition} OVERALL GOALS
:class: note
Use a vibrating string to:
- Investigate wave propagation through a medium
- Understand the relationship between wave frequency and wavelength
```


The general equation for the velocity of propagation of waves in a medium of continuously distributed stiffness and inertia is given by a formula of the form

```{math}
:label: eq-wave-velocity-general
v=\sqrt{\frac{\text{elasticity or stiffness factor}}{\text{density or inertial factor}}}
```

In the case of transverse waves propagated along a flexible cord, the elasticity or stiffness factor is due to the tension, $F_T$, in the cord; and the inertial factor is the linear density, $\mu=m/L$, of the cord. Thus the velocity of propagation, $v$, of a transverse wave is

```{math}
:label: eq-wave-velocity
v=\sqrt{\frac{F_T}{\mu}}
```

The velocity can also be determined from {eq}`eq-wave-frequency` by establishing standing waves with a known frequency, $f$. The wavelength, $\lambda$, is directly measurable from the spacing of nodes, or points of zero displacement. (The wavelength is twice the distance between successive nodes.)

```{math}
:label: eq-wave-frequency
v=\lambda f
```
A standing wave is produced when two identical waves travel in opposite directions in the same medium. The two waves interfere with each other forming a pattern of vibration that is stationary along the direction of propagation.


```{figure} WavesFigures/waves_2025_Spring_01_v03.jpg
:name: waves_harmonics_illustration
:width: 100%
:align: center

Illustration of 1st through 6th harmonics with their nodes/antinodes.
```


For our case, a wave is generated at one end of a cord by a string vibrator that moves the cord up and down at a measurable frequency. This wave travels down the cord to the other end and reflects back towards the source. As the wave reflects back and forth, augmented by the string vibrator at one end, the oppositely traveling waves interfere to produce a 'standing-wave' pattern of vibration. It can be shown that certain points of this pattern never move. They are called nodes (see {numref}`waves_harmonics_illustration`). Thus in order for a standing wave pattern to be produced on a cord that is effectively tied at both ends and cannot move, the pattern that is established must, at the very least, have nodes at each end (see fundamental in {ref}`demo-video-1-wavemotion-highspeed`).


(demo-video-1-wavemotion-highspeed)=
#### ○ Example Video: Waves on a String

<div style="text-align: center;">
  <iframe
    width="80%"
    height="315"
    src="https://www.youtube.com/embed/fQfNq8tJp3s"
    title="YouTube video"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin"
    allowfullscreen>
  </iframe>
  <figcaption>Demonstration video, examples of 1st, 2nd, 3rd harmonics. *No audio*</figcaption>
</div>

If embedding is broken, follow: <a href="https://www.youtube.com/watch?v=fQfNq8tJp3s" target="_blank" rel="noopener noreferrer">
https://www.youtube.com/watch?v=fQfNq8tJp3s
</a>




It can also be shown that the spacing of nodes is $\lambda$/2. Since the propagation velocity is only a function of the physical properties of the cord, the wavelength can be adjusted by selecting the appropriate frequencies of vibration that satisfy the condition of 'nodes at least at the ends'. Since the length of the cord must be such that nodes exist at each end, the length of the cord, tied at each end, must be an integral number of $\lambda$/2 and the allowable frequencies of vibration of the cord are integral multiples of each other. They are said to be harmonically related (see {numref}`waves_harmonics_illustration`).



In this experiment, similar to that seen in {ref}`demo-video-1-wavemotion-highspeed`, one end of a horizontal cord is attached to the string vibrator (see {numref}`fig-string-vibrator`) and the other end, after passing over a pulley, is attached to a hanging mass. We can adjust the amplitude and the frequency of the wave by adjusting the output of the sine wave generator, which powers the string vibrator. The tension is determined by the weight of the hanging mass. Therefore for a given tension and linear density, the frequency can be adjusted and measured for a standing wave condition. A measurement of node spacing establishes the wavelength. With the frequency and wavelength measured, the velocity can be determined from {eq}`eq-wave-frequency`. From a measurement of the linear density of the cord and the tension in the cord, we can independently determine the velocity from {eq}`eq-wave-velocity`. The two independently determined values of velocity of propagation can be compared.

```{figure} WavesFigures/DSC_6675.jpg
:name: fig-string-vibrator
:alt: Setup with sine wave generator and string vibrator experimental apparatus
:width: 600px
:align: center

Setup with sine wave generator and string vibrator.
```




### ● Equipment

```{table} Equipment
:name: waves-string-equipment-table

| Category | Items |
|---|---|
| **Signal Generation** | • Sine wave generator $(1 - 800\,\text{Hz}$, $0.1\,\text{Hz}$ resolution)<br>• Coarse and fine adjustment knobs ($1\,\text{Hz}$ and $0.1\,\text{Hz}$ increments)<br>• Amplitude control to adjust wave size (decrease to prevent string from hitting table) |
| **Wave Apparatus** | • PASCO String vibrator |
| **Electrical Connections** | • 2x banana-plug wires to connect sine wave generator to string vibrator |
| **Measurement Tools** | • Meter sticks ($1\,\text{m}$ and $2\,\text{m}$, additional on front wall) |
| **Mounting Hardware** | • Clamp to secure string vibrator to desk |
| **Strings** | • 2 strings of different linear densities (yellow and white)<br>• Length: $\sim 1-1.5\,\text{m}$ |
| **Mass & Tension System** | • Mass hanger of $\sim 50\,\text{g}$ with $100\,\text{g}$ and $200\,\text{g}$ disk masses (at front table)<br> • Black, low-friction pulley to convert hanging mass into string tension |
| **Force Measurement** | • PASCO High-Resolution Force Sensor<br>• Resolution: $0.002\,\text{N}$ or $0.0002\,\text{kg}$ |
```


## Experimental Procedure

### ● Preview


   ```{admonition} PROCEDURE OVERVIEW
   :class: note
   Investigate wave propagation through a medium for three cases (two different density strings at two different tensions)
    - Determine expected propagation velocity from linear density and tension measurements
    - Determine experimental propagation velocity by:
      - Vary and determine the frequency range of the sine wave generator where you achieve standing waves
      - Measure wavelength(s) from node to furthest acceptable node
   ```



### ● Preliminary Setup & Expected Velocity

The cases today are as shown in {numref}`waves-cases-table`.

```{table} Experimental Cases
:name: waves-cases-table

| Case | Cord Type | Total Mass (g) | Harmonics |
|------|----------|----------------|-----------|
| I    | White    | 250 | 1 - 6 |
| II   | White    | 350 | 1 - 6 |
| III  | Yellow   | 350 | 1 - 6 |
*Note: Total mass includes<br>the mass hanger (50 g).*
```

1. Create a common data table including necessary info for each case (but not limited to):
    - Accepted value of $g=9.803\,\text{m/}\text{s}^2$ for Fairfield, CT
    - cord masses
    - cord mass uncertainties
    - cord lengths
    - cord length uncertainties
    - calculated cord linear densities
    - linear density uncertainties
    - hanging masses
    - hanging mass uncertainties
    - tensions
    - tension uncertainties
    - expected propagation velocities
    - expected propagation velocity uncertainties

2. Measure the length and your estimated uncertainty of each cord by untying them completely and gently stretching them along a meter stick.

3. Weigh each cord using the force sensor as a digital scale with the provided Capstone file (see desktop). Zero sensor, hang string on hook; after values have settled (~5 - 10 seconds), highlight settled region of mass vs. time plot, see data table with associated data points highlighted, record mean and standard deviation (as mass uncertainty) to the nearest thousandth of a gram.

4. Calculate each cord's linear density (mass per unit length, $\mu=m/L$) and uncertainty by maximizing and taking the difference ($\delta\mu= (m+\delta m)/(L - \delta L) - \mu$).

5. Weigh each hanging mass (mass on hanger) and determine its uncertainty similar to how you found cords' masses earlier.

6. Calculate each hanging mass's related tension ($F_T = mg$) and uncertainty by maximizing and taking the difference ($\delta F_T = (m + \delta m) g - F_T$).

7. Calculate each case's expected propagation velocities using {eq}`eq-wave-velocity`, and similarly maximize and take the difference $\delta v=\sqrt{(F_T + \delta F_T) / (\mu - \delta \mu)} - v$


(section-waves-experimental-velocity)=
### ● Experimental Velocity

<!--- 
5. Create a common data table for each case including (but not limited to):
    - hanging mass
    - hanging mass uncertainty
    - tension
    - tension uncertainty
    - string linear density
    - string linear density uncertainty 
 
--->

8. Create a data table for the current case with rows for each trial (harmonic number $n = 1, 2, 3, 4, 5,$ and $6$) and average propagation velocity and uncertainty; columns for (but not limited to):
    - measured node-to-furthest-best-node distance
    - estimated node-to-furthest-best-node distance uncertainty
    - measured/determined wavelength $\lambda_n$
    - wavelength uncertainty $\delta \lambda_n$
    - minimum measured frequency $f_{n\text{,min}}$
    - maximum measured frequency $f_{n\text{,max}}$
    - the measured frequency $f_n$
    - the measured frequency uncertainty $\delta f_n$
    - the ratio $f_n/f_1$ of the $n$-harmonic's frequency to the fundamental
    - calculated propagation velocity $v_n=\lambda_n f_n$
    - calculated propagation velocity uncertainty

9. Tie one end of the cord to the vibrating blade, run it over the pulley, and hang the current case's total mass (slotted mass and hanger). 

10. Create the first-harmonic standing wave: Turn on the Sine Wave Generator and set the Amplitude knob about midway. Use the Coarse (1.0 Hz increments) and Fine (0.1 Hz increments) Frequency knobs of the Sine Wave Generator to adjust the vibrations so that the the cord vibrates in one segment. This first harmonic is achieved when the cord is vibrating at what is known as the fundamental frequency (see fundamental in {numref}`waves_harmonics_illustration`). Adjust the driving amplitude and frequency to obtain a large-amplitude wave that vibrates smoothly. Ensure the cord does not hit the table (***why?***). Check vibration near the vibrating blade. Ideally, the point where the cord attaches should be a node, but you will find that the apparent position of the node is somewhere past where the cord attaches.

11. Determine frequency $f_n \pm \delta f_n$. Slowly lower the frequency. Record $f_{n\text{,min}}$ as the lowest frequency you find while still having a standing wave. Slowly increase the frequency. Record $f_{n\text{,max}}$ as the highest frequency you find while still having a standing wave. Determine the measured frequency as the average of the min and max values $(f_n = (f_{n\text{,max}} + f_{n\text{,min}})/2)$. Determine the frequency's uncertainty as half the range you just found $(\delta f_n = (f_{n\text{,max}} - f_{n\text{,min}})/2)$.

12. Determine the ratio of each frequency to the fundamental frequency, $f_n/f_1$. Does this make sense? What is the expected ratio?

13. While at your determined frequency, measure the distance between nodes (i.e. node-to-furthest-best-node distance) and estimate its uncertainty. Calculate the wavelength $\lambda_n \pm \delta \lambda_n$.
    - For the first harmonic, you need to estimate the position of the node near the vibrating blade.
    - For higher harmonics, you can avoid the node near the blade and focus on the node at the pulley and the node furthest away along the string. *What's your estimated uncertainty in the length measurement; more or less accurate when measuring across single or multiple antinodes?*

14. Calculate the propagation velocity with {eq}`eq-wave-frequency`. Similarly calculate the velocity uncertainty by maximizing and taking the difference $(\delta v_n= (\lambda_n + \delta\lambda_n) (f_n + \delta f_n) - v_n)$. *As you reach higher harmonics for the current case, how do they compare to each other? Do you expect them to be the same or different, why?*

15. Raise the frequency to resonate at the second harmonic. The cord should vibrate with a node at each end and one node in the center (see higher harmonics in {numref}`waves_harmonics_illustration`). Again measure the frequency and the distance between pulley node and furthest-best-node along the string to determine wavelength.

16. Continue repeating the previous measurements for the higher harmonics (list in {numref}`waves-cases-table`).

17. Calculate the average $v$ and average $\delta v$ for the current case. Does it agree with your expected velocity (as calculated from the tension and the linear density in {eq}`eq-wave-velocity`)? If not, what may be contributing to the lack of accuracy?


### ● Graphical Analysis Velocity

18. Plot wavelength $\lambda$ vs. the inverse of the frequency $1/f$ for the current case. As you complete additional cases, add each case to the same single plot (include trendlines like normal) as you go.

19. Use `LINEST(y-values,x-values,TRUE,TRUE)` to calculate the slope and use {eq}`eq-wavelength-inverse-frequency` to determine the slope-derived propagation velocity ($v_\text{slope-derived} \pm \delta v_\text{slope-derived}$). Consider the uncertainty in the slope. Do your plot-derived propagation velocities agree with the expected velocities? Your plot will be represented by the reorganization of {eq}`eq-wave-frequency`:

```{math}
:label: eq-wavelength-inverse-frequency
\lambda = v \frac{1}{f}
```



### ● Continue to Additional Cases

20. CONSIDER: How do you expect tensions and linear densities to affect the wave propagation?

21. Once you are satisfied with your first case, increase the hanging mass to 350 grams and repeat the above procedure for Case II (at {ref}`section-waves-experimental-velocity`).

22. Using a cord with a different linear density, repeat for Case III (at {ref}`section-waves-experimental-velocity`).






## Post-Lab Submission --- Interpretation of Results

### ● Finalized Spreadsheets

  - Make sure to submit your finalized data table (Excel sheet).
  - Please include concise summary table.
  - Please include plot:
    - One plot with all three cases on it with their own trendlines: $\lambda$ vs $1/f$



### ● Post-lab Writeup

- In a **paragraph**, summarize your error analysis. Be quantitative, not only qualitative.
  - What is the precision of your equipment?
  - What are possible sources of systematic (i.e. affecting accuracy) and random (i.e. affecting precision) errors?
  - What are your measurement uncertainties, and, based on these uncertainties, how do your final results change? I.e. do your different measurement and slope uncertainties make your final results larger or smaller, by how much?


- In a **paragraph**, summarize the results you have determined for all cases. Consider:
  - What was the point of today's lab; what did we aim to discover?
  - For each case, do your experimental velocities of propagation (average and slope-derived) agree with your expected velocity from {eq}`eq-wave-velocity`? (be quantitative)
  - How is the velocity of propagation dependent on the tension in the string and density of the cord?
    - When the experiment was done with a lighter weight cord, why would the string vibrator have to be run faster for each measurement condition?
    - Looking at you plot containing all three cases, how are the cases organized? What do you notice about the slopes as you change cases?
  - Do you experimental ratios of $n$-harmonic's frequency to fundamental frequency agree with the expected relationship? Why, physically, do we expect this $f_n/f_1$ relationship?


## The Whiteboard

```{figure} WavesFigures/waves_2025_Spring_01_v02.jpg
:name: waves_whiteboard_01
:width: 100%
:align: center

Overview. Notes. Equation numbers have changed. Using error propagation instead of standard deviation. 3 Cases instead of 4, old case three is dropped.
```

```{figure} WavesFigures/waves_2025_Spring_02_v01.jpg
:name: waves_whiteboard_02
:width: 100%
:align: center

`LINEST()` function.
```
