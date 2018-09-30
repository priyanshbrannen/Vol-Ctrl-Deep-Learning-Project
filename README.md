# Volume Control with Dynamic Hand Gesture Recognition using Deep Learning Model

YOLOv2 (aka YOLO9000)
YOLO9000 is a high speed, real time detection algorithm that can detect over 9000!(object categories)

Step 1: Requirements
--> Py 3.5
--> TF
--> OpenCV
--> Cython
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
--> from there, open a cmd window
--> use command: python flow --model cfg/tiny-yolo.cfg --load bin/yolov2.weights --demo videofile.mp4 --gpu 1.0 --saveVideo
--> videofile.mp4 is the name of the your video
--> Note: If you do not have the GPU ver of TF, leave off the --gpu 1.0
--> --saveVideo indicates to save a name video file, which has the boxes around the objects.


Error 1:
 Microsoft Visual C++ 14.0 is required. Get it with "Microsoft Visual C++ Build Tools": http://landinghub.visualstudio.com/visual-cpp-build-tools
 
Solution: https://download.microsoft.com/download/5/f/7/5f7acaeb-8363-451f-9425-68a90f98b238/visualcppbuildtools_full.exe?fixForIE=.exe.

To avoid Microst Vsual C++ 14.0 error
	install Visual C++ 2015 update 3 then rc.exe fetal error 

add this to your PATH environment variables:

    C:\Program Files (x86)\Windows Kits\8.0\bin\x86

Copy these files:

    rc.exe
    rcdll.dll

From

    C:\Program Files (x86)\Windows Kits\8.0\bin\x86

To

    C:\Program Files (x86)\Microsoft Visual Studio 11.0\VC\bin

