# Error Analysis Review

In laboratory work, it is usually necessary to use experimental apparatus to measure physical quantities. The measurements are seldom, if ever, perfect. As a result, imperfections must be taken into account in any set of physical measurements. One of the most important things to be learned in the laboratory is how to make reliable estimates of the uncertainties involved in any physical measurements and how to handle the propagation of these errors, i.e., to know how the uncertainties affect calculated results of an experiment.

---

(error-analysis-sigFig)=
## Significant Figures

The number of digits required to express the result of an experimental measurement, so that it reflects the accuracy with which the measurement was made, are known as **significant figures**. Thus, the number of significant figures reflects the limitation of the measuring device and/or the experimenter. Whether the calculations are performed by hand or on a computer, the number of significant figures displayed in the final result must reflect the limitations of the experimental measurement. Often, a computer program will, by default, display either too many or too few digits. If too few digits are displayed, you need to adjust the program setting to show more digits.

For example, if the length of a cylinder is measured as $20.64,\text{cm}$, this quantity is said to be measured to four significant figures. If written as $0.0002064,\text{km}$, we still have only four significant figures. The zeros preceding the “2” are used only to indicate the position of the decimal point. The zero between the “2” and the “6” is a significant figure, but the other zeros are not.

If the above measurement is made with a meter stick, the last digit recorded is an estimated figure representing a fractional part of a millimeter division. All recorded data should include the last estimated figure in the result, even though it may be zero. If this measurement had appeared to be exactly $20$, it should have been recorded as $20.00,\text{cm}$, since lengths can be estimated by means of this instrument to about $0.01,\text{cm}$.

When the measurement is written as $20,\text{cm}$ it indicates that the value is known to be somewhere between $19.5,\text{cm}$ and $20.5,\text{cm}$, whereas the value $20.00,\text{cm}$ indicates a range between $19.995,\text{cm}$ and $20.005,\text{cm}$. Conversely, retaining too many significant figures implies greater accuracy than the figures actually represent.

### Rules for Significant Figures

* ▶ When collecting data, only one estimated figure is retained as a significant figure.
* ▶ In addition and subtraction, do not carry the result beyond the first column that contains an estimated figure.
* ▶ In multiplication and division, the result should have as many significant figures as the factor with the least number of significant figures.
* ▶ When dropping figures that are not significant, round to the nearest significant digit.
* ▶ While performing intermediate calculations, it is safer to carry one more significant figure than is required in the final result.

### Examples

**Addition**

```text
  427.5
   28.03
    0.0654
  396.0
  ------
  851.6
```

The result is rounded to one decimal place because the first term is given only to one decimal place.

**Multiplication**

If the length of a rectangle is $1.94,\text{cm}$ and the width is $1.84,\text{cm}$, the area is

$$
A = 1.94 \times 1.84 = 3.5696,\text{cm}^2.
$$

Since each factor has three significant figures, the result should be reported as

$$
A = 3.57,\text{cm}^2.
$$

In Excel, the number of significant figures can be controlled by formatting the cell to a *Number* type with the desired number of decimal places.

---

(error-analysis-ErrorProc)=
## Error Analysis Procedure
The steps for performing error analysis are:

* ▶ Identify the likely sources of measurement error.

  * Instrumentation
  * Experimental setup and procedure
  * Determine whether errors are systematic or random (see {numref}`error-analysis-TypesErrors`).

* ▶ Estimate the magnitude of measurement errors using:

  * Equipment specifications
  * Significant digits displayed
  * Your estimate of reading accuracy
  * The range or standard deviation of repeated measurements

* ▶ Calculate the expected error in calculated quantities due to measurement errors (see {numref}`error-analysis-ErrorPropagation`).

* ▶ If the difference between experimental and expected results is much larger than the expected error, check for:

  * Experimental mistakes
  * Calculation or unit conversion errors
  * Incorrect use of degrees vs. radians
  * Underestimated measurement error
  * Incorrect constants

* ▶ Report results with the correct number of significant figures and the calculated error.

---

(error-analysis-TypesErrors)=
## Types of Errors

Experimental measurements are characterized by **accuracy** and **precision**.

