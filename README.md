# Volume Control with Dynamic Hand Gesture Recognition using Deep Learning Model

YOLOv2 (aka YOLO9000)
YOLO9000 is a high speed, real time detection algorithm that can detect over 9000!(object categories)

Step 1: Requirements
--> Py 3.5
--> TF
--> OpenCV
Step 2: Download the Darkflow repository
https://github.com/thtrieu/darkflow

Step 3: Build the Library
--> open cmd & type: python setup.py build_ext --inplace
or
pip install -e .

Step 4: Download the weights file
--> Download the YOLOv2 608x608 weights file here (https://pjreddie.com/darknet/yolo/)
--> There are other weight files you can try if you want.
--> Create a bin folder within darkflow-master folder and put the weights file in the bin folder.

#Processing a video File
--> move the video file into the "darkflow-master" folder
