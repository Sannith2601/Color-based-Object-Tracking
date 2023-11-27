# Color based Object-Tracking

object tracking based on color using HSV (Hue Saturation Value)

Formulas used here

* Minimum Enclosing Circle :

      ((x, y), radius) = cv2.minEnclosingCircle( countourArea )
* Moments to find center of the Area :

     Image moments help you to calculate some features like center of mass of the object, area of the object etc.
     
     M = cv2.moments(c)
     
     center = (int(M["m10"] / M["m00"]), int(M["m01"] / M["m00"]))
     
# This Color Based Object Tracking is Based on SELF-DRIVING-CONCEPT

 * If the particular Color is goes long, then it shows "Front"
 
 * If the particular Color is comes close, then it shows "Stop"
 
 * If the particular Color is goes at the right corner, then it shows "Right"
 
 * If the particular Color is goes at the left corner, then it shows "Left"
 
 
# Steps :
     
     * Reading frame from camera
     
     * pre-processing image
     
     * Finding contours
     
     * Drawing minimum enclosing circle
     
     * Finding centre of contour Area 
     
     * Drawing circle & centre
     
     * Direction based on radius & position
     
     * Run the code and display the output
     
