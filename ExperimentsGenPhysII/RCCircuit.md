(electrical-example-of-an-exponential-decay-process-overall)=
# Electrical Example of an Exponential Decay Process with Resistors & Capacitors (RC Circuits)


## Background

### Background Overview

```{admonition} OVERALL GOALS
:class: note
Use resistors and capacitors to investigate:
- what a capacitor is
- the relationship between capacitance and resistance
- the discharging nature of capacitors
```

Many physical processes involve a rate of change that is proportional to the magnitude of the quantity itself; the result is an in exponential behavior over time. In this experiment, you will investigate the exponential relaxation (decay) of the voltage or charge on a capacitor.

An electrical analogy of this process is a simple circuit where a capacitor discharges through a resistor connected across its terminals. The schematic for this RC circuit is shown in {numref}`fig-rc-charging-circuit`-right.


```{figure} RCCircuitFigures/E5_Fig_001_v02.png
---
name: fig-rc-charging-circuit
align: center
width: 100%
---
Left) Schematic of circuit charging the capacitor. Right) Schematic of RC circuit disconnected from the battery and discharging through the resistor.
```

With the switch connecting the capacitor to the batteries (see {numref}`fig-rc-charging-circuit`-left), the capacitor rapidly charges up to the potential of the batteries. Since a capacitor will not pass a DC current, a positive charge builds up on one of the plates while a negative charge forms on the other. When the switch is flipped to connect the capacitor to the resistor, we have the circuit (shown in {numref}`fig-rc-charging-circuit`-right) containing a charged capacitor with a resistance across its terminals. 


### Time Dependence of Voltage in a Capacitor


We will now investigate how the voltage across the capacitor changes with time, starting at $t = 0$ when the capacitor is fully charged. The voltage will be measured by the voltmeter $V$ connected as shown in {numref}`fig-rc-charging-circuit`. As time progresses, current will flow from the positively charged plate of the capacitor through the resistance $R$ to the negatively charged plate.


Since a voltage exists across the capacitor, there must also be a voltage across $R$. This implies an electric current, and from Ohm's Law:

```{math}
I=\frac{V}{R}
```

Since current is a flow of charge, $Q$, and since the two sides of the capacitor are isolated from each other, the charge which flows through the resistor must originate on one of the plates and terminate on the other. Thus the flow of current reduces the charge on the capacitor. In a time, $t$, the amount of charge that passes through the resistor is $I \times t$. This must be $-Q$ (the negative change in the charge on the capacitor) which leads to the relation:

```{math}
I=-\frac{dQ}{dt}
```

The value of the resistance limits the amount of current that can flow and thus limits the rate of discharge of the capacitor.

From the definition of a capacitor, we know that the larger the voltage applied to the capacitor, the more charge it will put on the capacitor. Hence, if $V$ is the voltage across the capacitor, then $Q$ is proportional to $V$. The larger the plate area, the more charge it should hold. In addition, if the plates are brought closer together, the positive plate will attract more negative charge from the battery to the negative plate. All these factors have to do with the geometry and construction details of the device. Thus, the bigger the plate area and the smaller the plate spacing, the larger the charge that accumulates in the capacitor for a given voltage. Hence we can write:

```{math}
Q=CV
```

where $C$ is a constant for a given capacitor called its capacitance.

Combining these three equations, we obtain:

```{math}
:label: eq-capacitor-discharge
\frac{{\rm d}Q}{{\rm d}t}=-\frac{Q}{RC}
```

Notice that the **rate of change** of the charge at any time is directly proportional to the amount of charge on the capacitor at that time. (This is similar to the amount of radiation given off by a quantity of decaying atoms.) By writing {eq}`eq-capacitor-discharge` in the form:

```{math}
\frac{{\rm d}Q}{Q}=-\frac{{\rm d}t}{RC}
```

both sides of the equation can be integrated to obtain:

```{math}
\ln(Q)=\frac{1}{RC}+\ln(Q_{0})
```

After some simplification, the solution to this differential equation is:

```{math}
Q=Q_{0}e^{-\frac{t}{RC}}
```

At $t=0$, $V = V_{0}$, so that $Q = CV_{0}$ for $t = 0$. Thus the behavior of $Q$ or $V$ is the same after the switch is opened:

