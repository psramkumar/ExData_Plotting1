## Introduction

This assignment uses data from
the <a href="http://archive.ics.uci.edu/ml/">UC Irvine Machine
Learning Repository</a>, a popular repository for machine learning
datasets. In particular, we will be using the "Individual household
electric power consumption Data Set" which I have made available on
the course web site:


* <b>Dataset</b>: <a href="https://d396qusza40orc.cloudfront.net/exdata%2Fdata%2Fhousehold_power_consumption.zip">Electric power consumption</a> [20Mb]

* <b>Description</b>: Measurements of electric power consumption in
one household with a one-minute sampling rate over a period of almost
4 years. Different electrical quantities and some sub-metering values
are available.


The following descriptions of the 9 variables in the dataset are taken
from
the <a href="https://archive.ics.uci.edu/ml/datasets/Individual+household+electric+power+consumption">UCI
web site</a>:

<ol>
<li><b>Date</b>: Date in format dd/mm/yyyy </li>
<li><b>Time</b>: time in format hh:mm:ss </li>
<li><b>Global_active_power</b>: household global minute-averaged active power (in kilowatt) </li>
<li><b>Global_reactive_power</b>: household global minute-averaged reactive power (in kilowatt) </li>
<li><b>Voltage</b>: minute-averaged voltage (in volt) </li>
<li><b>Global_intensity</b>: household global minute-averaged current intensity (in ampere) </li>
<li><b>Sub_metering_1</b>: energy sub-metering No. 1 (in watt-hour of active energy). It corresponds to the kitchen, containing mainly a dishwasher, an oven and a microwave (hot plates are not electric but gas powered). </li>
<li><b>Sub_metering_2</b>: energy sub-metering No. 2 (in watt-hour of active energy). It corresponds to the laundry room, containing a washing-machine, a tumble-drier, a refrigerator and a light. </li>
<li><b>Sub_metering_3</b>: energy sub-metering No. 3 (in watt-hour of active energy). It corresponds to an electric water-heater and an air-conditioner.</li>
</ol>

## Loading the data





When loading the dataset into R, please consider the following:

* The dataset has 2,075,259 rows and 9 columns. First
calculate a rough estimate of how much memory the dataset will require
in memory before reading into R. Make sure your computer has enough
memory (most modern computers should be fine).

* We will only be using data from the dates 2007-02-01 and
2007-02-02. One alternative is to read the data from just those dates
rather than reading in the entire dataset and subsetting to those
dates.

* You may find it useful to convert the Date and Time variables to
Date/Time classes in R using the `strptime()` and `as.Date()`
functions.

* Note that in this dataset missing values are coded as `?`.


## Making Plots

Our overall goal here is simply to examine how household energy usage
varies over a 2-day period in February, 2007. Your task is to
reconstruct the following plots below, all of which were constructed
using the base plotting system.

First you will need to fork and clone the following GitHub repository:
[https://github.com/rdpeng/ExData_Plotting1](https://github.com/rdpeng/ExData_Plotting1)


For each plot you should

* Construct the plot and save it to a PNG file with a width of 480
pixels and a height of 480 pixels.

* Name each of the plot files as `plot1.png`, `plot2.png`, etc.

* Create a separate R code file (`plot1.R`, `plot2.R`, etc.) that
constructs the corresponding plot, i.e. code in `plot1.R` constructs
the `plot1.png` plot. Your code file **should include code for reading
the data** so that the plot can be fully reproduced. You should also
include the code that creates the PNG file.

* Add the PNG file and R code file to your git repository

When you are finished with the assignment, push your git repository to
GitHub so that the GitHub version of your repository is up to
date. There should be four PNG files and four R code files.


The four plots that you will need to construct are shown below. 


### Plot 1

* Step 1: Set your Project Folder as working Directory
    * setwd(this.dir <- dirname(sys.frame(1)$ofile))
* Step 1: Download Data from specified URL
* Step 2: UNzip the downloaded file to your working Dir
* Step 4: Reads in data from file then subsets data for specified dates
* Step 5: Change Date Column to Date Type
* Step 6: Filter Dates for 2007-02-01 and 2007-02-02
* Step 7: Create PNG Device to render Plot
* Step 8: Use Hist function to create the Plot.
* Step 9: Close the Device always the good practice
* Step 10: Remove the files to save up memory


![Generated PNG for Plot1](https://github.com/psramkumar/ExData_Plotting1/blob/master/plot1.png)


### Plot 2

* Step 1: Set your Project Folder as working Directory
    * setwd(this.dir <- dirname(sys.frame(1)$ofile))
* Step 1: Download Data from specified URL
* Step 2: UNzip the downloaded file to your working Dir
* Step 4: Reads in data from file then subsets data for specified dates
* Step 5: Prevents Scientific Notation
* Step 6: Making a POSIXct date capable of being filtered and graphed by time of day
* Step 7: Filter Dates for 2007-02-01 and 2007-02-02
* Step 8: Create PNG Device to render Plot
* Step 9: Use Plot function to create the Plot.
* Step 10: Close the Device always the good practice
* Step 11: Remove the files to save up memory

![Generated PNG for Plot2](https://github.com/psramkumar/ExData_Plotting1/blob/master/plot2.png)

### Plot 3

* Step 1: Set your Project Folder as working Directory
    * setwd(this.dir <- dirname(sys.frame(1)$ofile))
* Step 1: Download Data from specified URL
* Step 2: UNzip the downloaded file to your working Dir
* Step 4: Reads in data from file then subsets data for specified dates
* Step 5: Prevents Scientific Notation
* Step 6: Making a POSIXct date capable of being filtered and graphed by time of day
* Step 7: Filter Dates for 2007-02-01 and 2007-02-02
* Step 8: Create PNG Device to render Plot
* Step 9: Use Plot function to create the Plot.
* Step 10: Use line function to create Sub_metering_2 line with red color.
* Step 11: Use line function to create Sub_metering_3 line with Blue color.
* Step 12: Use legend function to create Legend on right corner with the proper Title
* Step 13: Close the Device always the good practice
* Step 14: Remove the files to save up memory

![Generated PNG for Plot3](https://github.com/psramkumar/ExData_Plotting1/blob/master/plot3.png)


### Plot 4

 Step 1: Set your Project Folder as working Directory
    * setwd(this.dir <- dirname(sys.frame(1)$ofile))
* Step 1: Download Data from specified URL
* Step 2: UNzip the downloaded file to your working Dir
* Step 4: Reads in data from file then subsets data for specified dates
* Step 5: Prevents Scientific Notation
* Step 6: Making a POSIXct date capable of being filtered and graphed by time of day
* Step 7: Filter Dates for 2007-02-01 and 2007-02-02
* Step 8: Create PNG Device to render Plot
* Step 9: Use [par](https://www.rdocumentation.org/packages/graphics/versions/3.4.3/topics/par) function to create Graphical Parameter with 2 by 2 matrix
* Step 10: Use Plot function to create the first Plot for Global Active Power
* Step 11: Use Plot function to create the second Plot for Voltage
* Step 12: Use Plot function to create the third Plot for Energy sub metering
* Step 12: Use Plot function to create the fourth Plot for Global Reactive Power
* Step 13: Close the Device always the good practice
* Step 14: Remove the files to save up memory

![Generated PNG for Plot4](https://github.com/psramkumar/ExData_Plotting1/blob/master/plot4.png)
