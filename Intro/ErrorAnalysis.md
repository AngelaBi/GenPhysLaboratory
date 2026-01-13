(error-analysis-overall-section)=
# Error Analysis Review

In laboratory work, it is usually necessary to use experimental apparatus to measure physical quantities. The measurements are seldom, if ever, perfect. As a result, imperfections must be taken into account in any set of physical measurements. One of the most important things to be learned in the laboratory is how to make reliable estimates of the uncertainties involved in any physical measurements and how to handle the propagation of these errors, i.e., to know how the uncertainties affect calculated results of an experiment.

---

(error-analysis-sigFig)=
## Significant Figures

The number of digits required to express the result of an experimental measurement, so that it reflects the accuracy with which the measurement was made, are known as **significant figures**. Thus, the number of significant figures reflects the limitation of the measuring device and/or the experimenter. Whether the calculations are performed by hand or on a computer, the number of significant figures displayed in the final result must reflect the limitations of the experimental measurement. Often, a computer program will, by default, display either too many or too few digits. If too few digits are displayed, you need to adjust the program setting to show more digits.

For example, if the length of a cylinder is measured as $20.64\,\text{cm}$, this quantity is said to be measured to four significant figures. If written as $0.0002064\,\text{km}$, we still have only four significant figures. The zeros preceding the “2” are used only to indicate the position of the decimal point. The zero between the “2” and the “6” is a significant figure, but the other zeros are not. If the above measurement is made with a meter stick, the last digit recorded is an estimated figure representing a fractional part of a millimeter division. All recorded data should include the last estimated figure in the result, even though it may be zero. If this measurement had appeared to be exactly $20$, it should have been recorded as $20.00\,\text{cm}$, since lengths can be estimated by means of this instrument to about $0.01\,\text{cm}$. When the measurement is written as $20\,\text{cm}$ it indicates that the value is known to be somewhere between $19.5\,\text{cm}$ and $20.5\,\text{cm}$, whereas the value $20.00\,\text{cm}$ indicates a range between $19.995\,\text{cm}$ and $20.005\,\text{cm}$. Conversely, retaining too many significant figures implies greater accuracy than the figures actually represent.

### Rules for Significant Figures

When deciding the number of significant figures to retain, the following rules apply:

- When collecting data, only one estimated figure is retained as a significant figure.
- In addition and subtraction, do not carry the result beyond the first column that contains an estimated figure. All figures lying to the right of the last column in which all figures are significant should be dropped.
- In multiplication and division, the result should have as many significant figures as the factor with the least number of significant figures.
- When dropping figures that are not significant, round to the nearest significant digit. That is to say, the last figure should be unchanged if the first figure dropped is less than 5.  The last figure retained should be increased by one if the first figure dropped is 5 or greater.
- While performing intermediate calculations, it is safer to carry more significant figures than is required in the final result. You can always fix it when you're done.

### Examples --- Addition \& Multiplication

The following examples help illustrate these rules.

#### Addition

When adding these four numbers:

```text
  427.5
   28.03
    0.0654
  396.0
  ------
  851.6
```

the result is rounded to the first decimal digit \(851.6\) because the first term \(427.5\) in the sum is only given to one decimal digit. The sum is expressed to the proper number of significant figures.

#### Multiplication


In our next example, we will calculate the area of a rectangle. If its length is measured as $1.94\,\text{cm}$ and width as $1.84\,\text{cm}$, the area as provided by a calculator is

$$
A = 1.94 \times 1.84 = 3.5696\,\text{cm}^2.
$$

Since each factor has three significant figures (as opposed to the five from the calculator), the result should instead be reported as

$$
A = 3.57\,\text{cm}^2.
$$

```{admonition} Number format in Excel
:class: tip
In Excel, the number of significant figures can be controlled by formatting the cell to a *Number* type with the desired number of decimal places. In addition to being more meaningful, formatting the cells makes the spreadsheet more readable.
```


---

(error-analysis-ErrorProc)=
## Error Analysis Procedure

This section is a guid to performing error analysis for an experiment. Steps for performing error analysis are:

- Identify the likely sources of measurement error.
  - Possible sources --- Instrumentation, experimental setup, procedure
  - Determine/explain whether errors are systematic or random (see {ref}`error-analysis-TypesErrors`).

- Estimate the magnitude of measurement errors using:
  - Equipment specifications
  - Significant digits displayed
  - Your estimate of how accurately you can read the instrument
  - The range or standard deviation of repeated measurements (see {ref}`error-analysis-TypesErrors`).

