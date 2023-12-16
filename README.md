# De-Smoking-De-Hazing-Algorithm

This project is a Python implementation of a single image dehazing algorithm. The purpose of the code is to enhance the visibility of images that are affected by atmospheric haze or fog. The dehazing process involves estimating the atmospheric light, calculating the transmission map, and then using this information to remove the haze from the original image.

# Here are the key components and features of the project:

# Image Dehazing Class (image_dehazer):
The image_dehazer class contains methods for estimating atmospheric light, calculating the transmission map, and removing haze from an input image.
The dehazing process involves techniques such as atmospheric light estimation, boundary constraints, filtering, and optimization using a regularization parameter.

# Parameters:
The dehazing algorithm is configurable with several parameters, including window sizes for atmospheric light estimation and boundary constraints, constants C0 and C1, regularization parameters, and parameters related to the optimization process.

# Filter Bank:
The project uses a set of Kirsch filters for image filtering. These filters are employed to calculate the weighting function, which is used in the dehazing optimization process.

# Optimization Process:
The optimization process involves iteratively refining the transmission map using a set of Kirsch filters and a regularization parameter. The goal is to enhance the image by reducing the impact of haze.

# Haze Removal:
The final result of the dehazing process is a haze-corrected image, where the atmospheric haze has been effectively reduced or removed.
Command-Line Interface (remove_haze function):

The project includes a function named remove_haze that can be used directly. It takes an input image and optional parameters, and it returns the dehazed image and the corresponding haze transmission map.
Visualization:

The code includes an option (showHazeTransmissionMap) to display the haze transmission map during the optimization process.

# Usage:
Users can utilize the remove_haze function by providing an input image and adjusting the parameters to suit their specific needs.
Demonstration:

The code includes a demonstration of the dehazing process on an example image, providing a practical example of the algorithm in action.

# OpenCV Integration:
The project leverages the OpenCV library for image processing tasks, including filtering and convolution operations.
