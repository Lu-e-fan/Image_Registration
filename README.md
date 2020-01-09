**Included in this repository is a zip containing python script with test and demo images**

In this project the goal is to implement an end-to-end image registration system. The system
will be capable of aligning image pairs to a common coordinate system. The project is
divided into different steps (roughly one for each module of the system). 

Functions used in script:<br/>
        --featureMatching(image1, image2)<br/>
        --DLT_Standard(p1,p2)<br/>
        --DLT_Normalized(p1,p2)<br/>
        --cv.findHomography<br/>
        --registerImage()<br/>
  
**Algorithm Brief Description:** The input of our program takes in two images and gets fed into SIFT for feature extraction and correspondence. After sorting out the good corresponding points, those points are sent into DLT to compute the Homography matrix. RANSAC is also applied as an alternative to "clean up" the feature points and help enhance DLT performance. Homography matrices are then applied onto one of the input images to compare with the other for evaluation. Images are rescaled to be stitched together for visualization.  
 
