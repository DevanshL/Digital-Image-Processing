# Image Sharpening Using Prewitt Filter
This repository contains code for sharpening an image using the Prewitt filter technique.

## Overview
The objective of this project is to sharpen an input image using the Prewitt filter. The sharpening process involves enhancing the edges in the image to improve its clarity and definition.

## Features
- Find the edge image of the input image.
- Sharpen the image using the Prewitt filter.
- Choose the sharpening effect by manually adjusting the parameter c.

## Instructions

1. **Download Input Image:**

- Obtain the input image you want to sharpen. You can use any online source or provide your own image.

2. **Convert to Grayscale:**

- Convert the input image to grayscale. This step ensures that the image is in a single-channel format for processing.

3. **Apply Prewitt Filter:**

- Implement the Prewitt filter to find the gradient of the grayscale image. Use separate convolution operations for horizontal and vertical gradients.

4. **Compute Gradient Magnitude:**

- Calculate the gradient magnitude by combining the horizontal and vertical gradients using the formula: gradient_magnitude = sqrt(gradient_x**2 + gradient_y**2).
5. **Thresholding:**

- Apply a threshold to the gradient magnitude image to create an edge mask. Set pixels with gradient magnitude greater than a predefined threshold T to 1 (edge) and others to 0 (non-edge).
6. **Sharpening:**

- Implement the sharpening operation using the formula: sharpened_image = input_image + c * edge_mask, where c is a manually chosen parameter to control the sharpening effect.

7. **Visualize Results:**

- Visualize the original input image, edge mask, and output image 

8. **Adjust Parameters:**

- Experiment with different values of the threshold T and the sharpening parameter c to achieve the desired sharpening effect and edge detection accuracy.

Clone the repository:

   ```bash
   git clone https://github.com/DevanshL/Digital-Image-Processing/tree/main/Assignment-03
   ```
