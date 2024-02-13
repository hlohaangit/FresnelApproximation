# Fresnel Diffraction Simulation

This Python script simulates and visualizes the phenomenon of Fresnel diffraction.

## Dependencies

The script requires the following Python libraries:

- numpy
- matplotlib
- scipy

## Description

The script simulates the diffraction of light through an aperture and its propagation to a detector. The simulation includes the following steps:

1. Define the parameters of the system, such as the wavelength of the light, the diameter of the aperture, the size of the detector, the distance between the aperture and the detector, and the number of points used for calculations.

2. Create an array representing the positions along the x-axis on the detector.

3. Initialize an array representing the electric field at each position on the detector.

4. Set the elements of the electric field array to 0 where the position is outside the aperture.

5. Perform a Fourier Transform on the electric field array.

6. Apply a propagation phase factor to the Fourier-transformed array to simulate the effect of light propagating a distance.

7. Perform an inverse Fourier Transform on the modified Fourier-transformed array.

8. Calculate the intensity and phase of the electric field.

9. Plot the intensity of the electric field and the theoretical intensity as a function of position on the detector.

## Usage

To run the script, simply execute the each section of the notebook

The script will display a plot of the simulated intensity of the diffracted light and the theoretical intensity as a function of position on the detector.

## Note

There are some commented-out lines of code that would write the calculated data to a file. These lines are currently not executed. If you wish to save the data to a file, you can uncomment these lines.
