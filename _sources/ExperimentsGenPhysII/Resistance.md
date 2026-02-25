(resistivity-resistors-dc-circuits-overall)=
# Resistivity with Resistors & DC Circuits



## Background


### Background Overview --- Resistance

```{admonition} OVERALL GOALS
:class: note
Use resistors and a light bulb to investigate:
  - The relationship between resistance, voltage, and current within a circuit.
  - Ohm's Law.
```


If a potential difference $V$ is applied across some element in an electrical circuit, the current $I$ in the element is determined by a quantity known as the resistance $R$. The relationship between these three quantities serves as a definition of the quantity resistance $R$:

```{math}
:label: eq-ohms-law
R=\frac{V}{I}
```

An object that is a pure resistor has its total electrical characteristics determined by {eq}`eq-ohms-law`. Other circuit elements may have other important electrical characteristics in addition to resistance, such as capacitance or inductance. The resistance of any circuit element, whether it has other significant electrical properties or not, is given by the ratio of voltage to current as described in {eq}`eq-ohms-law`. For any given circuit element, the value of this ratio may change as the voltage and current changes. Nevertheless, the ratio of $V$ to $I$ defines the resistance of the circuit element at that particular voltage and current. The unit of resistance is the volt/ampere defined as the ohm, denoted by the symbol "$\Omega$."

Certain circuit elements obey a relation that is known as ***Ohm's Law***. For these elements, the ratio of $V$ to $I$ (i.e. $R$) is a ***constant*** for different values of $V$. Therefore, in order to show that a circuit element obeys Ohm's Law, it is necessary to vary the voltage (the current will then also vary) and observe that the ratio $V/I$ is in fact *constant*. In today's experiment, such measurements will be performed on two different types of elements to determine their resistance response to voltage (ceramic/metal-film resistors and an incandescent light bulb).

The resistance of any object to electrical current is a function of the material from which it is constructed, as well as the length, cross-sectional area, and temperature of the object. At constant temperature, the resistance $R$ of a sample with a constant cross-section $A$, and length $L$ is given by

```{math}
  R=\rho  \frac{L}{A},
```

where $\rho$ is a material constant called the resistivity. Normally $\rho$ is dependent upon the temperature of the sample; depending upon the material, $\rho$ may either increase or decrease with increasing temperature. Thus, if the current is sufficient, the *heating of the material by the current passing through it can change the resistance.*

Consider a "black box" with some unknown circuit inside connected to two terminals on the box. If we apply a voltage $V$ to the terminals and observe a current $I$ flowing through the "black box," we define the resistance of the "black box" to be $R = V/I$. If the resistance of the circuit element is a constant independent of both the current and the voltage, then we say that the circuit element is ohmic and that it follows Ohm's law. Georg Simon Ohm found that most pure metals at room temperature have this property. However, a light bulb has a tungsten filament that heats up as you increase the current through it. Since the resistance of tungsten increases with temperature, the resistance of the tungsten filament increases as the voltage increases. Therefore a light bulb does not follow Ohm's law.

For an ohmic resistor, when a voltage $V$ is applied, then the current is $I = V/R$, so the current is proportional to the voltage. If you plot voltage vs. current, the result is a straight line whose slope is the resistance. For a non-ohmic element like a light bulb, a plot of voltage vs. current is curved.

### Series & Parallel Circuits

```{figure} ResistanceFigures/Figure01_v02.jpg
---
name: fig-series-parallel-resistors
align: center
width: 80%
---
Resistors connected in Series (top) and Parallel (bottom).
```



Series and parallel connections for three resistors ($R_1$, $R_2$, $R_3$) are illustrated in {numref}`fig-series-parallel-resistors`. 

The **equivalent resistance** $R_{\text{eq}}$ for each of these networks is that resistance which can replace the network of resistors between the terminals of the network. $R_{\text{eq}}$ for each is given by:

```{math}
:label: eq-equivalent-resistance
\text{Series} \rightarrow R_{\text{eq}} &= R_1 + R_2 + R_3 + \ldots + R_n \\
\text{Parallel} \rightarrow \frac{1}{R_{\text{eq}}} &= \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3} + \ldots + \frac{1}{R_n}
```

