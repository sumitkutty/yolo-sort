# yolo-sort
An implementation of object tracking coupled with object detection to detect and track people in CCTV footage.

## Objective
##### Detect and track all people in the CCTV Frame 
###### Add clash detection if people clash with each other.


### Method:
##### Detection and Tracking
* yolov5 is used for object detection. SORT is used for object tracking.

##### Clash Detection
* If 2 people in the frame clash for a single frame, a 1-frame alert is raised by the changing their respective bounding boxes to a specific color.
* If 2 people in the frame clash for more than 5 frames, a 5-frame alert is raised by the changing their respective bounding boxes to a another color.