```{math}
:label: eq-voltage-decay
Q=CV e^{-\frac{t}{RC}} \rightarrow V=V_{0}e^{-\frac{t}{RC}}
```

The behavior of the current $I$ is found directly from this:

```{math}
I=-\frac{dQ}{dt}=\frac{V_{0}}{R}e^{-\frac{t}{RC}}
```
The product $RC$ has the units of time (Ω × F); we can verify this by using dimensional analysis:

```{math}
RC\rightarrow \frac{V}{I}\times \frac{Q}{V}\rightarrow \frac{Q}{I}\rightarrow Q\times \frac{t}{Q}\rightarrow t
```

```{math}
[RC]=\Omega \times F\rightarrow \frac{V}{C/s}\times \frac{C}{V}\rightarrow C\times \frac{s}{C}\rightarrow s
```

This product is called the ***time constant*** of the circuit. In a time equal to $RC$, the voltage, $V$, drops to a fraction:

```{math}
:label: eq-time-constant-fraction
\frac{V}{V_{0}}=\frac{1}{e} \approx 0.368
```

This means that in any interval of time equal to $RC$, the voltage has decreased to 36.8% of the initial value. In determining $RC$, it is often more convenient to measure the time for the voltage to drop to $\frac{1}{2}$ of its initial value and from this to compute $RC$. The ***"half-life"*** $t_{1/2}$ is given by:

```{math}
\frac{V_{1/2}}{V_{0}}=\frac{1}{2}=e^{-\frac{t_{1/2}}{RC}}
```

Taking the natural logarithm of both sides and simplifying we obtain:

```{math}
:label: eq-half-life
t_{1/2}=RC \ln 2 \simeq 0.693 RC
```

or

```{math}
:label: eq-rc-from-half-life
\boxed{
RC=1.443 t_{1/2}
}
```

Note that by taking the natural log of the expression for the voltage, {eq}`eq-voltage-decay`, we obtain:

```{math}
\ln V=\ln V_{0}-\frac{t}{RC}
```

in the form of $y=mx+b$,

```{math}
:label: eq-linear-voltage-decay
\boxed{
\ln V=-(\frac{1}{RC})t+\ln V_{0}
}
```

If we **plot** the value of the natural log of $V$ as a function of time, $t$, we obtain a straight line whose slope is $-1/RC$ with an intercept of $\ln V_{0}$. From this slope, we can obtain a measured value for the product $RC$ which is the time constant, i.e. the time it takes the voltage (or charge) to decay to $1/e$ of its original value (see {eq}`eq-time-constant-fraction`).

### Dividing charge across capacitors

A capacitor $C$ at voltage $V$ holds a charge $Q = CV$. In the circuit shown in {numref}`fig-cc-charging-circuit` when the single-pole-double-throw (SPDT) switch connects the first capacitor ($C_\text{first}$) to the voltage source, it holds a charge $Q_\text{first} = C_\text{first} V$. The switch is then flipped to disconnect the first capacitor from the battery and connect it to the second capacitor ($C_\text{second}$). Charge moves from the lower capacitor to the upper capacitor, lowering the voltage and sharing the charge. Assuming the upper ($C_\text{second}$) capacitor is initially uncharged, the total charge is unchanged. The **total charge $Q$ must then be divided between the two capacitors so that they come to the same lower final voltage**:

```{math}
:label: eq-charge-division
V_f C_\text{first} &= Q_\text{first} \\
V_f C_\text{second} &= Q_\text{second} \\
Q_\text{first}+Q_\text{second} &= Q = C_\text{first} V \\
V_f &= \frac{C_\text{first}}{C_\text{first}+C_\text{second}} V
```

Because the two capacitors are at the same voltage, the total charge is divided between them in proportion to their capacitance.



```{figure} RCCircuitFigures/E5_Fig_001-5_v02.png
---
name: fig-cc-charging-circuit
align: center
width: 100%
---
Left) Schematic of circuit charging the capacitor. Right) Schematic of CC circuit disconnected from the battery and discharging to a separate capacitor.
```






### Equipment