* A set of measurements is *accurate* if the average value is close to the expected value.
* A set of measurements is *precise* if the measurements are closely clustered.

Random errors increase scatter and reduce precision. They arise from uncontrollable variations and can be reduced by repeated measurements. Systematic errors arise from calibration issues or faulty methods and cannot be reduced by averaging.

---


```{figure} IntroductionFigures/ErrorType_v4.png
:name: ErrorAnalysis_Fig01
:width: 100%
:align: center

The distinction between precision and accuracy.
```




Each measurement contains both systematic and random errors. Estimate the error in each measured quantity, then recalculate results using maximum and minimum values to determine the expected range of outcomes.

### Example: Density of a Block

Given

* $L = 2.00,\text{cm}$, $W = 3.00,\text{cm}$, $H = 5.00,\text{cm}$
* $M = 60.00,\text{g}$
* Uncertainty in length: $\pm 0.01,\text{cm}$
* Uncertainty in mass: $\pm 0.05,\text{g}$

The experimental density is

$$
\rho = \frac{60.00}{30.00} = 2.00,\text{g/cm}^3.
$$

Using maximum mass and minimum volume gives

$$
\rho_{\max} = 2.02,\text{g/cm}^3,
$$

and the minimum density is $1.98,\text{g/cm}^3$. If the expected value lies outside this range, further investigation is required.

---

(error-analysis-RandomErrors)=
## Random Errors

Random errors are inherent in nearly all measurements. They are assumed to be equally likely positive or negative and are more likely to be small than large. Independent repeated measurements reduce their effect.

### Mean and Standard Deviation

For $N$ measurements $x_1, x_2, \ldots, x_N$:

$$
\bar{x} = \frac{1}{N} \sum_{i=1}^{N} x_i,
$$

$$
\sigma = \sqrt{\frac{1}{N-1} \sum_{i=1}^{N} (x_i - \bar{x})^2}.
$$

The standard deviation of the mean is

$$
\sigma_{\text{mean}} = \frac{\sigma}{\sqrt{N-1}}.
$$

Your best estimate is $\bar{x} \pm \sigma_{\text{mean}}$.

### Example

Measurements (cm): 7.65, 7.61, 7.66, 7.68

* Mean: $7.65,\text{cm}$
* Standard deviation: $0.029,\text{cm}$
* Standard deviation of the mean: $0.017,\text{cm}$

Result:

$$
7.65 \pm 0.017,\text{cm}.
$$

---


## Systematic Errors

Systematic errors arise from faulty equipment, methods, or assumptions. They have a definite sign and magnitude and cannot be reduced by averaging. Calibration, improved procedures, or corrected equations are required to reduce them.

Examples include zero errors in calipers, incorrect stopwatch timing rates, and consistent reaction-time bias. Avoid vague descriptions such as “human error”; instead, specify the source clearly.

---

## Difference Between Experimental and Expected Values

If the true value is known, the systematic error may be estimated as the difference between the experimental and expected values. This difference is **not** an estimate of random error.

The percent difference is

$$
\frac{\text{Experimental Value} - \text{Actual Value}}{\text{Actual Value}} \times 100%.
$$

### Example

Measured value of gravity: $9.41,\text{m/s}^2$

Standard value: $9.803,\text{m/s}^2$

$$
\text{Percent difference} = \frac{-0.39}{9.803} \times 100% = -4.1%.
$$

A small percent difference does not imply small experimental error; it may result from cancellation of errors.

---

(error-analysis-ErrorPropagation)=
## Propagation of Errors

### Single Direct Measurement

For the volume of a sphere

$$
V = \frac{1}{6} \pi D^3,
$$

small errors obey

$$
\frac{\Delta V}{V} \approx 3 \frac{\Delta D}{D}.
$$

Thus, a 1% error in diameter produces a 3% error in volume.

---

### Two or More Direct Measurements

For a cylinder

$$
V = \frac{1}{4} \pi L D^2,
$$

small errors propagate as

$$
\frac{\Delta V}{V} \approx \frac{\Delta L}{L} + 2 \frac{\Delta D}{D}.
$$

This shows how fractional errors in each measured quantity contribute to the total error in the calculated result.
