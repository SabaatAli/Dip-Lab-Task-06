# Dip-Lab-Task-06
# Lab Task Overview: Digital Image Processing
# 1. Core Functionalities
The notebook implements several fundamental image processing operations using OpenCV, NumPy, and Matplotlib. The primary goal is to decompose an image into its frequency components—low and high frequencies—to understand the structural details of digital images.

# 2. Technical Working & Implementation
Library Initialization: The environment is set up by importing cv2 for image processing, numpy for mathematical array operations, and matplotlib.pyplot for visualization.

Image Loading: An image (specifically 'building.jpg') is loaded into the workspace in grayscale mode using cv2.IMREAD_GRAYSCALE.

# Frequency Analysis:

Low-Frequency Extraction: This captures the smooth areas and overall structure of the image, often achieved through blurring or low-pass filtering.

High-Frequency Extraction: This identifies sharp transitions, edges, and fine details. It is typically derived by subtracting the low-frequency component from the original image.

# Visualization:
The results are displayed in a side-by-side comparison using plt.subplot, allowing for a clear visual distinction between the original image, its low-frequency version, and its high-frequency (edge-dominant) version.

# 3. Key Code Logic
The following logic is central to the task's operation:

Read Image: cv2.imread(path, cv2.IMREAD_GRAYSCALE).

Process Components: Segregating pixel data into frequency-based images.

Output Generation: Using plt.imshow() with the gray colormap to render the processed matrices back into viewable images.
