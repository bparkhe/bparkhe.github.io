## Advanced Lane Finding Project	

**Project description:** 
This project was executed as a part of my Udacity Self Driving Car Nanodegree. The below project was part of module 2 where we improve upon our previous implementation of lane finding. The previous algorithm had problems with detecting higher order curvatures and detecting lane lines on a concrete road. I used indvidual images to show the steps and then the implemtation of the final video is included as well.

<img src="images/auto_bot/straight_lines1.jpg?raw=true"/>
---
### Undistort and perspective transform
First we preform an undistort to account for distortion due to the camera lenses. This the first and the most basicestep before we proceed with curvature calculations

<img src="images/auto_bot/test1_undist.jpg?raw=true"/>

Then I use a perpective transform to convert this image into a birds-eye view of the lane. The rendintion is not always accurate, but we check for this by looking at the perspective transform of a near straight lane. Its transform shoould be close to vertical lines.

<img src="images/auto_bot/straight_lines1_mask.jpg?raw=true"/>

<img src="images/auto_bot/straight_lines1_warped.jpg?raw=true"/>

---
### Color and Gradient Thresholds

By applying HLS color gradients and Sobel Gradient Transform we get the below image where we can easily extract the lanes for further processing.

<img src="images/auto_bot/test1_color_sobel_threshold.jpg?raw=true"/>

---
### Curvature Measurement
After applying the perspective transform and color threshold, we get a image similar to the one below. This is for a section of the the lane where there were cracks in the concrete and shadows from nearby trees. Hovewer, these are ignored and only the red and blue colored pixles are used for lane identification. 

A 2nd order polynomial is fitted to these points (yellow). A spline can also be fitted for roads with uneven curves.

<img src="images/auto_bot/test7.jpg?raw=true"/>

<img width="350" src="images/auto_bot/output_test1_polynomial.jpg?raw=true"/>

---
### Final Output
<video width="640" height="480" controls>
  <source src="images/auto_bot/project_video_output.mp4" type="video/mp4">
</video>

