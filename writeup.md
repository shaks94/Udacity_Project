# **Finding Lane Lines on the Road**

## Writeup
----
1) ##### This project aim to display the skill set after completion of project "Finding Lane Lines on the Road as first project in the nano degree"
2) ##### A pipeline is made in order to get the expected output result's 

## Reflection
---
* ### description of pipeline  
   1) The pipeline start from the function `process_image()` 
   2) Piepline consist of 5 set of step's 
        * Reading image 
        * Grayscale the image in order to obtain one color channel
        * Appling gaussian blur in order to achieve the _smooth_ image and reduce _noise_
        * Appling the Canny transform in order to achieve  the _edges_ of the Lane
        * Making region_of_interest in order to get _masked image_
            * ###### It mainly use **fillPoly and bitwise_and** function from cv2 library
        * Using hough_lines to **finds lines in a binary image**    
            * ###### it further use **draw_lines** function where Lane get red color and thickess which is                displayed in the code 
        * And at the end **weighted_img** function  used to _Calculates the weighted sum of two arrays._



2) ### Suggest possible improvements to your pipeline
    1) Increase the thickness from 2 to 10 for better guidance 
    2) slope detection in solution in coming day's 


