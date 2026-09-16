(data-acquisition-and-analysis-overall)=
# || Data Acquisition & Analysis in Excel & Capstone

## Purpose

Throughout this lab, you will perform measurements and interpret the results by using **spreadsheets** and a variety of measurement tools and sensors, some of which are controlled and monitored by PASCO's **Capstone** software. When appropriate, data analysis will entail conducting calculations, finding averages, uncertainties, standard deviations, or other error estimates.

Our experiments will often require many trials or multiple cases that require similar calculations. Spreadsheets and other computer programs can make these repetitive tasks more reliable, faster, reproducible, and presentable. The effort to set up the calculation is more than compensated by the subsequent ease of repeating calculations. Several experiments will make use of sensors connected to the lab computers to aid in measurements and data gathering. You can use **Capstone** to organize, analyze, and display that data.

This section presents:
  - How to access Microsoft Excel (used throughout the course)
  - Review of data manipulation and anlysis in Excel
  - Explain how to set up sensors and use **Capstone**. More detailed information will be given in the specific experiments.


## Microsoft Excel Spreadsheets --- How to Access

Throughout the course, we will use Microsoft Excel for all spreadsheets. To access Excel, you can do so through the browser with your Fairfield U. student login. We recommend doing your work in a browser to work with your lab group members on a shared Excel sheet, as that appears to be the most reliable and quick way to edit the same Excel spreadsheet. Follow the instructions here to access:

<a href="https://fairfield-university.atlassian.net/wiki/spaces/ITSKB/pages/30345528/Office+365+at+Fairfield+University" target="_blank">Access Office 365 in a browser at Fairfield University with your student login.</a>

Alternatively, you should be able to go to:

<a href="http://excel.cloud.microsoft/" target="_blank">http://excel.cloud.microsoft/</a> to Access Excel directly in a browser, use your Fairfield University student login.


(spreadsheet-data-analysis-setup)=
## Data Analysis with Spreadsheets

### Spreadsheet Orgnaization

A spreadsheet is a grid of **cells** organized into rows and columns where you can enter text, numerical values, or formulas. Spreadsheet programs provide all the mathematical functions, formatting, and graphing tools that you need for this lab course. They provide structure to data analysis that reduces calculation errors and repetitive typing.

You will often have multiple data tables within your speadsheet labeled with names and units including:
  - Common data values
  - Measurements and calculations
  - Summaries

For every data table, you will enter descriptors and values in different cells, **NEVER PLACE A NUMBER AND TEXT IN THE SAME CELL**, otherwise the spreadsheet won't be able to run calculations on that "string" of text:
  - Don't: `|9.803 m/s|`
  - Do: `|9.803|` and `|m/s|` as separate cells

Suggested use of separate rows and columns are:
- Use a row for each trial, labeled in the left cell with, for example, "Trial #1".
- Use a column for each measured or calculated value, labeled in the top cell with a description of the column and with units.

### Cell & Value Referencing

When you need a value for a calculation in a different cell, ***reference the value's cell*** rather than repeatedly, and sometime erroneously, typing in the same value:
  - Each accepted physical value such as $g$ and all common data for the experiment must be entered in cells and referenced in formulas that use that quantity.
  - **Do not retype** numbers. Use `$` to hold row or column coordinates constant that you don't want to change when copying formulas to different cells.
    - `$D5` will always refer to column `D` but the row will change.
    - `D$5` will always refer to row `5` but the column will change. 
    - `$D$5` will always refer to the same singlular cell.
- **Never** enter a value calculated outside the spreadsheet, for example, on your calculator. Any value you can find on the calculator can be calculated and updated automatically on the spreadsheet. Additionally, the spreadsheet shows your work, the outside calculator does not.

### Equations & Functions Syntax

You will create your own equations and use many built-in functions that exist in Excel and other spreadsheet programs to perform specific tasks on the input and return some output. Functions are often similar between spreadsheet programs, but not always, make sure to double check your syntax as needed. To start an equation or use a function in any given cell, you must first enter the equals sign: `=`. Say you wanted some simple addition, you would input `=3+5` and press enter at which point the cell would show a returned value of `8`.

Examples of other common functions are:
  - `=AVERAGE()` which returns the average of the referenced cells input between the parentheses
  - `=STDEV()` which returns the standard deviation of the referenced cells input between the parentheses
  - `=PI()` which returns the value of $\pi.$ NOTE: no input between parentheses

You can copy formulas to other cells by using the spreadsheet's "fill down" capability. Select an individual cell or a set of cells in a row and fill down by dragging with the little square in the bottom-right corner of the selected cell(s). Formulas will copy and the row numbers of referenced cells that are not preceded by `$` will increment automatically.
  - This approach makes it efficient to create a spreadsheet to analyze your data and to correct errors. If you make a mistake in a formula, you can correct the first trial and then correct the other trials by filling down.
  - This similarly works for columns filling right or left, or rows upward.