<!---
Notice that if a voltage is applied across the terminals of a **series circuit**, the current that flows is the same in all elements and the sum of the voltage across each element is equal to the total applied voltage. The relationship of the voltages is a statement of conservation of energy and is known as **Kirchhoff's Voltage Rule** (a.k.a. **Loop Rule**). It is more commonly stated as "The algebraic sum of the voltage changes around any closed loop is zero."

If a voltage is applied across the terminals of a **parallel circuit**, the voltage is the same across all the elements and the total current flowing into or out of the circuit is the sum of the currents through each of the elements. The relationship of the currents is a statement of conservation of charge and is known as **Kirchhoff's Current Rule** (a.k.a. **Junction Rule**). It is more commonly stated as "The sum of currents into a junction = the sum of currents out of the junction."

Kirchhoff's Rules can be used to completely analyze a complex network of circuit elements. Their application will provide the necessary equations to calculate the current through and the voltage across all the elements of a circuit.
--->



#### Series Circuits --- Kirchhoff’s Voltage Rule

Notice, in a *series circuit*, if voltage is applied, the **current** flows the same through every element. The sum of the voltage drops across the elements equals the applied voltage. This follows from conservation of energy and is expressed by **Kirchhoff’s Voltage Rule (a.k.a. Loop Rule)**:

> The algebraic sum of the voltage changes around any closed loop is zero.

In this experiment, you will primarily verify that the measured voltage drops across series elements add up to the total applied voltage, and secondarily confirm current is consistent through each element.


#### Parallel Circuits --- Kirchhoff’s Current Rule

In a *parallel circuit*, if a voltage is applied, the **voltage** across each branch of the circuit is the same. The total current flowing into or out of a junction equals the sum of the currents through each branch. This follows from conservation of charge and is expressed by **Kirchhoff’s Current Rule (a.k.a. Junction Rule)**:

> The sum of currents into a junction equals the sum of currents out of the junction.

In this experiment, you will primarily verify that the measured branch currents add to the total circuit current, and secondarily confirm voltage drops across each element is consistent.


Kirchhoff’s Rules above provide the equations needed to determine unknown currents and voltages in complex circuits. In this lab, you will apply these rules to analyze series and parallel resistor networks.


<!---
```{figure} ResistanceFigures/2025_E4_SetupOhmsLaw_v02.png
---
name: fig-ohms-law-setup
align: center
width: 700px
---
Schematic and example of setup for testing Ohm's law.
```
--->




### Equipment

Overall setup shown in {numref}`fig-ohms-law-setup`, with a full equipment list in the following table {numref}`resistance-equipment-table_3`.

<!---
- Low-voltage DC Power supplied by PASCO 850 Univeral Interface (using just ~0 -- 6 V) (Capstone example {numref}`E4Fig_05`)
- Resistors (see {numref}`E4Fig_01`):
  - 3x - unlabeled ceramic/metal-film resistors (each < 1 MΩ, colored blue, gray, brown)
  - 1x - Light bulb **(DO NOT EXCEED 6 V)**
- 9x jumper bars used to connect different sections of circuit modules (see {numref}`E4Fig_01`)
- Pasco modular circuit kit:
  - 1x Light bulb module
  - 12x Spring clips modules (to attach individual resistors, voltmeter, ammeter and to create series and parallel circuits)
  - 1x Single-pole single-throw (SPST) switch module to open and close circuit during reconfiguration and calibration
  - 1x Red/black terminal module (for connection to DC power supply)
  - 11x T-junction modules
  - 5x straight line modules
  - 4x blank modules
  - 34x U-shaped jumper clips to connect the different modules
- Fluke multimeter with alligator clips (example connections in {numref}`E4Fig_04`)
  - First:
      - Used as Ohmmeter (Ω) to measure resistors' and light bulb resistances ({numref}`E4Fig_03` left)
      - Also used as DC Voltmeter (V) to measure voltage drop across different circuit elements ({numref}`E4Fig_03` right)
  - Second:
      - Used as DC ammeter to measure current through resitors, light bulb, and resistors in series and parallel circuits ({numref}`E4Fig_03` center)

--->

