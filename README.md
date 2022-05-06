Description

The database includes online handwriting features of 101 students consisting of 49 students with Dysgraphia disorder and
52 non-dysgraphic students of first, second, and third grades, all of whom were right-handed, with 41 female students and the rest male.
Samples were taken from four schools and 15 classes, and both groups matched in age, gender, school, and class.
All participants were born in Iran and speak Persian.

We asked students to copy a couple of verses written on the board on a piece of paper placed on a digitizer.
The INTUOS PRO PAPER Large Digitizer was used to obtain children's handwriting information online.
This digitizer is able to record the following information almost every 5 milliseconds:
– Stroke number
– (X, Y, and Z): coordinates of the position of the pen on the tablet and in-air. 
– Pressure (8,192 pen pressure levels): the pressure on the pen. 
– Altitude (from 30 to 90 degrees): the angle between the pen and its projection on the tablet. 
– Azimuth (from 0 to 359 degrees): the angle of the pen barrel projected on the x-y tablet plane. 
– Time: the time in which the sample was taken.
– BTN: a binary variable, being 0 for the pen-up state (in-air movement) and 1 for the pen-down state (on-surface movement)

In addition to recording pen information when the pen is in contact with the tablet screen (on-surface),
this digitizer can also record pen information even when the pen is in the air and does not come in contact with the tablet, we call it in-Air.
In-Air Pen data recording is performed until the pen is approximately 10 mm away from the tablet screen.
To get the above information from the pen, we provided software that after the student has finished the poem,
the pen information is stored in a record for every 5 milliseconds, and depending on how long the writing process takes, the records are saved.

In this dataset, each student is identified by a number that can be accessed in any section with this number.

The database consists of three folders:
1. The "raw data" Folder contains the raw pen-tablet data for each student that was obtained during the writing process and stored in the form of a CSV file.
Each CSV file contains ten columns in the following order:
* Index,Btn,Stroke,X,Y,Z,Time,Pressure,Azimuth,Altitude

2. The "images" folder contains images adapted from the raw data and contains three subfolders:
* The "On-Surface" subfolder contains images of pen movements on the tablet surface.
* The "In-Air" subfolder contains images extracted from the movements of the pen when the pen does not touch the screen.
* The "Both" subfolder contains images extracted from both On-Surface and In-Air.
Students were asked to complete the task in a specific box on paper, and the images were not crop because the X and Y of the pen were not lost. 

3. The "info" Folder contains the following labels and personal information:
* label (1:dysgraphic, 0: non-dysgraphic)
* Gender (0:female, 1:male)
* Right/left hand (0:right, 1:left)
* Age
* Grade point average
* HPSQ Score

The order of the values inside the "info" folder files is as follows:
* Label,Gender,Handedness,Age,GPA,HPSQ

