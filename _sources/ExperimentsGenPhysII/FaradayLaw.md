(faradays-law-induction-overall)=
# 1172L-ONLY | Faraday's Law of Induction


## Background

### ● Background Overview

```{admonition} OVERALL GOALS
:class: note
Use a horseshoe magnet and a swinging coil of wire to:
- Explore magnetic flux, Faraday's Law, Lenz's Law, and mechanical energy dissipation
- Understand the relationship between magnetic flux and electro-motive force (EMF; effectively an induced voltage due to changes in magnetic flux)
```

Today's experiment will cover two main parts. The first will focus on characterizing the magnetic field near the center of a horseshoe magnet for use later. It will continue by determining average voltage and magnetic flux of the induction wand (loops of wire) as it passes through the horseshoe magnet. The second part focuses on characterizing energy lost due to the induced EMF on a closed circuit in addition to frictional effects.

<!--- 

- In this experiment, you will:
  - First determine the maximum magnetic field strength of the horseshoe magnet through where the wand's coil passes.
  - Second determine average voltage and magnetic flux of the wand passing through the magnetic field and compare to expected values of the induced voltage (EMF).
  - Third determine the amount of energy lost due to friction (with angles of the rotary sensor for change in gravitational potential energy), energy lost due to the resistor (area under power curve), and total energy lost (again with angles).

--->


### ● Magnetic Flux

The magnetic field in a volume of space can be described by vectors, which give the strength of the field (its magnitude) and the field's direction at each point of the volume. A closed loop (closed, so that the area of the loop is defined) will then have field vectors "punch through" the area bounded by the loop (see example in {numref}`fig_faraday_01`). 

```{figure} FaradayLawFigures/Figure_01_FluxThroughArea.png
:name: fig_faraday_01
:width: 100%
:align: center

Overview.
```

One can think of this as the field "flowing" through the area defined by the loop (very similar to water flowing through a cross sectional area of a pipe). This flux can be defined by:


```{math}
:label: eq-magnetic-flux
\Phi=\oint \vec{B} \cdot d \vec{A} = \vec{B} \cdot \vec{A} = \vec{B} \vec{A} \cos{\theta} \rightarrow \text{if } \theta=90^{\circ}, \Phi=BA
```

Note that, the right-hand side of the equation holds only if $B$ is constant over the area defined by the loop. The flux will be zero if the magnetic field is parallel to the area of the loop and maximum if the field is perpendicular to the area of the loop.

### ● Faraday's Law

If a loop of wire (for example a coil) is moving into or out of a magnetic field or if the magnetic field over the area of the loop itself changes (either direction or magnitude), then an electro-magnetic force (EMF, essentially induced voltage) might be induced in the loop due to the fact that the magnetic flux through the loop changes. Faraday's Law states that the induced electro-motive force [EMF] or voltage in the loop is directly proportional to the rate of change of the flux through the loop. In this experiment, the magnet and coil are arranged so that the magnetic field is perpendicular to the coil loops and:

```{math}
:label: eq-faraday
\mathcal{E} = \Delta V= -N \frac{d\Phi}{dt}
```

