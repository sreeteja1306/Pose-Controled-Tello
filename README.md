# Bodypose controlled tello
 Control Tello using MediaPipe's Body Pose 

## Creating Own Pose Trainng dataset
 create a video in certain pose and convert the video into frames for using `videos2frames.py` 

## Training
Training is a two stage process first obtain key points for each frame and save it into a csv as features using `my_pse_train.py` and then use the csv to train a KNN model to associate the pose with the action using `knncsv.py`

## Testing
Test your knn model using `PoseModule.py`

## Tello Controling 

Connect Tello to you system and send control signals to tello using `drone_pose_control.py` 