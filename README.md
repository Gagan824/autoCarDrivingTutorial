# autoCarDrivingTutorial

## Objective:
### * Objective is just to make the car automatic, system will detect the lanes on the road, according to the lane system will predict curve and center offset from the car. And also warn you for the alert like if any car comes near to your car then it will warn you and in case when ther is any traffic sign on the road, it will warn you as per the detected sign.
## Overview
##### 1. Model will take the image or frame as the input
##### 2. First we have calibrated our camera on chess board images to get the camera matrix and distortion factors.
##### 3. After the calibration part once we have camera matrix and diistortion factors then we can go with the undistortion of the input image.
##### 4. After taking the input, model will apply some thresholding transformation like LUV, HLS thresholding etc..
##### 5. Then model will combine all the result from all the thresholding transformations.
##### 6. The main objective of doing above steps is to detect the optimal edges for the lane on the road.
##### 7. Step3 will give the binary image.
##### 8. Once we will have binary image then we will apply perspective projection to warp the image into an aerial view.
##### 9. At step8 we will get the binary warped image then from the image will try to find the points of the lanes.
##### 10. Then model will try to create the line or polygon using those points to draw the lane.
##### 11. There are two other models:
###### 11.1. Object Detection Model: Model(yolov5) will detect the vehicles, person and traffic signs alomng with the traffic light on the road.
###### 11.2. Depth Model: Model(monodepth2) will calculate the depth of the frame to calculate the distance to other objects.

<br />
<br />
<br />
<br />
###########################################################################################################

###### NOTE: This is just for trial purpose if you need complete code then you can contact me on my gmail(guptagagan824@gmail.com).

###########################################################################################################