The general setup with electrical schematic can be seen in {numref}`fig-rc-setup`, with the voltmeter attached on either side of the capacitor section of the circuit. Capacitors to be determine, resistors to be treated as known, and wire and jumper bars are shown in {numref}`fig-rc-setup_capacitors_resistors`.


<!---
- Two *known* (with ohmmeter) ceramic/metal-film resistors ($R_{1\text{,brown}}$, $R_{2\text{,blue}}$)
- Two to-be-determined capacitors ($C_{1\text{,big}}$, $C_{2\text{,small}}$)
- Pasco modular circuit kit
  - 4× Corner module
  - 1× T-junction module
  - 1× Straight-line module
  - 2× AA battery module
  - 3× Spring clip modules (to attach individual resistors, capacitors, jumper bar)
  - 1× Single-pole double-throw (SPDT) switch module to open and close circuit during charging of capacitors, and discharging of capacitors through resistors
  - 13× U-shaped jumper clips to connect the different modules
- Voltmeter via Capstone -- connected to the jumper clips the on either side of the capacitors with alligator clips
- Fluke multimeter with alligator clips
  - Use as Ohmmeter (Ω) to measure resistors' resistance to be treated as known values
  - Use as capacitance meter (F) to measure capacitors' actual capacitance to compare experimental values to later on
--->


```{table} Equipment
:name: rc-equipment-table

| Category | Items |
|----------|-------|
| **Resistors** | • 2× *known* ceramic/metal-film resistors: $R_{1\text{,brown}}$, $R_{2\text{,blue}}$ (measured with ohmmeter) |
| **Capacitors** | • 2× unknown capacitors: $C_{1\text{,big}}$, $C_{2\text{,small}}$ |
| **PASCO Modular Circuit Kit** | • 4× corner modules <br> • 1× T-junction module <br> • 1× straight-line module <br> • 2× AA battery modules <br> • 3× spring clip modules (attach resistors, capacitors, jumper bar) <br> • 1× SPDT switch module (change circuits to charge / discharge capacitors <br> • 13× U-shaped jumper clips |
| **Measurement Device ("actual")** | • Fluke multimeter with alligator clips (for "actual" values) <br> • Ω: measure resistor values (treated as known) <br> • F: measure "actual" capacitor values for later experimental comparison |
| **Experimental Voltage Measurement** | • Capstone voltmeter (Connected across capacitors using alligator clips on jumper bars) |
```


```{figure} RCCircuitFigures/E5_Fig_002_setup_v02.png
---
name: fig-rc-setup
align: center
width: 100%
---
Left) Schematic, with circuit modules with spring modules for connecting capacitors, resistors, jumper bars. Right) Example of actual setup with voltmeter (used in Capstone) is connected across the eventual locations of the capacitor(s).
```

```{figure} RCCircuitFigures/E5_Fig_003_RCWires_v01.png
---
name: fig-rc-setup_capacitors_resistors
align: center
width: 50%
---
Example of capacitors, resistors, and wire and jumper bar to be used.
```




## Experimental Procedure

- Assume **we know the resistance** of your resistors, but **we don't know the capacitance** of the capacitors, and we need to determine those C values
- *DISCUSSION POINT*: How do different RC (resistor-capacitor) combinations affect the change of their circuits' voltages over time?
- Conduct two experiments:
  - Measure the capacitance of your capacitors, $C_1$, $C_2$, and $(C_1+C_2)$
    - **GRAPHICALLY** with LN(V) vs. Time plot (a linearized version of exponential decay plot)
    - Via the **HALF-LIFE, $t_{1/2}$** (where half-life, the time for exponential decay to reach half its original value, is related to the natural log of 2 [LN(2)])
  - Divide charge between two capacitors


**FIRST EXPERIMENT** We study resistor-capacitor circuits and how capacitors discharge.

1. You have two resistors and two capacitors. Create a common data table and measure the value of resistors $R_1$ and $R_2$ with the Fluke multimeter set to measure ohms (Ω, note the units on the multimeter). [It doesn't matter which resistor is which number, just be consistent] Also in the common data table, record the actual capacitance of $C_1$, $C_2$, and the parallel combination of $(C_1+C_2)$ with the Fluke 175 multimeter when set to measure farads (the yellow alternate function of the ohmmeter, looks like two letter T's that are rotated toward each other).

