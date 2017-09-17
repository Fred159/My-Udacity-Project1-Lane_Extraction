# **Finding Lane Lines on the Road** 

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Code was failed in challenge videos
* referenced methodology from mvirgo


### Reflection

### 1. My strategy

My pipeline include 10 steps.
1. Install essential libs and import libs
2. Define the functions and add extra functions
3. Read image
4. Change into gray
5. Bluring the image with gaussian
6. define ROI
7. Use hough function to extract the endpoints of the line in image
8. Seperate the lines based on the slope
9. Average the slopes and lines, and calculate the final lines which should weighted in origin image
10. put the extracted lines image to the origin image.

### 2. Short coming
The code is not stable. It is only can work in good road condition. Even in good condition it is still not performed good enough.
And the tuning should be done more times.
The region and other parameters are all constant. It will causes many issues in complex environment.
I don't know why but my code can't run with challenge videos. 

### 3. Suggest possible improvements to your pipeline

Calculation of the mean value of the slope and lines end position could be improved.
Constant value should be set to variable and change based on the ROI and road condition.
Challenge video's problem can be solved by saperate the yellow lines and white lines.
