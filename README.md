# IRIS-PSF-Magnitude-Extraction

IRIS Point Spread Function Magnitude Extraction
This repository contains Python code for extracting the magnitudes from IRIS (astro surf astronomical image processing software) generated by the point spread function on a star.
```
x=4377  y=2194  i=2862 
X = 4404.673  -  Y = 2151.556
Intensity = 678013.6  -  Background = 2897.58
Magnitude = -14.578
FWHM X = 25.27  -  FWHM Y = 24.67
```
to
```
Magnitudes:
-14.578
...
```

Prerequisites
```
pip install tkinter
```
How to Use

Download either ExtractMagnitude.py or Extract MadnitudewAverage.py
> ExtractMagnitude is for singular readings taken on a single image 

> ExtractMagnitudewAverage is for 5 readings taken on a single image which is then averaged into a single reading. The code will read the input file, extract the magnitudes, and calculate the average of the last 5 magnitudes found.

A graphical user interface window will appear after running the script.
Click the "Browse" button to select the input file containing the IRIS data. The input file should be a text file saved from IRIS's analyse -> display data window.
Next, choose the output file where the calculated magnitudes will be written. The output file should have a '.txt' extension.

##Data Extraction and Magnitude Calculation

The calculated average will be written to the specified output file.

#Check the Output

Once the process is complete, you will see a message indicating the successful export of magnitudes and intensities to the output file.

##Example Data Format
For successful execution, ensure that your input file follows the example format:
Magnitudes:
-18.123
-18.456
-18.789
...

##Important Note
This code is designed specifically for IRIS data in the given format. Modify the code accordingly if your data has a different structure or if additional preprocessing is required.
