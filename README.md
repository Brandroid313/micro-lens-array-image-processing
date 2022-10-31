# micro-lens-array-image-processing
Internship project. This code was used to process the image data of a newly developed micro lens array for Kyoto University.
The goal of the code developed during the internship was to help process image data of small particles within a 1mm x 1mm area appoxminately 0.5mm in depth.
The depth is defined is the total distance from the ccd, so it follows the following pattern in the code ( -5.o, -5.1, -5.2 ... -5.5 ). In order
to properly detect the x, y and z axis of the particles detected, a gaussian, 2D gaussian and sum of 2D gaussian functions are applied. 
# Files overview
This was written in Juypter notebook and the 4 main files are:
- ccd_helpers -> This is the small library of functions I made to help with the image processing
- Particle Trajectory -> Juypter notebook file that process the tiff imgae data and plots its movement in 3 dimensions
- Calibrating_visualizaing_search_area -> This holds the code to calibrate the software to the image following the specifications 
found in the calibration pdf, and visualizes the search area for confirmation and debugging
- Calibration and Peak Trajectory -> This file combines both the Calibration code and the peak trajectory code to track the progress of the particle