<!---
```{table} Equipment
:name: resistance-equipment-table

| Category                      | Item                                                 | Notes / Reference                                                    |
| ----------------------------- | ---------------------------------------------------- | -------------------------------------------------------------------- |
| **Power Supply**              | Low-voltage DC power (PASCO 850 Universal Interface) | ~0–6 V output (Capstone example {numref}`E4Fig_05`)                |
| **Resistors**                 | 3× unlabeled ceramic/metal-film resistors            | Each < 1 MΩ; colors: blue, gray, brown ({numref}`E4Fig_01`)          |
|                               | 1× light bulb                                        | **DO NOT EXCEED 6 V**  ({numref}`E4Fig_01`)                          |
| **Connections**               | 9× jumper bars                                       | Connect sections of circuit modules ({numref}`E4Fig_01`)             |
| **PASCO Modular Circuit Kit** | 1× light bulb module                                 |                                                                      |
|                               | 12× spring clip modules                              | For attaching resistors, voltmeter, ammeter, and creating series & parallel circuits        |
|                               | 1× SPST switch module                                | Open/close overall circuit during reconfiguration                    |
|                               | 1× red/black terminal module                         | Connect to DC power supply                                           |
|                               | 11× T-junction modules                               |                                                                      |
|                               | 5× straight-line modules                             |                                                                      |
|                               | 4× blank modules                                     |                                                                      |
|                               | 34× U-shaped jumper clips                            | Electrically connect different modules                               |
| **Measurement Device**        | Fluke multimeter with alligator clips                | Example connections to circuit in {numref}`E4Fig_04`                 |
|                               | Used as Ohmmeter (Ω)                                 | Measure resistors' & bulb resistances ({numref}`E4Fig_03` left)      |
|                               | Used as Voltmeter (V)                                | Measure voltage drop across circuit elements ({numref}`E4Fig_03` right)     |
|                               | Used as DC Ammeter                                   | Measure current through resistors & bulb and series & parallel circuits ({numref}`E4Fig_03` center) |
```

```{table} Equipment
:name: resistance-equipment-table_2

| Category | Items | Notes / Reference |
|----------|-------|------------------|
| **Power Supply** | PASCO 850 Universal Interface (0–6 V DC) | Capstone example {numref}`E4Fig_05` |
| **Resistors** | 3× ceramic/metal-film resistors (<1 MΩ; blue, gray, brown); 1× light bulb | **Do not exceed 6 V** ({numref}`E4Fig_01`) |
| **Connections** | 9× jumper bars | Used to connect circuit sections ({numref}`E4Fig_01`) |
| **PASCO Modular Kit** | 1× bulb module; 12× spring clip modules; 1× SPST switch (open/close); 1× red/black terminal module (to DC power); 11× T-junctions; 5× straight modules; 4× blank modules; 34× U-shaped jumper clips | Build single resistor circuits & series/parallel circuits; connect components |
| **Measurement Device** | Fluke multimeter (with alligator clips): Ω (resistance), DC V (voltage), DC A (current) | Example connections {numref}`E4Fig_04`; meter use shown in {numref}`E4Fig_03` |
```
--->


```{table} Equipment
:name: resistance-equipment-table_3

| Category | Items |
|----------|-------|
| **Power Supply** | • PASCO 850 Universal Interface (~0–6 V DC)  <br> • Capstone example {numref}`E4Fig_05` |
| **Resistors** | • 3× ceramic/metal-film resistors (< 1 MΩ; blue, gray, brown) ({numref}`E4Fig_01`) <br> • 1× light bulb — **DO NOT EXCEED 6 V** ({numref}`E4Fig_01`) |
| **Connections** | • 9× jumper bars ({numref}`E4Fig_01`) |
| **PASCO Modular Circuit Kit** | • 1× light bulb module <br> • 12× spring clip modules (attach resistors, voltmeter, ammeter; build series/parallel circuits) <br> • 1× SPST switch module (open/close circuit) <br> • 1× red/black terminal module (connect to DC supply) <br> • 11× T-junction modules <br> • 5× straight-line modules <br> • 4× blank modules <br> • 34× U-shaped jumper clips |
| **Measurement Device** | • Fluke multimeter with alligator clips ({numref}`E4Fig_04`) <br> • Ω: measure resistor & bulb resistance ({numref}`E4Fig_03` left) <br> • DC V: measure voltage drop across circuit elements ({numref}`E4Fig_03` right) <br> • DC A: measure current through resistors & bulb and series & parallel circuits ({numref}`E4Fig_03` center) |
```


<!---
  - 1× Wireless Current Sensor (Ammeter) -- connected to Capstone software
  - 1× Voltmeter via Capstone -- connected to the jumper clips the on either side of the resistors with alligator clips
  - Seven wires with alligator clips (multi-colored)
