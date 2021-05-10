# Aruco-tag-cameraCalibandPose
This task was assigned to me as part of the selection process for the Autonomous Ground Vehicle Research Group software team at IIT Kharagpur.
## Key Learnings
1. Camera Calibration - Extrinsic and Intrinsic parameters
2. Importance of Fiducial Markers
3. Pose Estimation

## Challenges and Workarounds
### Getting Roll, Yaw and Pitch from Rotation Vector
Rotation, Translation matrices are used to transform from the world coordinate system to camera coordinate system. Rotation matrix used for this is usually a matrix of 
dimension = (3, 3).
But the output (rvec) I got from cv2.calibrateCamera() was a vector of dimension = (1,3). Later I found out that rvec is a Rodrigues vector and we need OpenCV's Rodrigues function to convert this into a rotation matrix of dimension = (3,3)

## Conclusion
This task was really fun to do! I also learnt a lot about AruCo Tags and Camera calibration. 
