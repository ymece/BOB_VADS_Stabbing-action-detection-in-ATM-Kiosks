#  STABBING ACTION DETECTION IN ATM KIOSKS
We have developed two prototypes using the state-of-the-art Deep learning architecture (published by us) and another one using Microsoft Azure-custom vision object detection model

Prototype 1:
We have developed a GUI to detect the abnormal activitiy of stabbing with knife inside ATM and bank premises using the State-of-The Art framework:GMM, YOLOV5 and Lucas Kanade Motion Estimation

# ENVIRONMENT SETUP
Python(3.6.8)

Jupyter notebook
  # Requirements
!pip install CV2

!pip install SYS

!pip install NUMPY

!pip install GLOB

!pip install PIL

!pip install tkinter

!pip install tkvideo

!pip install Torch


# RUN INSTRUCTIONS

1.Install all the required libraries and Import the ATM folder in jupyter notebook

2.Run the GUI.ipynb file in jupyter notebook

3.A tkinter window pops up

![image](https://user-images.githubusercontent.com/53227455/199953814-aa23a221-23f7-4420-a2d8-8da5d2dbc682.png)

First, Perform the foreground_segmentation which uses GMM (Gaussian Mixture Model) 

  1.The output is stored in yolov5 folder 
	
Next, Perform the knifeinhand detection using yolov5

  2.The output is stored in yolov5/runs/detect/exp 
	
Finally, to perform Lucas Kanade method for motion estimation, upload the output of yolov5

#  STABBING ACTION DETECTION IN ATM KIOSKS
Prototype 2:
We have developed a GUI to detect the abnormal activitiy of stabbing with knife inside ATM and bank premises using Microsoft Azure - custom vision object detection model(with alarm system)
We have used a custom dataset with knife in hand (for training and prediction) collected from various resources.

# ENVIRONMENT SETUP
Python(3.6.8)

Jupyter notebook

  # Requirements
  
  pip install tensorflow
  
  pip install pillow
  
  pip install numpy
  
  pip install opencv-python
  
  # Run Instructions
   
   Unzip the downloaded folder and open the detect.ipynb file 
   
   A tkinter windoe pops up
   
   Select the required input from input folder 
   
   The prediction result is displayed in the terminal and gets saved as knife_detection.mp4 file
   
   When knife is detected, the alarm will alert.