--->



```{figure} ResistanceFigures/E-4_Fig_02_OverallSchematic_01.png
---
width: 100%
name: fig-ohms-law-setup
---
Left) Schematic, with example circuit for $R_1$ and ammeter in series and voltmeter in parallel connections with $R_1$. Right) Example of actual setup. Red jumper bars show all locations that can be changed to create different circuit configurations. Light bulb and resistor locations are shown for easy testing. Power is supplied by the black and red banana plug output from the Pasco 850 (controlled in Capstone). SPST switch can be used to open/close entire system.
```



```{figure} ResistanceFigures/E-4_Fig_01_resistors_v03.png
---
width: 100%
name: E4Fig_01
---
Examples of the resistors, light bulb, and jumper bar you will use today.
```


```{figure} ResistanceFigures/E-4_Fig_03_voltmeters.png
---
width: 100%
name: E4Fig_03
---
Examples of the measurement type, connections used, and multimeter overall configurations in use today. Left) configuration for measuring resistance in ohms (Ω) --- note, this auto-ranges, double check the magnitude of your units (e.g. Ω, kΩ, MΩ). Center) configuration for measuring DC current in milliamps (mA) through the 300 mA fused circuit. Right) configuration for measuring DC voltage in volts (V).
```

```{figure} ResistanceFigures/E-4_Fig_04_voltAmpConnection.png
---
width: 100%
name: E4Fig_04
---
Examples how to connect ammeter (in line or in series with resistor) and voltmeter (across or in parallel with resistor) alligator clips to the spring modules. For the light bulb, connect voltmeter to the U-shaped module clips.
```

```{figure} ResistanceFigures/E-4_Fig_05_PascoUse.png
---
width: 100%
name: E4Fig_05
---
Example of Hardware Setup, selecting Output Voltage-Current Sensor, and Signal Generator tabs in Capstone set to DC waveform, control output voltage with "DC Voltage", Voltage limit of $6\,\text{V}$, Current limit of $1.50\,\text{A}$, use On/Off buttons to supply power.
```


## Experimental Procedure
### Procedure Preview

```{admonition} OVERVIEW
:class: note
Conduct three experiments involving:

 - 4 cases: circuits with individual resistors and light bulb
 - 1 case: three resistors in series
 - 1 case: three resistors in parallel

You will apply a range of voltages through the circuits and measure both current and voltage across the resistors (ceramic/metal-film) and light bulb individually and compare your experimental resistances to the "actual" resistance as measured with the ohmmeter. You will then apply a constant $4.00\,\text{V}$ to the circuit with all three resistors in either series or parallel configurations and again measure both current and voltage across each resistor, calculate equivalent resistances, conduct error propagation, and compare to the expected values.
```

<!---
```{admonition} Additional Tips
:class: tip
sdfasdf
```
--->





### Preliminary Setup


1. Create a common data table of your resistors' resistances in Ohms ($\Omega$) where $R_1=\text{blue}$, $R_2=\text{gray}$, $R_3=\text{brown}$, and $R_\text{bulb}=\text{light bulb}$.

2. Measure and record to the common data table the actual resistances of each ceramic/metal-film resistor and light bulb as $R_{1\text{-actual}}$, $R_{2\text{-actual}}$, $R_{3\text{-actual}}$, $R_{\text{bulb-actual}}$. 
    - Take such measurements with the Fluke ohmmeter (setting as shown in {numref}`E4Fig_03` left). You will compare your experimentally determined values to these later on.
    - To measure their resistance, you can either attach the alligator clips directly to the ends of the resistors and light bulb, ***OR*** more preferrably to decrease wear and tear, place the resistors in the spring modules as you will in the next step (example shown in {numref}`E4Fig_01`), and connect the alligator clips to the springs or U-shaped clips as shown for the voltmeter connections in {numref}`E4Fig_04`. This second method is preferred as it is generally easier to deal with, especially for the light bulb. *NOTE: ensure no jumper bars are installed if measuring the resistances when resistors are installed in the modular circuit springs as it may include other elements of the circuitry than just the resistor in question.*

3. Also record an uncertainty in your actual values $\delta R_\text{-actual}$ for each resistor and light bulb in the common data table. (hint: how are you measuring, where would the uncertainty come from for this measurement?)

