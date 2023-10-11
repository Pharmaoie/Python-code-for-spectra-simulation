# Python-code-for-spectra-simulation
Python script that generates a plot of ensemble average vertical excitation spectra with multiple datasets. 
It uses Matplotlib for visualization and NumPy for numerical operations. The code defines functions to create Gaussian summation curves and plots stick spectra with error bars for each dataset. It also includes additional data as a scatter plot.

Code Structure
The code consists of several sections:

Importing Libraries:

The code begins by importing necessary Python libraries, including sys, imp, numpy, and matplotlib. It also imports FontProperties from matplotlib.font_manager.
Define the gaussBand Function:

The gaussBand function is defined to create Gaussian summation curves. It takes input values x (an array of x-coordinates), bands (an array of center positions for Gaussian peaks), strengths (an array of strengths for each peak), and stdev (standard deviation for the Gaussian curves).
Set Configuration Variables:

Several variables are defined to configure the plotting behavior. You can adjust these variables to change the portion of the spectrum to be plotted and the number of points for plotting.
Sample Data and Additional Data:

Sample data for different datasets are defined as dictionaries. Each dataset contains energies, deviations in both x and y directions, intensities, and a label.
Additional data is also defined as a dictionary, which includes energies and intensities to be plotted as a scatter plot.
Create a Plot:

A Matplotlib figure and axis are created.
Custom fonts are defined for axis labels and legends.
The primary y-axis (ax1) and a secondary y-axis (ax2) are created.
A loop iterates over the datasets, where each dataset is plotted with stick spectra and error bars.
A Gaussian curve is generated for each dataset and plotted on the secondary y-axis.
Additional data is plotted as a scatter plot on the secondary y-axis.
Customize the Plot:

Labels, titles, and legend placement are customized.
The lower limit of the y-axis is set to zero to ensure the plot starts from the baseline.
Combine Legends:

Legends from both axes are combined, and their location is set to the upper left corner of the plot.
Customize Tick Labels:

The font size of tick labels on both axes is customized.
Display the Plot:

The plot is displayed without a background grid.
How to Use
To use this code:

Make sure you have the required Python libraries installed (NumPy and Matplotlib).
Configure the variables in the code to specify the portion of the spectrum to be plotted and other parameters.
Define your datasets by modifying the data_sets and additional_data dictionaries.
Run the script to generate the plot.
The resulting plot will display ensemble average vertical excitation spectra with stick spectra for multiple datasets and additional data as a scatter plot.

Please note that this code includes sample data, so you should customize it with your own dataset to obtain meaningful results.
