# **Lane-Detection**
Lane detection is a critical component of self-driving cars and autonomous vehicles.With it the vehicle will know where to go and avoid the risk of running into other lanes or getting off the road. This can prevent the driver/car system from drifting off the driving lane.
## Dependencies:
Python version 3.7 <br>
opencv-python <br>
numpy <br>
matplotlib <br>

## Getting Started
Using Canny Edge detection algorithm and Hough Transform method
This is our image:
<p align="center">
<img src = "https://github.com/anushkagarg5653/Lane-Detection/blob/master/Images/test_image.jpg" width="500" height="300">
</p>

### 1. Grayscaling
Grayscale is a range of shades of gray without apparent color. The darkest possible shade is black, which is the total absence of transmitted or reflected light. The lightest possible shade is white, the total transmission or reflection of light at all visible wavelength. This process helps in increasing the contrast of the lanes, to be able to distinguish them from the rest of the image.
Image after applying grayscale
<p align="center">
<img src = "https://github.com/anushkagarg5653/Lane-Detection/blob/master/Images/GrayScale.JPG" width="500" height="300">
</p>

### 2. Gaussian Blur
The Gaussian blur function is applied on the grayscaled image. It is a widely used effect in graphics software, typically to reduce image noise and reduce detail.
Image after applying Gaussian blur
<p align="center">
<img src = "https://github.com/anushkagarg5653/Lane-Detection/blob/master/Images/blur.JPG" width="500" height="300">
</p>

###  Canny Edge Function
Canny edge detection is a multi-step algorithm that can detect edges with noise supressed at the same time. Smooth the image with a Gaussian filter to reduce noise and unwanted details and textures.

<p align="center">
<img src = "https://github.com/anushkagarg5653/Lane-Detection/blob/master/Images/Canny.JPG" width="500" height="300">
</p>

###  Hough Transform
The Hough transform is a feature extraction technique used in image computer vision. The purpose is to find imperfect instances of objects within a certain class of shapes by a voting procedure.
<p align="center">
<img src = "https://github.com/anushkagarg5653/Lane-Detection/blob/master/Images/Cropped.JPG" width="500" height="300">
</p> 


After applying all the above concept, we finally get our required edges of lane lines traced on black pixels, which we then merge with our original image by weighted additions, and voila! we have detected the lane lines.
Our final merged image, indicating lane lines will look like this:
</a>
</p>