4. Prepare your experimental set up to match the example {numref}`fig-ohms-law-setup`, with light bulb, $R_1=\text{blue}$, $R_2=\text{gray}$, and $R_3=\text{brown}$ in their respective positions. Attach the resistors by gently sliding the wire leads into the springs of the spring modules as shown in {numref}`E4Fig_01`. Connect the banana-plug wires if not already connected from the DC power output as supplied by the Pasco 850 interface to the red/black terminal module. Install jumper bars into the spring modules as needed to create a closed circuit. For $R_1$, it will be the same as what is shown in the schematic of {numref}`fig-ohms-law-setup`.



```{admonition} Consistent Descriptions
:class: tip
Throughout the following experiments, ensure you are descriptive and consistent in your spreadsheet for each resistor to help keep track of everything.
```

### Part I -- Individual Resistors across Voltage Range


```{admonition} Part I Overview
:class: note
4 cases: circuits with individual resistors and light bulb. You will apply a range of voltages through the circuits and measure both current and voltage across the resistors (ceramic/metal-film) and light bulb individually and compare your experimental resistances to the "actual" resistance as measured with the ohmmeter.
```

5. Trace the circuit from start to finish to ensure the circuit is completed for $R_1$. Start from the red (positive) terminal to of the red/black terminal module through to the ammeter, the resistor, ensuring SPST switch is closed, and end back at the black (negative) terminal. Add jumper bars as needed. Ensure ammeter and voltmeter are connected to measure current through and voltage drop across the resistor ({numref}`E4Fig_04`). (small note: no jumper bar needed for ammeter connections as we want the current to flow through the ammeter, not bypass it)

6. For the first resistor case, create a data table with columns for the following list (but not limited to; add columns as needed for unit conversion to SI units) and include enough rows for each trial/target voltage:
    - Trial number
    - Target voltage: increments you set in the Capstone power supply
    - Measured voltage: voltage drop across circuit element in question
    - Measured voltage uncertainty
    - Measured current: current flowing through circuit element in question
    - Measured current uncertainty
    - Resistance: resistance as calculated with Ohm's law
    - Additional areas for `LINEST()` calculations later on.

7. Target voltages will be $0.10, 0.50, 1.00, ...0.50\,\text{V increments}... 6.00\text{V}$. The first trial is the odd one out since we want a near-zero value, but cannot actually be at zero volts.

8. In Capstone, go to Signal Generator ({numref}`E4Fig_05` right) and ensure it is set to DC waveform. Control the *target* output voltage with "DC Voltage", ensure voltage is limited to a max of $6\,\text{V}$, ensure current is limited to $1.50\,\text{A}$, and use On/Off buttons to supply power. 

9. Set the target voltage to the first target voltage $0.10\,\text{V}$ as listed earlier. Turn ***ON*** the power supply. In Capstone, in place of the normal `Record` button is the `Monitor` button at the bottom of the screen. Press `Monitor` and you should see the output voltage and output current constantly updating. These will purely be used for monitoring output of the power supply, but not for any explicit measurements. Notes: If they are not updating, check that the Hardware Setup (see {numref}`E4Fig_05` left) is set for the Output Voltage-Current Sensor. If the monitored output voltage in Capstone does not agree with what you set in the signal generator, the Output Voltage-Current Sensor may just need to be zeroed out --- turn off power supply, ensure sensor is selected in bottom of screen, press the button to the right that has a 0 with two yellow arrows pointing to the zero line, then check by turning on the power supply, and check calibration is now accurate.

10. Measure and record the DC current $I$ through and the DC voltage $V$ across the resistor (multimeters connected as in {numref}`E4Fig_04`).

11. Increase the power supply output to the next target voltage of $0.50\,\text{V}$. Measure and record current and voltage again with the multimeters, and continue increasing target voltages in $0.50\,\text{V}$ increments until $6.00\,\text{V}$. *Do not frustrate yourself* by trying to get the multimeter-measured voltages to exactly 0.50 V steps --- just set the target voltage record whatever the voltage and current are. The point here is to have a good sampling across a wide range of voltages.

12. For each trial, calculate the resistance by:

```{math}
R_\text{trial#} = \frac{V_\text{trial#}}{I_\text{trial#}}
```

<!---
13. After running all target voltage trials, add a row below to calculate the average and standard deviation of your resistance values.
--->