(data-acquisition-and-analysis-trigonometric-functions)=
### Trigonometric Functions

  - Excel *functions* like `SIN()`, `COS()`, etc. take some `input` between the parentheses (e.g. `SIN(input)`) and then return a value such that `output = SIN(input)`. 
  - Reminder, Excel likes radians; Excel's trig functions are expecting the input to be in units of ***radians***
    - *Convert to Radians:* Use `RADIANS()` function to take your angle in degrees and return it as radians for use in Excel's trig functions.
    - *Convert to Degrees:* Use `DEGREES()` function to take your angle in radians (or Excel's output of radians) and return it/convert it back as degrees for your use.
    - Example of deg. to rad. inside trig function: `=SIN(RADIANS(measured angle in degrees))` returns the sine of your angle in radians
    - Example of converting overall value back to degrees after sine is found: `=DEGREES(SIN(RADIANS(measured angle in degrees)))`
  - While we normally write a trig function to some power like $\sin^2\left(\frac{\theta}{2}\right)$; Excel does not know how to interpret that.
    - To square any function's output in Excel is like saying `output`$^2$. To do such a thing with a trig function (or any Excel function for that matter), we would instead type `=SIN(input-in-radians)^2`.


(data-acquisition-plotting-in-excel)=
### Plotting in Excel & LINEST

Unless otherwise stated, use Excel for graphs and for fitting data:
- Display the trendline (the equation of the fit, usually slope and intecept) on the graph itself.
- When applicable, conduct all error propagation analysis in your Excel spreadsheet.
- ***LINEST function for linear estimation***: When assuming a linear fit, $Y = mx +b$, use the `LINEST` function to calculate a plotted data's slope and y-intercept as well as their uncertainties. This allows us to have a referenceable cell for calculations that require the use of a trendline's values without having to manually copy the trendline information from the plot (which could introduce a chance of mistyping and messing up your calculations, or changes if you retest previous values).
  - Determine the slope of your graph using the `LINEST` function:
    - `=LINEST(y-values,x-values,TRUE/FALSE,TRUE/FALSE)`
      - unless otherwise stated, use of `LINEST` throughout the course will be ***`...TRUE,TRUE)`***
    - y-values are from your dependent variable
    - x-values are from your independent variable
    - Y-intecept
      - True to calculate the y-intercept like normal, just from the data
      - False to force the y-intercept to zero
    - Statistics
      - True to return statistics on the fit as shown in {ref}`tab-excel-linest-simplified-overview`
      - False to return just the slope
    ```{table} Simplified Excel LINEST Output (showing only slope and intercept)
    :name: tab-excel-linest-simplified-overview
    | Row | Column 1 (Slope)                         | Column 2 (Intercept)                         |
    |:---:|-------------------------------------------|-----------------------------------------------|
    |  1  | **Slope value $m$** – best-fit line slope     | **Intercept value $b$** – y-intercept of the line |
    |  2  | **Slope uncertainty $\delta m$** – std. error of *m*   | **Intercept uncertainty $\delta b$** – std. error of *b*   |
    |  3  | *(Ignored for this course)* R² and related metrics        | *(Ignored for this course)*                                   |
    |  4  | *(Ignored for this course)* Additional regression stats   | *(Ignored for this course)*                                   |
    |  5  | *(Ignored for this course)* Residual statistics           | *(Ignored for this course)*                                   |
    ```


(capstone-setup-data-aquisition)=
## Capstone

Many of our experiments use the *Capstone* program to communicate with measurement hardware and collect data. This section is a very brief introduction to using the *Capstone* software. Additional tools and tips can be found in {ref}`capstone-tools-tips-additional`.

### Setting up Hardware

Once you have opened the program you will notice a button labeled **Hardware Setup** on the left-hand side of the main window. If you click on the button you will get a list of all sensors that are currently connected to the computer. In almost all cases the program will recognize the connected sensor automatically and load a standard setup for the corresponding sensor. In a few cases you will be required to provide the program with certain values needed to determine the value of the quantity the sensor is supposed to measure. In the specific instructions for the experiment you will be told what values to provide. If you do not see the sensor try to dis- then reconnect the sensor to the computer or ask for help.

### Collecting Data

Upon opening the **Capstone** program you have the choice of several display modes for the data you will be collecting. The exact choice depends on the experiment you will be performing and detailed instructions will be provided if they deviate from the description below. In the simplest of all cases you will be using the **Table & Graph** display. If you click on this option the program will create a data table and a graph on the main canvas of the program. By default the measurements will be undetermined, but you can choose any variable that is allowed by the sensor to be displayed in the data table columns or on the graph axes. Clicking with the cursor onto the **Select Measurement** in the data table headers or on graph axes will allow you to chose the variable to display. At times a mathematical equation using the actual measured quantities can be defined by selecting the **Create New** → **Calculation** (data table) or **Add Similar Measurement** (graph axes) option in the pulldown menus.

To start collecting data you need to press the red **Record** button on the bottom of the **Capstone** window. The program will then record all data being collected by the sensors and display them as numbers in the data table and points on the graph. The data collection can be stopped by pressing the red **Record** button a second time. After collecting all the data the information can then be analyzed.

### Analyzing Data

Data can be analyzed by exporting the collected data into a data file, that can be read by Excel (or other mathematical program). An easier way to analyze the data is often to interpret the graph that has been produced by the **Capstone** program. Tools to analyze the graph are very readily available in the menubar above the graph window. The most important tools are discussed in more detail below:

- **Highlight range of points in active data**.  
  This option allows you to consider only the highlighted region of the data set to be analyzed. Once selected the program will display a rectangular area that can be resized and dragged over the collected data points. Only the points inside the rectangle will be considered in the selected analysis tool. The selected points will also be displayed in the data table with the same highlighting.

- **Display selected statistics for active data**.  
  Selecting this option will display several useful mathematical quantities for the selected data set, e.g. average of all values, mean of all values, maximum value, minimum value, etc.

- **Display area under active data**.  
  This option will allow you to calculate the area under the curve for the selected data points (the integral).

- **Apply selected curve fits to active data**.  
  With this option the user can fit a line of best fit to the elected data range. The drop down menu will give several options for graphs to fit (e.g. straight line, parabola, etc.)

- **Show coordinates and access delta tool**.  
  Once selected this tool will display a cross-hair onto the coordinate frame and allow to determine the values of specific points by placing the cursor onto a data point of the graph. Right-clicking on the cursor will allow to select a delta tool to determine a range in the data set (both $x$- and $y$-range).