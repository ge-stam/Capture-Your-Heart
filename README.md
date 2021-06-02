Program organization:
The main.py file contains the main program that utilizes all of the other modules defined in the other code files to read in the input video, run Eulerian magnification on it, and to display the results. The purposes of the other files are described below:

preprocessing.py - Contains function to read in video from file and uses Haar cascade face detection to select an ROI on all frames
pyramids.py - Contains functions to generate and collapse image/video pyramids (Gaussian/Laplacian)
eulerian.py - Contains function for a temporal bandpass filter that uses a Fast-Fourier Transform
heartrate.py - Contains function to calculate heart rate from FFT results
How to run:
To run the program, specify the path to the input video in the preprocessing.read_video() function on line 13 of main.py. To alter the frequency range to be filtered, change the values assigned to freq_min and freq_max on lines 8 and 9.