- Calculate the magnitude of the expected error in calculated quantities due to measurement errors (see {ref}`error-analysis-ErrorPropagation`).

- If the *difference* between **your experimental results** and the **expected results/accepted values** is much *larger* than the expected error, check for:
  - Experimental procedure mistakes
  - Calculation or unit conversion errors
  - Incorrect use of degrees vs. radians
  - Underestimated measurement error
  - Incorrect constants or other common values

- Report results with the correct number of significant figures ({ref}`error-analysis-sigFig`) and the calculated error, otherwise noted as the range or experimental value $\pm$ uncertainty.

---

(error-analysis-TypesErrors)=
## Types of Errors

Experimental measurements are characterized by **precision** and **accuracy**.

- A set of measurements is *precise* if the measurements are closely clustered. (e.g. {numref}`ErrorAnalysis_Fig01`-left)
- A set of measurements is *accurate* if the average value is close to the expected value. (e.g. {numref}`ErrorAnalysis_Fig01`-center)
- A set of measurements is both *accurate* and *precise* if the measurements are closely clustered close to the expected value. (e.g. {numref}`ErrorAnalysis_Fig01`-right)


**Random errors** increase scatter and reduce precision. They arise from uncontrollable variations and inherent limitations of the equipment; they can be estimated and reduced by repeated measurements. **Systematic errors** arise from calibration issues or faulty methods; they can reduce precision and cannot themselves be reduced by repeated measurements. Often you can estimate precision errors by considering the equipment and its specifications.

---


```{figure} IntroductionFigures/ErrorType_v4.png
:name: ErrorAnalysis_Fig01
:width: 100%
:align: center

The distinction between precision and accuracy.
```

(error-analysis-ErrorPropagation)=
## Error Propagation of Measurement Uncertainties

Error analysis can help you recognize if your results are consistent with a *known* or *expected* value. Each measurement has some combination of systematic and random errors. 

 - Make your best estimate of the measurement uncertainty for *each measured value*
    - For direct measurements, think about how confident you are in your measured value. How much could you increase or decrease the measurement tool while still being confident this uncertainty range is still representative of your measurement.
        - E.g. using a triple-beam balance, you measure $432.2\,\text{grams}$, but the level line still appears level when you push the slider to $432.5\,\text{grams}$, your value $\pm$ measurement uncertainty range could be $432.2\,\pm\,0.3\,\text{grams}$.
    - Your estimate may include instrument limitations and variation of measurements over multiple trials. Calculate the differences between your experimental results and any known values. 
 - Recalculate experimental results using maximum and minimum values to determine the expected range of outcomes. Complete this in your spreadsheet by changing your measurements by adding or subtracting the estimated errors. Observe the range of experimental values (maximum and minimum) that you find in these recalculations. If the expected values fall too far outside this range, there is some problem which you need to address.


### Example: Error Propagation --- Density of a Block

Suppose you are measuring the density of a rectangular block. The block has dimensions length $L$, width $W$, height $H$, mass $M$ each with their respective measurement uncertainty. The calculated density is mass divided by volume.


Given

* $L = 2.00\,\text{cm}$, $W = 3.00\,\text{cm}$, $H = 5.00\,\text{cm}$
* $M = 60.00\,\text{g}$
* Uncertainty in length: $\delta L = \delta W = \delta H = \pm 0.01\,\text{cm}$
* Uncertainty in mass: $\delta M = \pm 0.05\,\text{g}$

The experimental density is

$$
\rho_\text{experimental} = \frac{M}{V} = \frac{M}{LWH} = \frac{60.00}{30.00} = 2.00\,\text{g/cm}^3.
$$

To find the max/min range, the maximum density consistent with your measurements is the ratio of the maximum mass and the minimum volume: 

$$
\rho_{\max} = \frac{M+\delta m}{V-\delta V} = \frac{M+\delta m}{(L-\delta L)(W-\delta L)(H-\delta L)} = \frac{60.05}{1.99\times0.99\times4.99} = \frac{60.05}{29.69} = 2.02\,\text{g/cm}^3,
$$

and similarly, the minimum density is $1.98\,\text{g/cm}^3$. If the expected value lies outside this range, further investigation is required. If the expected density is not in this range, you need to consider possible explanations:
 - Errors in the measurements could be larger than you estimated
 - Actual density could be different from the expected value
 - Your calculation may be wrong
 - Perhaps the shape is not exactly rectangular


