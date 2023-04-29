# Image Processing Techniques to Extract Targeted Image Region
The above code uses various image processing techniques to extract a targeted image region from an input image. The following steps were used to achieve this:

1. **Image Resize**: The input image was resized to a smaller size to make it easier to process. 

2. **Noise Removal**: The image was converted to grayscale and then blurred using a Gaussian filter to remove noise.

3. **Edge Detection**: The edges in the image were detected using the Canny edge detection algorithm.

4. **Countour Extraction**: The contours of the edges in the image were extracted using OpenCV's `findContours` function. The contours were then sorted in descending order based on their area and the contour with four corners was selected.

5. **Contour Reordering**: The corners of the selected contour were reordered to obtain a fixed order.

6. **Perspective Transformation**: The input image was transformed to a fixed-size screen using OpenCV's `getPerspectiveTransform` function.

The final output image was the extracted targeted image region.

The code has been documented using inline comments to explain each step in detail. Additionally, `matplotlib` has been used to visualize the intermediate steps of the image processing techniques.
