
We have primary used python language for preprocessing and analysis data for plotting different graphs such as bar chart, confusion matrix etc.
For Manual Annotation Misclassification analysis following code was used for face detection, head pose estimation, and pupil detection.
##Face Detection:
We have created our own face detector by trianing a model on a more than 365 participants face data (Data was used from different gaze dataset consists face image data such as DGW, D-Gaze DG-unicamp, ET-DGaze etc.)  using YOLOV4. It is difficult to upload the trained weights (because of larger size) here so only testing file is given with some detected sample image. The original yolov4 was taken from the following link.
For training and testing custom face detector 1600 and 400 images were used respectively.
https://docs.ultralytics.com/models/yolov4/

In our study face detector was used to obtain the face bounding box coordinate which was further used for head pose Estimation.
![frame1](https://github.com/user-attachments/assets/a78a040a-fc41-47ca-a6dc-5fbea5982746)
Fig.1 Face bounding box.


##Headpose Estimation:
In this study head pose was measured in terms of Euler Angle (Yaw, Pitch, Roll as shown in Fig.2 represent by different color) using Hopenet Algorithm. Details of Hopenet is given in original github given in the following Link.
https://github.com/natanielruiz/deep-head-pose

![Picture1](https://github.com/user-attachments/assets/14d4e9ff-c7b1-4342-92ba-7856d2cb60c2)
Fig.2 Face bounding box and headpose.

We have also upload a folder Headpose_Estimation in which face was detected using Yolov4 custom made face detector and further face detected coordinate was used for headpose estimation.  
##Pupil Detection:
Pupil was detected using  pupil detector. Python code of pupil detection originally present in the following link.
https://github.com/pupil-labs/pupil-detectors

![image](https://github.com/user-attachments/assets/278771f7-d9be-4350-a0f8-c1e48cb9198f)
Fig. 3 Detected Pupil

Folder Pupil_Detection contain modified code of pupil detection which was original given in the above link. 