The two types of errors illustrated in {numref}`ErrorAnalysis_Fig01` require different treatment. The systematic errors illustrated on the target labelled **Precise** cannot be reduced by taking more measurements, while the average value obtained with the random errors on the target labelled **Accurate** *improves* with more measurements. The following sections provide guidance on analyzing systematic and random errors.


---




(error-analysis-RandomErrors)=
## Random Errors

Random errors are inherent in nearly all measurements. They arise because of uncontrollable conditions affecting the observer, the measuring device, and the quantity to be measured. On the basis of probability, these errors are as likely to be positive as negative, and more likely to be small than large. 

Independent repeated measurements and use of their average in any calculation reduce their effect. This minimization is only achieved if the measurements are independent. A common mistake is biasing a new measurement to agree with the previous measurements. This mistake makes the measurements more precise, but less accurate as shown in {numref}`ErrorAnalysis_Fig01`. **Taking truly independent measurements** is the best way to reduce random error.



### Mean, Standard Deviation, Standard

The most well established method to quantify the spread of random errors in a measurement is to compute the **standard deviation**. Suppose you make $N$ measurements $x_1, x_2, \ldots, x_N$ of a certain quantity $x$. The average value is:


```{math}
:label: eq-errorMeanX
\bar{x}=\frac{x_1 + x_2 + \ldots + x_N}{N}=\frac{1}{N}\sum_{i=1}^N x_{i},
```

and the standard deviation of the individual measurements is

```{math}
:label: eq-errorSigmaX
\sigma = \sqrt{\frac{(x_1-\bar{x})^2 + (x_2-\bar{x})^2 + \ldots + (x_N-\bar{x})^2}{N-1}} = \sqrt{\frac{1}{N-1} \sum_{i=1}^{n}\left(x_i-\bar{x}\right)^2}.
```

In Excel, these operations can be carried out using the functions `AVERAGE()` and `STDEV()` or `STDEV.S()`.

If you perform many measurements, then your estimate of the average value improves. The **standard deviation of the mean** (a.k.a. **standard error**) for $N$ measurements is

```{math}
:label: eq-errorSigmaMeanX
\sigma_{\mbox{mean}} = \frac{\sigma}{\sqrt{N-1}}.
```

Your **best estimate of a measurement** $x$ is then $\bar{x} \pm \sigma_{\text{mean}}$.


### Example of Average $\pm$ Standard Error

Suppose you take four length measurements (cm): 7.65, 7.61, 7.66, 7.68

The mean value is

```{math}
\bar{x} = \left(7.65 + 7.61 + 7.66 + 7.68\right)/4\,\text{cm}
= 7.65\,\text{cm},
```

and the standard deviation is

```{math}
\sigma = \sqrt{\frac{(7.65-7.65)^2 + (7.61-7.65)^2 +
(7.66-7.65)^2 + (7.68-7.65)^2}{4-1}\,\text{cm}^2}
= 0.029\,\text{cm}.
```

The standard error (i.e. standard deviation of the mean) of the average value is thus reduced to $ 0.029\,\text{cm} / \sqrt{3} = 0.017\,\text{cm}$ and therefore the best estimate of the length is $\bar{x} = 7.65\,\text{cm} \pm 0.017\,\text{cm}$.


### Estimation through Variation or Instrumentation

Frequently, a set of measurements has to be taken in an experiment under a prescribed condition. It may be difficult to judge exactly when this condition is satisfied. In this case, it may be necessary to vary the physical quantities that produce this condition and to note how much each may be varied without appreciably altering the prescribed condition. This variation may be used to determine the error.

Finally, the measuring devices (meter stick, voltmeter, and so on) are not perfectly accurate even if one could make a precise reading with them. The manufacturer specifies the accuracy in the measuring device; for example, a particular type of voltmeter may be guaranteed to give readings accurate to $\pm 1\%$ of full scale reading. Part of this tolerance is random error that can average out by taking multiple readings. As discussed in the next section, another part of the instrument error is systematic. An ammeter may always read $0.5\%$ high because of the value of a resistor internal to the device.




---


## Systematic Errors

Systematic errors occur in an experiment because of a defective measuring apparatus, faulty methods, or incomplete working equations or assumptions. They are definite in sign and magnitude and cannot be reduced by averaging because the same error is included in each measurement.

These errors are often *more important* than the random errors. Calibrating the measuring apparatus, modifying the method, or correcting the equations may reduce them. These are generally described as corrections that are made in the performing of the experiment.



### Examples of Systematic Errors

- The reading of a Vernier caliper may not be zero when the jaws are in contact. This so-called zero error must be corrected for in using the instrument, i.e., the instrument must be calibrated. Otherwise, all measurements made with the caliper will be in error by a determinate amount, the zero error.