13. After running all target voltage trials for the current case, determine your overall $R_{1\,\text{experimental}}\pm \delta R_{1\,\text{experimental}}$ by using the `LINEST`($\hat{Y}$,$\hat{X}$,TRUE,TRUE) function to determine the linear relationship between Voltage (as Y-values) and Current (as X-values).

    ```{admonition} Slope Is ...?
    :class: question
    If you were to rearrange {eq}`eq-ohms-law` to be in the linear form of $y=mx+b$, what does the slope $m$ end up representing? When creating your summary table later, ensure you reference the `LINEST` slope's cell and it's uncertainty (remember not to just copy/paste) and accurately describe what it represents, not just described as slope.
    ```

14. Calculate the **difference** between your experimental resistance value (as determined in previous step) and actual values (i.e. $R_\text{experimental} - R_\text{actual}$). Also calculate the **percent difference** between your experimental and actual values (reminder of this in {eq}`eq-percentChangeinErrorAnalysis`). (Generally should be $<10\%$)

15. ***PLOT*** the voltage ($y$) vs. current ($x$) for all cases all on the same plot, starting with this first one ($R_1$). Add the other cases ($R_2$, $R_3$, and light bulb) as you return to this step later. This will be similar to how you plotted both cases on the same plot in last week's lab. For each case, add a linear trendline. For the light bulb case, also add a quadratic or polynomial-to-the-order-of-2 trendline for direct comparison to linear (i.e. light bulb case will have two trendlines on the same data set). In your lab submission, consider the four datasets including the significance of the shape and the slopes.

16. Repeat the preceding steps for resistors $R_2$, $R_3$, and the light bulb. Add/remove jumper bars to create the new circuits. **LIGHT BULB**: Please don't over-volt the bulbs, otherwise they'll burn out sooner, maximum value of $V = 6.00\,\text{V}$.


### Part II -- Resistors in Series at Constant Voltage

```{admonition} Part II Overview
:class: note
1 case: three resistors in series. You will apply a constant $4.00\,\text{V}$ to the circuit with all three resistors in series configuration and again measure both current and voltage across each resistor, calculate equivalent resistances, conduct error propagation, and compare to the expected values.
```

17. Create a new data table including rows for each resistor, columns for:
    - measured voltage
    - uncertainty in measured voltage
    - measured current
    - uncertainty in measured current
    - resistance from {eq}`eq-ohms-law`

18. Include additional areas for:
    - calculated experimental equivalent resistance, $R_\text{eq-series-experimental}$
    - maximized experimental equivalent resistance
    - uncertainty in experimental equivalent resistance ($\delta\,\text{value}=$ difference between maximized and calculated $R_\text{eq-series-experimental}$)
    - expected equivalent resistance from "actual" resistance values, $R_\text{eq-series-actual}$
    - maximized expected equivalent resistance from "actual" resistance values
    - uncertainty in expected equivalent resistance from "actual" resistance values ($\delta\,\text{value}=$ difference between maximized and calculated $R_\text{eq-series-actual}$)

19. Reconfigure the jumper bars to create a series connection of $R_1$, $R_2$, and $R_3$ (see {numref}`fig-series-parallel-resistors` top).

20. Set the power supply target voltage to $4.00\,\text{V}$.

21. Record the current (in series with the circuit) and the voltage (parallel to each resistor) for each of the three resistors with the Fluke multimeter (set to DC amperage and DC voltage, respectively). Note uncertainties. Check that your individual resistances make sense when calculated from {eq}`eq-ohms-law`.

22. Determine the total series experimental equivalent resistance:

```{math}
R_{\text{eq-series-experimental}} = \frac{V_1}{I_1} + \frac{V_2}{I_2} + \frac{V_3}{I_3}
```

23. Calculate the expected equivalent resistance from "actual" resistance values from the Ohmmeter and {eq}`eq-equivalent-resistance`.

24. Maximize both your experimental and expected equivalent resistances. Reminder: both your experimental and expected values should have an uncertainty range since they are both based on measured values (be it voltage, current, or resistance with the multimeters).

    ```{admonition} Maximizing?
    :class: question
    To maximize $R_\text{eq-series}$:
      - should you increase or decrease voltage;
      - should you increase or decrease current;
      - should you increase or decrease resistance?
    Working this out on paper can be a useful exercise (calculations still need to be done in Excel)
    ```

