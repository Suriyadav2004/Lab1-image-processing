1. Introduction
This lab focuses on fundamental techniques in image processing using Python. The objective is to understand various image manipulation methods and their applications in analyzing and enhancing images.

Objectives
To perform basic image processing tasks such as loading, displaying, and modifying images.
To explore various image filters and transformations.
To analyze the results of different processing techniques.

2. Tools and Libraries
The following libraries were utilized during the lab:

OpenCV: For image manipulation and analysis.
NumPy: For numerical operations on image data.
Matplotlib: For displaying images and results.
Installation
bash
Copy code
pip install opencv-python numpy matplotlib

3. Methodology
3.1 Loading Images
Images were loaded from the local directory using OpenCV:

python
Copy code
import cv2

image = cv2.imread('path_to_image.jpg')
3.2 Displaying Images
Images were displayed using Matplotlib:

python
Copy code
import matplotlib.pyplot as plt

plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
plt.axis('off')
plt.show()

3.3 Image Processing Techniques
Various techniques were applied, including:

Grayscale Conversion:

python
Copy code
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
Blurring:

python
Copy code
blurred_image = cv2.GaussianBlur(image, (5, 5), 0)
Edge Detection:

python
Copy code
edges = cv2.Canny(image, 100, 200)

3.4 Applying Filters
Different filters were applied to enhance images. Examples include:

Gaussian Blur
Median Filtering

4. Results
The results of the processing techniques were visually analyzed. Below are some example outputs:

Original Image:
Grayscale Image:
Blurred Image:
Edge Detection:

5. Discussion
The application of different image processing techniques showed varied results. Grayscale conversion is useful for simplifying the image, while edge detection highlighted significant features. Blurring can reduce noise but may also obscure important details.

Limitations
Some techniques may not be effective on all types of images.
The choice of parameters (e.g., kernel size) significantly impacts results.

6. Conclusion
This lab provided a foundational understanding of image processing techniques. The ability to manipulate images using programming enhances the potential for applications in fields such as computer vision, photography, and data analysis.

7. References
OpenCV Documentation: opencv.org
NumPy Documentation: numpy.org
Matplotlib Documentation: matplotlib.org