- In many experiments time is measured with a stopwatch. Using a stopwatch that does not run at the proper rate would introduce an instrumental systematic error. A watch that ran too fast would cause all times recorded to be too high. 

- A more significant systematic error encountered with a stopwatch is reaction time error. In measuring the time for an air track glider to travel down an incline, the observer may introduce a systematic error due to the reaction time required to stop the watch and a random error due to variation in reaction time. 

Report these sources of error as **Vernier caliper error** or **reaction time error.** The expression **human error** is too ambiguous to be useful in describing measurement errors.

```{admonition} Error Description
:class: caution
**NEVER** state the source of an error as ***human error*** due to ambiguity. Be clear and descriptive.
```


---

## Difference Between Experimental and Expected Values

If the true value of a quantity is known, then the systematic error can be estimated as difference between the experimental and expected values. It is important to remember that this is an *estimate of the ***systematic error****. The difference between your experimental value and the expected value is **not** *an estimate of the random experimental error*. 


To report this difference as a percentage (**percent difference**), divide the difference by the true, expected, or actual value and multiply by $100\%$. In Excel, you can use percent format instead of multiplying by $100\%$.

The percent difference between experimental and actual values is

```{math}
:label: eq-percentDifferenceinErrorAnalysis
\frac{\text{Experimental Value} - \text{Actual Value}}{\text{Actual Value}} \times 100%.
```

Sometimes, rather than a difference to actual values, you will be looking at how some quantity changes from an initial to final state. Similar to percent difference, you can report a **percent change** (when applicable) to help contexualize the process with

```{math}
:label: eq-percentChangeinErrorAnalysis
\frac{\text{Final Experimental Value} - \text{Initial Experimental Value}}{\text{Initial Experimental Value}} \times 100%.
```




### Example of \% Difference

Suppose a student measures the value of gravity and will compare to the standard accepted value.

- Measured value of gravity: $9.40\,\text{m/s}^2$
- Standard value: $9.803\,\text{m/s}^2$

The systematic relative difference, expressed as a percentage, is 

$$
\frac{9.40 - 9.803}{9.803} \times 100\% = \frac{-0.403}{9.803} \times 100\% = -4.11\%
$$

It is important to maintain the proper sign of the error as it indicates whether your experimental value was larger or smaller than the actual value (or increased/decreased in the context of \% change). **There is no definite allowable difference** between the experimental and expected values in this course's experiments. However, all measurements should be made with the greatest care, so as to reduce the error as much as possible.

It should be noted that the percent difference is not an estimate of experimental error. Any measurement has random and systematic errors even if the percent difference happens to be small. 

```{admonition} Small \% Difference $\ne$ Small Experimental Error
:class: tip
A small percent difference does not imply small experimental error; it result from cancellation of errors.
```

Often, scientists do not know the actual value of the quantity they are measuring and they give their best estimate with error. Comparing the **difference** between the experimental and actual values with your best estimate of the experimental error (e.g. using standard deviation $\sigma$, standard error $\sigma_\text{mean}$, or direct measurement uncertainties $\delta$) will help determine if there is a systematic error in your results. 

- If the difference is less than your estimated random error, then the results are consistent with the expected value. 
- Having a zero percent difference could be the result of a lucky cancellation of errors and still just means the results are consistent. 
- If the difference is significantly more than the estimated error, then you can begin to ask why your result is not consistent with the expected value.





---

(error-analysis-ErrorPropagation)=
## Propagation of Systematic Errors through 1. Brute Force \& 2. Calculus


Through indirect measurement, the effect of systematic errors can be followed through the equations used. Two simple examples will be discussed.

### Calculation from a Single, Direct Measurement (Sphere)

Consider the volume of a sphere $V$ as calculated from a direct measurement of its diameter, $D$. We would use

$$
V = \frac{1}{6} \pi D^3
$$

where $\pi = 3.1415926\ldots$. Suppose the value of $D$ is measured as $3.04\,\text{cm}$ and $V$ computed to be $14.71\,\text{cm}^3$. It is later discovered that the value of $D$ has a systematic error $\Delta D = +0.01\,\text{cm}$, (unnecessarily large, in all probability). What is the error $\Delta V$ in $V$ and the corrected value of $V$?

#### 1. Direct, brute-force method  
- Correct $D$ to $3.03\,\text{cm}$
- Re-compute $V_{\text{corrected}}$ as $14.56\,\text{cm}^3$
- The systematic error $\Delta V$ in $V$ is then $V - V_{\text{corrected}} = +0.15\,\text{cm}^3$ or $+1\%$