25. For equivalent resistance, determine both experimental and expected uncertainty ($\delta$) ranges by using the difference between maximized and normally calculated equivalent resistances.

26. Compare your experimental $R_\text{eq-series-experimental} \pm \delta R_\text{eq-series-experimental}$ with your expected $R_\text{eq-series-actual} \pm \delta R_\text{eq-series-actual}$. Agree/disagree; why/why not? If due to something fixable, re-take necessary measurements.

### Part III -- Resistors in Parallel at Constant Voltage

```{admonition} Part III Overview
:class: note
1 case: three resistors in parallel. You will apply a constant $4.00\,\text{V}$ to the circuit with all three resistors in parallel configuration and again measure both current and voltage across each resistor, calculate equivalent resistances, conduct error propagation, and compare to the expected values.
```

27. Create a new data table including rows for each resistor, columns for:
    - measured voltage
    - uncertainty in measured voltage
    - measured current
    - uncertainty in measured current
    - resistance from {eq}`eq-ohms-law`

28. Include additional areas for:
    - calculated experimental equivalent resistance, $R_\text{eq-parallel-experimental}$
    - maximized experimental equivalent resistance
    - uncertainty in experimental equivalent resistance ($\delta\,\text{value}=$ difference between maximized and calculated $R_\text{eq-parallel-experimental}$)
    - expected equivalent resistance from "actual" resistance values, $R_\text{eq-parallel-actual}$
    - maximized expected equivalent resistance from "actual" resistance values
    - uncertainty in expected equivalent resistance from "actual" resistance values ($\delta\,\text{value}=$ difference between maximized and calculated $R_\text{eq-parallel-actual}$)

29. Reconfigure the jumper bars to create a parallel connection of $R_1$, $R_2$, and $R_3$ (see {numref}`fig-series-parallel-resistors` bottom).

30. Set the power supply target voltage to $4.00\,\text{V}$.

31. Record the current (in series with the circuit) and the voltage (parallel to each resistor) for each of the three resistors with the Fluke multimeter (set to DC amperage and DC voltage, respectively). Note uncertainties. Check that your individual resistances make sense when calculated from {eq}`eq-ohms-law`.

32. Determine the total parallel experimental equivalent resistance:

```{math}
\frac{1}{R_{\text{eq-parallel-experiment}}} = \frac{I_1}{V_1} + \frac{I_2}{V_2} + \frac{I_3}{V_3}
```

33. Calculate the expected equivalent resistance from "actual" resistance values from the Ohmmeter and {eq}`eq-equivalent-resistance`.

34. Maximize both your experimental and expected equivalent resistances. Reminder: both your experimental and expected values should have an uncertainty range since they are both based on measured values (be it voltage, current, or resistance with the multimeters).

    ```{admonition} Maximizing?
    :class: question
    To maximize $R_\text{eq-parallel}$:
      - should you increase or decrease voltage;
      - should you increase or decrease current;
      - should you increase or decrease resistance?
    Working this out on paper can be a useful exercise (calculations still need to be done in Excel)
    ```

35. For equivalent resistance, determine both experimental and expected uncertainty ($\delta$) ranges by using the difference between maximized and normally calculated equivalent resistances.

36. Compare your experimental $R_\text{eq-parallel-experimental} \pm \delta R_\text{eq-parallel-experimental}$ with your expected $R_\text{eq-parallel-actual} \pm \delta R_\text{eq-parallel-actual}$. Agree/disagree; why/why not? If due to something fixable, re-take necessary measurements.



37. Create a concise summary table summarizing all three parts of today's lab.
    - Part I including for each resistor/light bulb:
      - Experimentally slope-derived resistance
      - Experimentally slope-derived resistance uncertainty
      - Difference between experimental and actual values
      - Percent difference between experimental and actual values
    - Part II including:
      - $R_\text{eq-series-experimental} \pm \delta R_\text{eq-series-experimental}$
      - $R_\text{eq-series-actual} \pm \delta R_\text{eq-series-actual}$
    - Part III including:
      - $R_\text{eq-parallel-experimental} \pm \delta R_\text{eq-parallel-experimental}$
      - $R_\text{eq-parallel-actual} \pm \delta R_\text{eq-parallel-actual}$


