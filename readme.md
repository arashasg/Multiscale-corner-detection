# Multiscale-corner-detection
## Corner Detection(multiscale_corner_detection.py)
We have 3 images saved to the files kntu1.jpg , kntu2.jpg and kntu4.jpg . All images
are of the same size (800 by 800 pixels). However, the logo in images kntu2.jpg and
kntu4.jpg are respectively 2 and 4 times smaller than the logo in kntu1.jpg.
<p float="left" align="center">
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/Logos.PNG" />
</p>
We want to find the correct window size for detecting Harris corners in each of these
images. For this, we run the Harris corner detection algorithm for window sizes 2, 4,
8, 16, 32 and 64 for each image. We know that the image have 78 corners and We want to 
find the smallest harris window size that correctly detects 78 corners. We compare the scale of each Two
images by comparing their corresponding harris window size which detects 78 corners.

## Corner Detection using Pyramid(Multiscale corner detection with Image Pyramid.py)
An alternative approach is to keep the Harris window size fixed and change the
image size instead. In the following, we use a fixed window size (win_size = 4) and
run the corner detection algorithm for different image sizes in an image pyramid.


### output:
The output of both codes is the same and only the approach is different.
<p float="left" align="center">
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output1.PNG" width="600px" height="350px" />
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output2.PNG" width="600px" height="350px" />
</p>

## Polygon corner detection with connected components(Polygons Corner Detection.py)
First, we separated each connected component. Afterward, we 
applied harris corner detection to each one of connected components. As harris cornerner detector finds
many corner near each corner of the polygon, we applied connected component again to find the real number of corners.

### input:
<p float="left" align="center">
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/polygons.jpg" width="600px" height="350px" />
</p>

### output:
<p float="left" align="center">
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output3.PNG" width="350px" height="350px" />
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output4.PNG" width="350px" height="350px" />
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output5.PNG" width="350px" height="350px" />
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output6.PNG" width="350px" height="350px" />
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output7.PNG" width="350px" height="350px" />
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output8.PNG" width="350px" height="350px" />
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output9.PNG" width="350px" height="350px" />
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output10.PNG" width="350px" height="350px" />
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output11.PNG" width="350px" height="350px" />
  <img src="https://github.com/arashasg/Multiscale-corner-detection/blob/master/Images/output12.PNG" width="350px" height="350px" />
</p>