#### 2. Method based on calculus  
Find the derivative of $V$ with respect to $D$,

  ```{math}
  :label: Eq-errorCalcMethod
  \frac{{\rm d}V}{{\rm d}D} = \frac{3}{6} \pi D^2

  {\rm d}V = \frac{3}{6} \pi D^2 {\rm d}D
  ```


  Note that this shows a direct dependence of a change in $V$ on an infinitesimal change in $D$. Now divide through by $V = \frac{1}{6} \pi D^3$

  ```{math}
  \frac{{\rm d}V}{V} = 3 \frac{{\rm d}D}{D}.
  ```

  If a finite change in $D$, such as the systematic error $\Delta D$, is small compared to $D$, then ${\rm d}V$ and ${\rm d}D$ can be approximated by $\Delta V$ and $\Delta D$, respectively, and so the following can be written:

  ```{math}
  \frac{\Delta V}{V} \approx 3 \frac{\Delta D}{D}.
  ```

  This means that the fractional or percent error in $V$ is very nearly 3 times as large as that in $D$. Another way to say, a 1\% error in diameter produces a 3\% error in volume. Therefore,

  ```{math}
  \frac{\Delta V}{V} \approx + 3 \frac{0.01}{3.04} \approx 1 \%.
  ```

  Hence,

  ```{math}
  \Delta V \approx 0.15\,\text{cm}^3
  ```

  and

  ```{math}
  V_{\text{corrected}} = V - \Delta V = 14.56\,\text{cm}^3.
  ```

    

### Calculation from Two or More Direct Measurements (Cylinder)

Consider the volume $V$ of a right, circular cylinder as calculated from its diameter $D$ and length $L$. For convenience, let $D$ be measured as $2.00\,\text{cm}$ and $L$ as $5.00\,\text{cm}$. Then,

```{math}
V = \frac{1}{4} \pi L D^2 = 15.71\,\text{cm}^3.
```

If $D$ has an error of $+0.01\,\text{cm}$ and $L$ an error of $-0.02\,\text{cm}$, what is the error $\Delta V$ in $V$ and what is the corrected value of $V$?

#### 1. Direct, brute-force method
To obtain $V_{\text{corrected}}$
- Subtract $0.01\,\text{cm}$ from $D = 2.00\,\text{cm}$
- Add $0.02\,\text{cm}$ to $L = 5.00\,\text{cm}$
- Recompute $V_{\mbox{corrected}}$ as $15.61\,\text{cm}^3$, whereby $\Delta V$ must be $+0.01\,\text{cm}^3$.

#### 2. Method based on calculus
Find the partial derivatives of $V$

  ```{math}
  \frac{\partial V}{\partial L} =\frac{1}{4} \pi D^2 \hspace{2 cm} \frac{\partial V}{\partial d} =\frac{1}{2} \pi D L
  ```

  ```{math}
  {\rm d} V = \frac{\partial V}{\partial L} {\rm d} L + \frac{\partial V}{\partial D} {\rm d} D
  ```

  so that

  ```{math}
  \Delta V \approx \frac{\partial V}{\partial L} \Delta L + \frac{\partial V}{\partial D} \Delta D = \frac{\pi}{4} D^2 \Delta L + \frac{\pi}{2} D L \Delta D.
  ```

  Now dividing through by $V = \frac{1}{4}\pi , D^2 , L$

  ```{math}
  \frac{\Delta V}{V} \approx \frac{\Delta L}{L} + \frac{2 \Delta D}{D}.
  ```

  This shows how fractional errors in each measured quantity contribute to the total error in the calculated result; i.e. the fractional (or percent) systematic error in $V$ is very nearly equal to the fractional systematic error in $L$ plus twice the fractional error in $D$. In our case,

  ```{math}
  \frac{\Delta L}{L} = \frac{-0.02}{5.00} = -0.4 \%
  ```

  and

  ```{math}
  \frac{2\Delta D}{D} = \frac{+0.02}{2.00} = +1.0 \%
  ```

  so that

  ```{math}
  \frac{\Delta V}{V} \approx +0.6 \%.
  ```

  Thus $\Delta V = +0.09\,\text{cm}^3$, i.e. the systematic error, is $+0.09\,\text{cm}^3$; the correction is $-0.09\,\text{cm}^3$ and $V_{\text{corrected}} = +15.62\,\text{cm}^3$.