Here $N$ is the number of windings in the coil and the negative sign in front of the expression indicates that the EMF is induced in such a way that it opposes the change in flux through the loop (this direction indication is commonly known as Lenz's Law).

If we were to then integrate {eq}`eq-faraday`, and know for in this lab the area of the coil is constant, but the B-field through the area defined by the coil will change, we would find:

```{math}
:label: eq-faraday-integrated
\int_{\textrm{peak}}\Delta V dt= -N A \Delta B
```

If we were to average over time, we would find the average EMF (again, with unchanging area for today) is:


```{math}
:label: eq-faraday-average
\mathcal{E}_\text{avg} = \frac{1}{\Delta t} \int_{\textrm{peak}}\Delta V dt= -N A \frac{\Delta B}{\Delta t}
```


<!---
```{math}
:label: eq-faraday-dB-dt
\mathcal{E} = \Delta V= -N A \frac{d B}{dt}
```

or, if we average over a time $\Delta t$:

```{math}
:label: eq-faraday-average
\mathcal{E}_\text{avg} = \Delta V_{ave}= -N A \frac{\Delta B}{\Delta t}
```

Integrating {eq}`eq-faraday` gives:

```{math}
:label: eq-faraday-integrated
\int_{\textrm{peak}}\Delta V dt= -N A \Delta B
```
--->


If the area is integrated from the beginning of the peak to the point where the voltage is zero and the coil is at the maximum field, then $\Delta B$ will equal the maximum field. Capstone has an area function ![FaradayArea](../Intro/CapstoneFigures/FigCapstone_012_IntegralAreaTool.png) that can be used to measure the integral of the voltage.

If the coil is in a closed circuit with total resistance $R$ then a current will flow through the coil according to Ohm's Law:

```{math}
:label: eq-ohms-law2
V = I R
```

The circuit will dissipate energy at a rate of:

```{math}
:label: eq-power-dissipation
P= V I= I^{2} R
```

Since power is work per time, the energy that is lost in the circuit can be found by calculating the area under the power vs. time graph (i.e. the integral of the Power $P$ over time $t$):

```{math}
:label: eq-energy-loss
E_{lost}=\int P\, dt= \textrm{Area under the P vs t graph}
```

### ● Energy in a pendulum

The center of mass of a pendulum starting at an initial height $h_{i}$, then swinging through its lowest point and finally rising to a height $h_{f}$, will experience a change in potential energy of:

```{math}
:label: eq-potential-energy-change
\Delta PE= m g (h_{f}-h_{i})
```

If no energy was dissipated, then the change in potential energy would be zero (no potential energy would be lost in this case). If the final height were less, as indicated by the smaller final angle in {numref}`fig-pendulum-energy`, then the change in energy would give the energy lost during the motion:

```{math}
:label: eq-energy-lost-height
E_{lost}=\Delta PE = m g (h_{f}-h_{i})
```

Finally the initial and final heights can be related to the angles $\theta_i$ and $\theta_f$ the pendulum makes with the vertical direction at these location (see {numref}`fig-pendulum-energy`):

```{math}
:label: eq-energy-lost-angle
E_{lost}=\Delta PE = m g\, L(\cos\theta_f-\cos\theta_i)
```

In this equation $L$ indicates the distance from the center of mass to the pivot of the pendulum.

```{figure} FaradayLawFigures/Figure01.jpg
:name: fig-pendulum-energy
:alt: Coil wand swinging from initial angle to final angle showing energy loss
:width: 100%
:align: center

This picture shows the coil wand swinging from an initial angle $\theta_{i}$ to a final angle $\theta_{f}$. The final angle is less because of energy lost in the process, which reduces the potential energy by an amount $E_{Lost}$ (see {eq}`eq-energy-lost-angle`).
```

```{figure} FaradayLawFigures/Figure_80_experimentalequipment.png
:name: fig-experimental-equipment
:alt: Coil wand experimental equipment showing center of mass, resistor, and internal components
:width: 100%
:align: center

Left) Coil wand with resistor and an example of the center of mass line and mass noted on the wand itself. Center) Resistor and circuit diagram of the wand; resistor plugs in and completes the circuit allowing energy to be dissipated. Right) Internals of the wand; wires lead from the ports to the coil at the bottom of the wand. The area of the loop refers to the area inside the white loop of wire at the bottom.
```

### ● Equipment

- Variable Gap Horseshoe Magnet
- Induction Wand as shown in {numref}`fig-experimental-equipment`. The number of turns of the coil is $N=200$ and the area of the coil is $A = \pi r^2 = \pi (0.013\,\text{m})^2$.; mass and center of mass are noted on the white label.
- $\sim 4.7\,\Omega$ resistor (you will measure your resistor directly to confirm later on). It can be inserted into the wand to complete the circuit in the wand in order to measure the energy dissipated in the resistive load by the induced current.
- Stand, rods, and clamps
- Voltage Sensor to Capstone; records the voltage induced in the coil. The plugs of this sensor are connected to the jacks at the end of the coil wand. The voltage sensor is plugged into an analog input with a sample rate set to $1000\,\text{Hz}$.
- PASPORT 2-Axis Magnetic Field Sensor (axial measures positive B-field into the end of the probe; perpendicular measures positive B-field upwards through the probe) for measuring strength of horseshoe magnet.
- Rotary Motion Sensor (RMS) connected to Capstone. Detects and measures angular displacement, angular velocity, and angular acceleration. A 3-step pulley is affixed to its axle (see {numref}`fig-faraday-setup`). The coil wand is mounted onto the 3-step pulley so that the rotational motion of the wand (and therefore the coil) can be measured. The RMS is set to a nominal sample rate of $500\,\text{Hz}$.

<!---
%The experiment consists of a circular coil with 200 windings, which is mounted on a pendulum wand so that it can swing through the (adjustable) gap of a horseshoe magnet (see Fig.~\ref{E8Fig02}). A resistor can be attached to the wand in order to measure the energy dissipated in the resistive load by the induced current.

%The data needed for the analysis is recorded by the Capstone software, which records data collected from three sensors, which are simultaneously plugged into a PASCO 850 Universal Interface connected to the computer:
%\begin{itemize}
%\item The Rotary Motion Sensor (RMS) is able to detect and measure angular displacement, angular velocity, and angular acceleration. It is attached to a vertical rod and has a 3-step pulley affixed to its axle (see Fig.~\ref{E8Fig02}). The coil wand is mounted onto the 3-step pulley so that the rotational motion of the wand (and therefore the coil) can be measured. The RMS is plugged into a PASPORT input with the sample rate set to $1000\,\hertz$.
%\item A Hall effect magnetic field sensor measures the magnetic field between the poles of the horseshoe magnet. 
%\item A voltage sensor records the voltage induced in the coil. The plugs of this sensor are connected to the jacks at the end of the coil wand. The voltage sensor is plugged into an analog input with a sample rate set to $1000\,\hertz$.
%\end{itemize}
%Pictures of the experimental setups are shown below.

--->


## Experimental Procedure


### ● Preview

```{admonition} PROCEDURE OVERVIEW
:class: note
Run Part I for ***both 1.5 cm*** and ***3.0 cm*** magnetic plate spacing.
- Part I.1: Magnetic Field
  - Experimentally determine the maximum magnetic field strength of the horseshoe magnet through where the induction wand's coil passes when swung.
- Part I.2: EMF (Induced Voltage)
  - Experimentally determine average EMF and magnetic flux of a single coil for when the wand swings through the magnetic field; use first peak; compare to expected value.
  - ● PLOT 1 of 2 ●: photo/screenshot of Capstone's Voltage vs. Time and related Angle vs. Time for one full swing (out and back) for just one of the 1.5 cm or 3.0 cm cases.
- Part I.3: Lenz's Law
  - Discuss & consider Lenz's Law: Conceptual analysis for discussion in post-labs based on the existing plots

Run Part II for narrow magnet spacing with magnetic plates **removed**.
  - Part II.1: Energy Conservation by parts
    - Determine total energy loss by measuring change in energy of each individual part of the system
      - Part II.1.A.: Energy lost to just friction using change in gravitational potential energy
        - Use Angle vs. Time plot and swing **without** resistor
      - Part II.1.B.: Energy lost to just circuitry (resistor dissipation)
        - Use area under curve of Power vs. Time and swing **with resistor plugged in** to see amount of energy dissipated as heat by the resistor
        - ● PLOT 2 of 2 ●: photo/screenshot of Capstone's Power vs. Time and related Angle vs. Time for one full swing (out and back).
  - Part II.2 Energy Conservation on the whole
    - Determine total energy loss by measuring change in energy of the whole system
      - Total energy lost (combination of friction and circuitry) using change in gravitational potential energy
        - Use same Angle vs. Time plot from Part II.1.B (**with resistor plugged in**)
  - Compare Part II.1 sum of parts to Part II.2 total energy lost to friction and circuitry (resistor dissipation)
```



### ● Part I: Preliminary Setup
The experiment should be already set up for you as shown in {numref}`fig-faraday-setup`. If not, match the figure to include the magnetic pole plates (CAREFUL WITH FINGERS, ASK FOR ASSISTANCE AS NEEDED).

```{figure} FaradayLawFigures/Figure_05_EMFSetup.png
:name: fig-faraday-setup
:width: 100%
:align: center

Overall experimental setup consisting of induction wand mounted on the RMS as well as the horseshoe magnet. The cables connecting to the voltage sensor are plugged into the two jacks at the top of the wand.
```




#### ○ Part I.1: Magnetic Field


```{figure} FaradayLawFigures/Figure_04_MagneticFieldSensor.png
:name: fig-setup-magnetic-field
:width: 100%
:align: center

How to measure positive magnetic field strength of horseshoe magnet. Use the perpendicular sensor on the PASPORT 2-Axis Magnetic Field Sensor which measures B-field as positive from North to South or out-of-the-page as illustrated on the sensor casing itself in the right-hand side image.
```



1. Set gap between the plates on the magnet to $1.5\,\text{cm}$ (Case 2 will be $3.0\,\text{cm}$).
2. Starting in the first tab in the Capstone file, click Record and use the magnetic field sensor to measure the magnetic field strength between the poles of the magnet. First press the Tare button on the 2 Axis Magnetic Field Sensor with it held far from the magnets. Hold the field sensor sideways (same position as in {numref}`fig-faraday-setup`) and insert the tip into the gap between the poles of the magnet. When the measured field is positive the label of the magnetic field sensor points towards the South pole of the magnet. The magnetic field direction as measured (positive or negative) is as shown in the diagram on the sensor. The field lines coming out of the side of the sensor with the diagram and tare button on it indicate the magnetic field strength as positive, pointing North to South when external to the magnet.
3. Hold the Induction Wand pendulum up out of the way. Insert the Magnetic Field Sensor probe between the magnetic pole plates. If the pole plate on the same side as the label on the magnetic field sensor is a south, the Magnetic Field Sensor signal is positive.
4. Click RECORD. Use the Magnetic Field Sensor to determine which pole plate is north and put a label on it. You will need that for the Lenz's law part of the experiment. If a compass is available, check to make sure you have labeled your magnet correctly.
5. Use the Magnetic Field Sensor to probe the field between the plates. Record the maximum field at the center of the plates.
6. Determine the distance from the horseshoe magnet where the field drops to less than $0.001\,\text{T}$ (essentially zero). You will start the coil wand swinging this far from the magnet so that it begins its swing in approximately zero field. Enter your values in the Magnetic Field Data table.
7. Click STOP.



#### ○ Part I.2: Induced EMF (Voltage)
8. In this section you will compare the calculated and experimental $\mathcal{E}$ (EMF or voltage) induced in the wand's coil.
9. The coil should be able to move freely through the gap between the magnet poles, with the poles as close together as possible (about $1.5\,\text{cm}$ between the plates) without restricting the motion of the coil. The center of the coil should be moving right through the middle of the poles. The long axis of the plates is horizontal so the pendulum swings through a more uniform magnetic field.
10. Switch the Capstone file to the second tab, with Voltage vs. time and angle vs. time plots.
11. Ensure the Voltage Sensor banana plugs are plugged into the banana jacks on the end of the coil wand. Drape the Voltage Sensor wires over the rods so the wires will not exert a torque on the coil as it swings.
12. Let the pendulum hang at rest. Press RECORD, and ZERO the voltage sensor by looking in the bottom recording bar, with the voltage sensor selected, click the zero button (zero with two yellow arrows pointing towards each other).
13. You can now pull the pendulum back. Let the pendulum swing freely and ensure the pendulum can swing 10 oscillations over about 10 seconds. If it's longer, you may have extra friction from the wand hitting/scraping against the magnet or wires. No data is needed for this step, just double check your setup. Once you're sure the pendulum can freely swing, move on to the next step.
14. WITH THE PENDULUM AT REST, click RECORD and pull the coil wand out a bit further than the zero-B-field position you measured in step 2 above ($\sim 25^{\circ}$). Release the wand and let it swing through the magnet out and back once (see {numref}`fig-faraday-EMFExample_withDemo`). Then click STOP. The graph should show at least four pulses similar to {numref}`fig-faraday-EMFExample`.

```{figure} FaradayLawFigures/Figure_05.5_EMFSetupSwingExample.png
:name: fig-faraday-EMFExample_withDemo
:width: 100%
:align: center

Example of releasing the wand and example of just half a cycle the start/stop times and area under the curve for just the first peak.
```

```{figure} FaradayLawFigures/Figure_10_exampleEMF_v02.png
:name: fig-faraday-EMFExample
:width: 100%
:align: center

Example of plots for this part.
```

15. Press the "Stop" button on Capstone.
16. Enlarge the portion of the voltage vs. time graph where the coil passed through the magnet.
17. Enable and use the Multi-coordinates tool ![RCCircuit_multicoordinateTool](../Intro/CapstoneFigures/FigCapstone_001_MultiCoordinateTool_v02.png) to determine the difference in time from the beginning to the end of the first peak.
    - Record initial and final times (see {numref}`fig-faraday-EMFExample_withDemo`).
18. Find the average voltage by highlighting the first peak from when voltage lifts off from zero and returns to zero.
    - Find the experimental area under the curve of the voltage versus time graph for the first peak using the area tool ![FaradayArea](../Intro/CapstoneFigures/FigCapstone_012_IntegralAreaTool.png). 
      - See {numref}`fig-faraday-EMFExample_withDemo` and {numref}`fig-faraday-EMFExample`.
      - *You will have to CHANGE the tool properties number format to show sufficient significant digits.*
    - Calculate your experimental value of the average EMF using your plot-derived values and the left-hand side of {eq}`eq-faraday-average`. (The integral is the area under the curve)
    - Calculate the expected value of the average EMF using the right-hand side of {eq}`eq-faraday-average`.
    - Compare your experimental and expected values with a percent difference (reminder in {ref}`errorAnalysis-percentDiff-experimentalExpected`).
    - Use $N = 200$ for the number of turns of the coil and $A = \pi r^2 = \pi (0.013\,\text{m})^2$ for its area.
19. Find change in Magnetic Flux through ***a single loop***
    - Determine your experimental change in Magnetic flux for a single loop using your average EMF value and {eq}`eq-faraday-average`.
    - Calculate the expected change in magnetic flux for a single loop calling back to {eq}`eq-magnetic-flux`.
    - Compare your experimental and expected values with a percent difference (reminder in {ref}`errorAnalysis-percentDiff-experimentalExpected`).
20. ***PLOT 1 of 2*** --- for just the first case ($1.5\,\text{cm}$): take a photo/screenshot of Capstone's Voltage vs. Time and related Angle vs. Time for one full swing (out and back, example in {numref}`fig-faraday-EMFExample`).
21. Increase the magnet gap to $3.0\,\text{cm}$ and repeat previous steps, still releasing the pendulum from the same position you used before.



#### ○ Part I.3: Lenz's Law
- Think about this section as you will need to cover it in your post-lab submission.
- Look at the circuit diagram showing the coil orientation printed on the Induction Wand (also shown in {numref}`fig-experimental-equipment`). Note that we have connected the red plug from the Voltage Sensor to the upper port and the black plug to the lower port. If coil current flows in the direction shown by the arrows (clockwise), then the upper port becomes positive due to excess positive charge there, and the lower port becomes negative due to decrease in positive charge. Since the red lead from the Voltage Sensor is attached to the upper port, the Voltage Sensor would read a positive voltage. Caution: although current flow in an external circuit is from positive to negative, current flow inside a battery or power supply must be from negative to positive.
- Lenz’s Law states that the current induced in a coil by a changing magnetic field through the coil will flow in a direction to oppose the change which produced it. In particular, the field produced by the induced current will be in a direction to try and prevent the field through the coil from changing.
- The magnetic field points from the north pole to the south pole. As the coil enters the magnet, the magnetic flux increases in that direction. Lenz’s Law says that the induced voltage opposes the change in flux. 

    ```{admonition} Lenz's Law?
    :class: question
    - For the first peak of the Voltage vs. Time plot, since the coil is entering the field, what does Lenz's law say about the induced voltage of the first peak compared to the second peak; should they both be positive or negative, or should one be positive and one be negative?
    - Does it matter which direction the coil is moving or which direction the magnetic field is pointing?
    ```





<!---
```{figure} ExperimentsGenPhysII/FaradayLawFigures/Figure_06_withResistorNoPlates.png
:name: fig-resistor-load
:alt: Resistive load attached to coil wand showing voltage sensor connections
:width: 100%
:align: center

This picture shows the resistive load attached to the coil wand. The cables leading to the voltage sensor are plugged into the resistor. In order to disconnect the resistor without changing the mass-distribution of the coil wand only one of the resistors plugs is connected to the jacks of the wand.
```
--->

### ● Part II: Energy Conservation Preliminary Setup

1. In Capstone, go to the next page. On the left side, click on the calculator.
    - With the coil ***outside*** of the magnetic field, use an ohmmeter to:
      - Measure the resistance of the coil in the induction wand. *Why must the coil be out of the field of the horseshoe magnet when measuring resistance?*
      - Verify the resistance of the $4.7\,\Omega$ resistor. 
    - Enter the accurate resistance values in the calculator and click accept. Finally click the calculator to close it. Before you start any additional trials, click the calculator to make sure the resistor values are correct and have not reverted to the default values.
2. Change the setup to match {numref}`fig-resistor-overall-setup`.
    - Remove the magnet pole plates. (ASK FOR ASSISTANCE AS NEEDED) Move the magnets as close to each other as possible, making sure that you leave enough space for the coil to move through the gap.


```{figure} FaradayLawFigures/Figure_06_withResistorNoPlates.png
:name: fig-resistor-overall-setup
:width: 100%
:align: center

This picture shows the overall setup for the current part. Note: magnetic pole plates are removed and magnet spacing shrunk. Resistive load attached to the coil wand. The cables leading to the voltage sensor are plugged into the resistor.
```

3. Connect the voltage sensor wires with the $4.7\,\Omega$ resistor into the coil wand.
    - Make sure for the first part (friction only), only half of the resistor is plugged so current does not flow, but the weight distribution stays consistent (see {numref}`fig-resistor-overall-setup-unplugged`).


```{figure} FaradayLawFigures/Figure_07_resistorUnplugged_v02small.png
:name: fig-resistor-overall-setup-unplugged
:width: 100%
:align: center

This picture shows the resistor half plugged-in.
```


3. Measure the distance of the center of mass of the wand (marked on the white piece of paper taped to the wand) from the pivot (the screw). Note the result in the data table. (see {numref}`fig-experimental-equipment`)
4. Note the mass of the wand (also noted on the wand) in your data table.



#### ○ Part II.1.A: Energy Lost due to Only Friction

5. First determine the amount of energy lost to friction by letting the pendulum swing through the magnet with the resistor disconnected. Reminder, this is done by having the resistor plugged into the wand with only one of the banana plugs connected (see {numref}`fig-experimental-equipment`). This makes sure that no current flows through the wand (and the resistor) while leaving the center of mass of the wand relatively unchanged.
6. Press the "Record" button on Capstone with the coil **at rest** between the magnet poles. The rotary sensor zeros itself out whenever you start recording, we want to make sure $0°$ is when the wand is at rest inside the magnet.
7. Rotate the wand to an initial angle of $25^{\circ}$ and let it go.
8. Press the "Stop" button after the wand has reached the other side.
9. Zoom in to the portion of the angle vs. time graph where the coil passed through the magnet. Select the peak and get the maximum (initial) and then the minimum (final) angle of the motion to find the initial angle ($\theta_{i}$) and the angle to which the pendulum rises after it has passed once through the magnet ($\theta_{f}$). (see {numref}`fig-faraday-POWERExample`-bottom)


```{figure} FaradayLawFigures/Figure_11_examplePower_v02.png
:name: fig-faraday-POWERExample
:width: 100%
:align: center

Example of plots for this part.
```

10. Calculate the energy lost to friction using {eq}`eq-energy-lost-angle`.

#### ○ Part II.1.B: Energy Lost due to Only Resistor

11. Now connect the resistor by plugging in both plugs into the wand ({numref}`fig-resistor-overall-setup-pluggedin`).

```{figure} FaradayLawFigures/Figure_08_resistorPlugged_v02small.png
:name: fig-resistor-overall-setup-pluggedin
:width: 100%
:align: center

The resistor fully plugged-in.
```

12. Press the "Record" button on Capstone with the coil at rest between the magnet poles.
13. Rotate the wand to an initial angle of $25^{\circ}$ and let it go.
14. Press the "Stop" button after the wand has reached the other side.
15. Detemine energy dissipated by the resistor.
    - Highlight both peaks on the power vs. time plot and find the area under the curve (area tool ![FaradayArea](../Intro/CapstoneFigures/FigCapstone_012_IntegralAreaTool.png)).
    - Right-click the displayed value to set the numeric format and increase sig. figs. Record this area as it equals the the energy dissipated by the resistor as presented in {eq}`eq-energy-loss`.


#### ○ Part II.2: Energy Lost Overall

16. Using the same data run as Part II.1.B, measure the initial angle ($\theta_{i}$) and the angle to which the pendulum rises after it has passed once through the magnet ($\theta_{f}$), but now that the resistor was fully plugged in.
17. ***PLOT 2 of 2*** --- for just when the resistor was plugged in: take a photo/screenshot of Capstone's Voltage vs. Time and related Angle vs. Time for one-half swing (out but not back, example in {numref}`fig-faraday-POWERExample`).
18. Calculate the total energy lost using {eq}`eq-energy-lost-angle`.
19. Compare this total energy lost value (Part II.2) to the sum of the energy lost due to friction (Part II.1.A) and the energy dissipated by the resistor (Part II.1.B).
    - Calculate the percent difference between the two.


### ● Summary & Cleanup

1. Create a summary table of your data (e.g. relevant final result values and percent differences from Part I and Part II).

2. When you are finished, reset your experimental setup before leaving.

    ```{admonition} CLEAN UP
    :class: important
    Please return your experimental station back to the way you found it or better:
     - Reset magnet spacing back to about 1.5 cm with the rectangular plates (CAREFUL WITH YOUR FINGERS...ask for assistance as needed)
     - Remove resistor from wand and store in number tray, reattach voltage sensor cables (red on top banana plug, black on bottom)
     - Close (DO NOT SAVE) Capstone
    ```










## Post-Lab Submission --- Interpretation of Results

### ● Finalized Spreadsheets

  - Make sure to submit your finalized data table (Excel sheet).
  - Please include concise summary table.
  - Please include plots (from Capstone):
    - $V$ vs time and related Angle vs. Time (Part I) for one full cycle or swing out and back
    - $P$ vs time and related Angle vs. Time (Part II) for one-half cycle or swing out (but not back) when resistor is in circuit


### ● Post-lab Writeup

- In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
  - What is the precision of your equipment?
  - What are possible sources of systematic (i.e. affecting accuracy) and random (i.e. affecting precision) errors?
  - What are your measurement uncertainties, and, based on these uncertainties, which impact your final results the most?



- In a **paragraph**, summarize the results you have determined for all cases. Consider:
  - What was the point of today's lab; what did we aim to discover?
  - PART I
    - Do your experimental results for average EMF and change in flux from part 1 agree with the expected values? By how much?
    - What was the induced voltage of the coil of wire swinging into the magnetic field dependent on?
    - Looking at your plot from Capstone of Voltage vs. Time, there should be four spikes in voltage during one whole cycle forward and back.
      - Why are the first and second peaks opposite signs (positive vs. negative, look back on the wand's circuit diagram and think about how current would flow), and how does that relate to Lenz's Law? 
      - Why is the voltage zero as the coil passes through the center of the magnet?
      - Does it matter which direction the coil is moving or which direction the magnetic field is pointing?

  - PART II
    - Do your values for total energy loss (with resistor) agree with the sum of the energy dissipated by the closed circuit (with resistor) plus friction of the rotary sensor (without resistor)?
      - Why would you expect them to agree? Why physically was energy lost?
    - Why, for the Power dissipated vs. Time plot were there two peaks, but now of the same sign (i.e. both positive)?
    - Why, if you used a larger resistor, for example a $10\,\Omega$ resistor in place of the $4.7\,\Omega$ resistor, should the damping of the pendulum would be reduced?



<!---    - The magnetic field points from the north pole to the south pole. As the coil enters the magnet, the magnetic flux increases in that direction. Lenz’s Law says that the induced voltage opposes the change in flux. 
    - For the first peak, as the coil is entering the field, what does Lenz's law say about the induced voltage of the first peak compared to the second peak; should they both be positive or negative, or should one be positive and one be negative?
--->








## The Whiteboard

```{figure} FaradayLawFigures/Faraday_Summer_2025_01_v01.jpg
:name: faraday_whiteboard_01
:width: 100%
:align: center

Old overview, majority still the same, but different induced voltage values to find.
```

```{figure} FaradayLawFigures/Faraday_Spring_2025_02_v01.jpg
:name: faraday_whiteboard_02
:width: 40%
:align: center

Multimeter settings, changing significant figures in Capstone (must be done every new data run).
```

```{figure} FaradayLawFigures/Faraday_Spring_2025_03_v01.jpg
:name: faraday_whiteboard_03
:width: 100%
:align: center

Short notes on the three parts of the lab.
```