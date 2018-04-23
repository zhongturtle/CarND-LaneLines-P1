# **Finding Lane Lines on the Road** 

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[solidwhite]: ./test_images_output/solidWhiteRight_result.jpg
[solidYellowLeft]: ./test_images_output/solidYellowLeft_result.jpg

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps.
First, I converted the images to grayscale, then I apply Gaussian smoothing to blur the image.
After these two thing , I do the Canny algorithm to detect the edge.
After all , I create maked edges image 
At last step , I use hough_line to make the image with line on it and use the function called weighted_img to adjust the image.
In order to draw a single line on the left and right lanes, I modified the draw_lines() function by detect the slpoe of both side which maybe a line 
Here is the result:

![alt text][solidYellowLeft]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
