# Velocimeter

## Introduction

Optical encoder is device which converts angular displacement directly into digital form. Therefore, they can be used to estimate the linear speed and distance of a rotating body such as a shaft or a wheel in various mechanical systems. 

In this project, a velocimeter program was coded in LabVIEW that processed the digital signals from an optical encoder to measure a real-world scenario, such as dropping a weight to estimate the acceleration due to gravity.

## Folder Structure

```
└───Velocimeter
    ├───Experimantal Media Files
    ├───Glyphs
    ├───Saved Data Files
    ├───Screenshots
    ├───Simulation Files
    ├───SubVIs
    └───Type DefsProjectName
```

`Experimental Media Files` - contains the files for demonstration.

`Glyphs` - contains the thumbnails for the user defined functions.

`Saved Data Files` - contains the final output the program with the calculated acceleration.

`Screenshots` - contains the screenshots of the program for quick reference.

`Simulation Files` -  contains the raw .csv files that can be inputed into the LabView UI to produce the Saved Data Files.

`SubVIs` -  contains user defined functions.

`Type DefsProjectName` - contatins .ctl file for state machine architecture.

## State Machine 

The velocimeter has 5 states:
1. Intialise - intialises the parameters to prepare for data acquisition from the optical encoder.
2. Idle - program moves to idle state after it intialises the parameters and remains in that state until user interacts with the UI to 'Begin Test'.
3. Select Method - allows the user to choose whether they want simulate using one of the .csv files or collect fresh data from the optical encoder.
4. Process Data - based on the user input from the Select Method state the data is processed accordingly.
5. End - final state where user can choose to exit or test again which would bring the state back to idle.

## Dashboard and Block Diagram

![Diagram](/Screenshots/Dashboard_Screenshot.PNG)
<p align="center"><b>Figure 1:</b> Dashboard.</p>

![Diagram](/Screenshots/Process-Data-Block-Diagram.PNG)
<p align="center"><b>Figure 2:</b> Process Data block diagram.</p>