38. When you are finished with all experiments, reset your experimental setup before leaving.

    ```{admonition} CLEAN UP
    :class: important
    Please return your experimental station back to the way you found it or better:
     - Return resistors and jumper bars back to containers
     - Power supply is off/Capstone closed
     - Multimeters off
    ```




## Post-Lab Submission --- Interpretation of Results

### Finalized Spreadsheets

  - Make sure to submit your finalized data table (Excel sheet).
  - Please include concise summary table.
  - Please include the relevant plot(s) including (just one for this lab):
    - $V$ vs. $I$, with all three resistors and the light bulb all plotted on the same graph. Linear trendlines for all cases, plus additional quadratic trendline for the light bulb.


### Post-lab Writeup

- In a **paragraph**, summarize your error analysis. Be qualitative, not only quantitative.
  - What is the precision of your equipment?
  - What are possible sources of systematic (i.e. affecting accuracy) and random (i.e. affecting precision) errors? How would they change your final results (larger, smaller, more varied)?
  - What are your measured uncertainties for Voltage and Current; how did you estimate these? Based on these uncertainties, how do your final results change --- test it --- go back and ***make a copy of your spreadsheet to test***:
    - For just the largest-resistance resistor (likely blue):
      - How does your final resistance value change due to increasing/decreasing just voltage by your voltage uncertainty?
      - How does your final resistance value change due to increasing/decreasing just current by your current uncertainty?
      - Which has a bigger overall impact and why?
    - For each of the Series and Parallel circuits:
      - How did your final equivalent resistance results change (larger/smaller?) based on increasing/decreasing your voltage and current uncertainties?
      - Which has a bigger overall impact and why?
      - What was the overall uncertainty range of your equivalent resistances due to error propagation of both voltage and current at the same time?
    - For the resistor, series, and parallel, if your final results became larger or smaller, were they more or less accurate to expected values? 

<!---    - How does this inform whether systematic or random errors. Did anything stand out as a causing less accuracy or less precision?
--->

<!---
  - How could you improve your random errors?
  - Were your systematic errors significant; how could this be improved if you were to re-run this experiment?
--->



- In a **paragraph**, summarize the results you have determined for all cases. Consider:
  - What was the point of today's lab; what did we aim to discover?
  - Do your experimental results for the individual resistors and the light bulb agree with your expected values (as measured with the ohmmeter)? Why or why not? (reminder, since both the actual and experimental values were measured or derived from measured values, you should have both an actual and experimental uncertainty range for comparisons)
    - Do your percent differences make sense? What do they represent?
  - What do the shapes of the resistors and light bulb plotted data mean (linear or non-linear relationship?); why, from a physical standpoint, does the light bulb plot look the way it does as compared to the resistors?
  - Do your experimental results for the equivalent resistances $R_{\text{eq}}$ {eq}`eq-equivalent-resistance` of both series and parallel circuits agree with their respective expected values based on the expected equivalent resistance from the resistors' actual values (from Ohmmeter)?
    - Physically, why should we expect the resistance of a series circuit to be greater than that of a parallel circuit made of the same resistors? (It can sometimes be useful to incorporate analogies to help explain this).




<!---


%OLD Version !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! before 11/6/2024
%\begin{enumerate}
%\item How are the $V$ vs $I$ graphs different for the light bulb and the ohmic resistance?
%\item Does the series connection increase or decrease the resistance? What about the parallel connection?
%\item Why are you connecting a voltmeter in parallel and the ammeter in series? How can they affect your measurement?
%\item Why does a voltmeter have high resistance and an ammeter have low resistance?
%\end{enumerate}

--->


## The Whiteboard

```{figure} ResistanceFigures/DCResistors_2025_Summer_01_v02.jpg
:name: DCResistors_whiteboard_01
:width: 100%
:align: center

Overview for both main parts of the lab. `LINEST()` function (use `Y,X,True,True`).
```


<!---
```{figure} ResistanceFigures/DCResistors_2025_Spring_02_v02.jpg
:name: DCResistors_whiteboard_02
:width: 100%
:align: center

Sensor setup notes.
```

```{figure} ResistanceFigures/DCResistors_2025_Spring_03_v01.jpg
:name: DCResistors_whiteboard_03
:width: 100%
:align: center

WARNING --- MUST HAVE RESISTOR IN SERIES WITH AMMETER TO AVOID DAMAGE. Data taking notes; multimeter settings.
```
--->