2. Use the capacitors with individual resistors. Perform the following steps for the following pairs of resistor and capacitor cases:
    - $R_1+C_1$
    - $R_2+C_1$
    - $R_1+C_2$
    - $R_1+(C_1+C_2)$ in parallel
    - $R_1+(C_1+C_2)$ in series

3. **Zero the voltage sensor** (this is before any resistors or capacitors are in the circuit). Connect the voltmeter to the Capstone program via the PASCO 850 Universal Interface. Set the sample rate to 2500 samples per second (should be set by default, double check though). Zero the voltage sensor in Capstone by first opening the single-pole-double-throw (SPDT) switch to ensure no current is flowing; then in the bottom recording bar, with the voltage sensor selected, click the zero button (zero with two yellow arrows pointing towards each other).

4. In Capstone (should be already set up), you should have graphs of the voltage versus time, the Natural Log(V) vs. time, and a running table of voltages and times (this table is connected to the V vs. T plot, so if you highlight data points on the plot, they'll be highlighted in the table).


5. Connect the resistor, capacitor(s), switch, batteries, voltmeter as shown in {numref}`fig-rc-decay-circuit`. Also see {numref}`fig-rc-decay-circuit_parallel_series` for the cases involving capacitors in parallel and series.



```{figure} RCCircuitFigures/E5_Fig_004_Example_v03.png
---
name: fig-rc-decay-circuit
align: center
width: 100%
---
Modular electronic RC circuit. The resistors and capacitors will just be placed in the spring modules to become part of the circuits. Left) Example with capacitor being charged. Right) Example with capacitor discharging through resistor.
```

```{figure} RCCircuitFigures/E5_Fig_005_parallel_series_v03.png
---
name: fig-rc-decay-circuit_parallel_series
align: center
width: 85%
---
Left) Parallel capacitors and Right) Series capacitors in spring modules.
```


6. Create a data table for the first resistor and capacitor case (once you have this all set up, you'll then be able to just copy and paste this data table for the five other RC combinations):

   - With **five columns** (1 for each of the 5 decay trials, the act of discharging each capacitor). Also include a **column** for the average values, a **column** for the standard deviation (σ), and a **column** for the standard error of the mean ($\frac{\sigma}{\sqrt{n-1}}$ where $n=$ number of trials. Reminder, this is effectively your +/- uncertainty of the average. *DISCUSSION POINT for later*: How well does your average value of capacitance +/- standard error agree with your expected values?).

   - Include **three rows** for:
     - Slope. You will get this from the linear fit of the natural log(V) vs. time plot (linearizing the exponential decay) in Capstone where the fit will be in the form $y=mt + b$, and slope $m=\frac{-1}{RC}$
     - Time constant $(RC)$ of the exponential decay as determined from the slope
     - Capacitance ($C_{\text{graphically from decay}}$) as determined from the decay time constant

   - Include an additional **six rows** for:
     - Initial voltage ($V_{\text{init}}$, right ***after*** decay starts)
     - Final voltage ($V_{\text{final}} = V_{\text{init}}/2$, i.e. voltage that is half the value of the initial voltage)
     - Initial time ($t_{\text{init}}$, when $V=V_{\text{init}}$). Found either with the Capstone table or the individual data point selection tools
     - Final time ($t_{\text{final}}$, when $V=V_{\text{final}}$). Found in a similar way in Capstone, just at half the voltage
     - Half-life ($t_{1/2}= t_{\text{final}}-t_{\text{init}}$)
     - Capacitance ($C_{\text{by half-life}}$) as determined by the rearrangement of {eq}`eq-rc-from-half-life` (the characteristic of the half-life of an exponential decay)




7. **DATA TAKING:**

   - Start recording; flip the SPDT switch to connect the batteries to the capacitor and observe the voltmeter as the capacitor rapidly charges to $V_\text{init}$. Once the capacitor is fully charged (voltmeter shows constant voltage at $V_\text{init}$), flip the switch to connect the capacitor to the resistor; observe the decay of the voltage across the capacitor. **Wait until the voltage drops to less than** 10% of $V_\text{init}$. (e.g. if $V_\text{init}=3.0$ V, then $V_\text{10-percent}= 0.3$ V) In essence, the battery has been eliminated from the circuit and the capacitor is now acting as the voltage source.

   - WHILE STILL RECORDING: (so everything is just in the same plot, save some time) Repeat this switch flipping **four more times** for a total of **5 decays**.

   - GRAPHICAL: In the Capstone plot of LN(Voltage) vs. Time, highlight the data of the linear portion of the decay curve with the highlighter tool and record the slope. The linear section covers the time it took voltage to decay from 100% to 10% of $V_\text{init}$. The linear fit, as described in {eq}`eq-linear-voltage-decay`, in Capstone should be in the form $y=mt + b$, where $m=\frac{-1}{RC}$. Calculate the time constant $RC$, and the capacitance $C_\text{graphically from decay}$ as determined from that time constant.

   - HALF-LIFE: Find the voltage and time of when your capacitor was at its initial voltage right before decay. Divide the $V_\text{init}$ by 2 to find the final voltage; then find the time for that final voltage. Determine half-life from the time difference ($t_{1/2}= t_\text{final}-t_\text{init}$). *Suggestions on finding those values*: Examine the exponential decay plot (V vs. T) with the crosshair tool by zooming in to find the data points right before the voltage decay, clicking the data point and selecting the crosshair, then note the time and voltage. Alternatively, in the exponential decay plot (V vs. T), zoom in to the area right before decay and use the data highlight tool to make a small selection box which will then also highlight those same data points in the Capstone table of voltages and times.

8. For your capacitance that you determined ***graphically*** from the LN(V) vs. time slope, calculate the average, standard deviation, and standard error of the mean. For your capacitance that you determined with the ***half-life*** $t_{1/2}$ (time span for initial voltage to halve), determine the standard deviation (σ) and standard error of the mean ($\frac{\sigma}{\sqrt{n-1}}$).




***DATA TAKING:***
 - Start recording; flip the SPDT switch to connect the batteries to the capacitor and observe the voltmeter as the capacitor rapidly charges to $V_\text{init}$. Once the capacitor is fully charged (voltmeter shows constant voltage at $V_\text{init}$), flip the switch to connect the capacitor to the resistor; observe the decay of the voltage across the capacitor. **Wait until the voltage drops to less than** $10\%~\text{of}\,V_\text{init}$. (e.g. if $V_\text{init}=3.0\,\text{V}$, then $V_\text{10-percent}= 0.3\,\text{V}$) In essence, the battery has been eliminated from the circuit and the capacitor is now acting as the voltage source. 
  - WHILE STILL RECORDING: (so everything is just in the same plot, save some time) Repeat this switch flipping **four more times** for a total of **5 decays**.
  - GRAPHICAL: In the Capstone plot of LN(Voltage) vs. Time, highlight the data of the linear portion of the decay curve with the highlighter tool and record the slope. The linear section covers the time it took voltage to decay from 100\% to 10\% of $V_\text{init}$. The linear fit, as described in {eq}`eq-linear-voltage-decay`, in Capstone should be in the form $y=mt + b$, where $m=\frac{-1}{RC}$. Calculate the time constant $RC$, and the capacitance $C_\text{graphically from decay}$ as determined from that time constant.


```{figure} RCCircuitFigures/E5_Fig_015_GraphicalExample_v02.png
---
name: FigE5_015_graphical
align: center
width: 80%
---
Example Voltage vs. Time plot (top) and LN(V) vs. Time plot (bottom). Left) Time of start of a decay trial. Lower bound of data-highlight box for fitting data in LN(V) vs. Time plot. Right) Time of the effective end of a decay trial when voltage drops to 10% of initial voltage (i.e. when $V = V_\text{10-percent}$ and upper bound of data-highlight box.)
```


  - HALF-LIFE: Find the voltage and time of when your capacitor was at its initial voltage right before decay. Divide the $V_\text{init}$ by 2 to find the final voltage; then find the time for that final voltage. Determine half-life from the time difference ($t_{1/2}= t_\text{final}-t_\text{init}$). \textit{Suggestions on finding those values}: Examine the exponential decay plot (V vs. T) with the crosshair tool by zooming in to find the data points right before the voltage decay, clicking the data point and selecting the crosshair, then note the time and voltage. Alternatively, in the exponential decay plot (V vs. T), zoom in to the area right before decay and use the data highlight tool to make a small selection box which will then also highlight those same data points in the Capstone table of voltages and times.



```{figure} RCCircuitFigures/E5_Fig_014_HalfLifeExample_v01.png
---
name: FigE5_014_halflife
align: center
width: 80%
---
Example Voltage vs. Time plot (top) and LN(V) vs. Time plot (bottom). Left) Time of start of a decay trial. Center) Time when half of the initial voltage is reached (i.e. after a half-life or $t_1/2$). Right) Time of the effective end of a decay trial when voltage drops to 10% of initial voltage (i.e. when $V = V_\text{10-percent}$.)
```




<!---    %\item Then repeat this step **four more times** for a total of **five time trials**.




  %  \item Using those time values, calculate $\Delta t$ for each trial's voltages. For your $\Delta t$ values at each target voltage, calculate their average (mean) values.

--->

   - For your capacitance that you determined ***graphically*** from the LN(V) vs. time slope, calculate the average, standard deviation, and standard error of the mean.
   - For your capacitance that you determined with the ***half-life*** $t_{1/2}$ (time span for initial voltage to halve), determine the standard deviation ($\sigma$) and standard error of the mean ($\frac{\sigma}{\sqrt{n-1}}$).

%\item  In a separate location on your data sheet, calculate the average capacitance from your half-life and resistor values with Eqn.~\ref{E4Eq:HalfLife} and determine its standard deviation and standard error of the mean.

9. Compare this value for capacitance to the actual capacitance values of the capacitors, $C_1$, $C_2$, and $(C_1+C_2)$ you measured with the multimeter in Step 2.

10. Replace the resistor and/or capacitor for the next combination and repeat the procedure (from Step 7) above for each of the six combinations listed in Step 2.

**DISCUSSION POINT**: How do different RC (resistor-capacitor) combinations affect the change of their circuits' voltages over time (i.e. decay)?

**DISCUSSION POINT**: How well does your average value of capacitance +/- standard error agree with your expected values? Why or why not? What are possible sources of uncertainty or systematic bias that could cause your values to agree/not agree with your expected values that you had found with the multimeter?

---

**SECOND EXPERIMENT** We study dividing charge across two capacitors, as in {numref}`fig-capacitor-charge-division`.


```{figure} RCCircuitFigures/E5_Fig_006_CC_Example_v04.png
---
name: fig-capacitor-charge-division
align: center
width: 100%
---
Modular electronic circuit with two capacitors. Left) Example with lower capacitor being charged by batteries. Right) Example with lower capacitor discharging to the upper capacitor.
```

1. Ignore what you've called the capacitors from the first experiment, now just consider them as either low- or high-capacitance capacitors in either the $C_1$ or $C_2$ positions. Construct the circuit shown in {numref}`fig-capacitor-charge-division` by replacing the resistor with the high-capacitance capacitor (in the top springs block, e.g. $C_2$ position in {numref}`fig-capacitor-charge-division`). Put the low-capacitance capacitor in the bottom springs block ($C_1$ position in {numref}`fig-capacitor-charge-division`). Ensure the voltmeter is connected as in {numref}`fig-capacitor-charge-division` and continue using the same Voltage vs. time plot in Capstone.

2. Create a data table including your previous, experimentally-determined values of capacitance of $C_1$ and $C_2$ and **three columns** for initial and final voltages as well as the difference between the two. Create **five rows** for five trials. Note: Initial voltage is V when the battery is connected to $C_1$ *before* you throw the switch to connect the capacitors together in Step 5. Final voltage is V *after* you throw the switch to allow the charge in the first capacitors to be distributed between the two capacitors.

3. Temporarily connect a wire across each capacitor to discharge them before flipping the switch (i.e. no charge is stored and both circuits are open).

4. Connect $C_1$ to the battery using the single-pole-double-throw (SPDT) switch. Record the initial voltage.

5. Flip the SPDT switch to disconnect $C_1$ from the battery and connect it to $C_2$. Flip the switch back and forth quickly **for a total of five trials**. Record the final voltage after the charge is distributed between the capacitors (near immediate change).

6. Notice how the final voltage is drifting up towards the initial voltage and the difference between the two is changing. Something is wrong with the assumptions built into {eq}`eq-charge-division` (which should be true). The problem is that after the first time throwing the switch, $C_2$ is not at zero charge. So the total charge is higher than $C_1 V$. *Challenge: Can you figure out what the voltage will be after the second, third, or $n$th time you flip the switch?*

7. Try temporarily connecting a wire across $C_2$ to discharge it before flipping the switch. Now you should consistently get the final voltage predicted by {eq}`eq-charge-division`. Record the initial and final voltages after doing this **five more times**. Does this voltage difference agree with {eq}`eq-charge-division`?

8. Repeat from step 4 with the low- and high-capacitance capacitors in swapped positions in the circuit.











## Post-Lab Submission --- Interpretation of Results

### Finalized Spreadsheets

  - Make sure to submit your finalized data table (Excel sheet).
  - Please include concise summary table.
  - Please include an example of the relevant plot(s) for
    - First Experiment
    - Second Experiment


### Post-lab Writeup

- In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
  - What is the precision of your equipment?
  - What are possible sources of systematic (i.e. affecting accuracy) and random (i.e. affecting variance) errors? How would they change your final results (larger, smaller, more varied)?
  - For this exercise, assume voltage uncertainty of $0.01\text{V}$ and time uncertainty of $0.01\text{sec}$. Based on these uncertainties, how do your final results (for just the first case) change? (I.e. larger or smaller?)
    - If larger or smaller, are they more or less accurate to expected values?
    - Which, voltage or time in this case, presents a larger effect on final results?

- In a **paragraph**, summarize the results you have determined for all cases. Consider:
  - What was the point of today's lab; what did we aim to discover?
  - First Experiment:
    - For each case, using standard deviation as our uncertainty for this lab, do your experimental results for average capacitance agree with your expected values (as measured with the multimeter)?
    - Of the two (graphical and half-life), which method's results could we be more confident in and why?
    - How do different RC (resistor-capacitor) combinations affect the change of their circuits' voltages over time (i.e. decay)? Remember, you had five cases of various combinations:
      - How did an increase of resistance affect the decay (shorter/longer)? Physically why?
      - How did an increase of capacitance affect the decay (shorter/longer)? Physically why?
      - How did capacitors in parallel and series each affect the decay (shorter/longer)? Physically why?
  - Second Experiment
    - How does the difference in voltage (final - initial) change after each switch back and forth when using $C_{2\text{,small}}$ to charge up $C_{1\text{,big}}$?
      - What would be the same or different with the capacitors swapped (with $C_{1\text{,big}}$ charging up $C_{2\text{,small}}$)?
    - Explain why, in step 3 of the second experiment you connect a wire across each capacitor. Why is a brief connection sufficient? *Hint: What is the time constant for the wire and capacitor; how is it different to the resistor and capacitor setup?*
      - How does the difference in voltage change when the second capacitor is connected with a wire?





<!--- replace results question with something more meaningful?

  - Is the graphical or half-life method more accurate to the expected values; why?

--->


%OLD Version !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! before 11/6/2024
%\begin{enumerate}
%\item Comment on the relative precision of the two measurements (half-Life and slope).
%\item Some current flows through a voltmeter when it is measuring a voltage. If the resistance of the voltmeter is $2\,\mega\ohm$ then how would it affect the experiment?
%\item The capacitor used in this experiment has a relatively high value of capacitance. What would happen if you replaced it with a $1000\,\pico\farad$ capacitor?
%\end{enumerate}
% end file E4Decay.tex



## The Whiteboard

```{figure} RCCircuitFigures/RCCircuits_2025_Summer_01_v02.jpg
:name: RCCircuits_whiteboard_01
:width: 100%
:align: center

Overview 1st part.
```

```{figure} RCCircuitFigures/RCCircuits_2025_Summer_02_v02.jpg
:name: RCCircuits_whiteboard_02
:width: 80%
:align: center

Overview 2nd part.
```

```{figure} RCCircuitFigures/RCCircuits_2025_Summer_03_v02.jpg
:name: RCCircuits_whiteboard_03
:width: 80%
:align: center

Multimeter settings; Capstone significant figures notes.
```