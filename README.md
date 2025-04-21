# MultiModal VR BallThrowing Dataset for VR Biometrics

## Contents
[Description](#description)

[Contributors](#contributors)

[Overview of Dataset](#overview-of-dataset)

## Description

## Contributors
Mingjun Li, Natasha Kholgade Banerjee,  Sean Banerjee

[Terascale All-sensing Research Studio](https://tars-home.github.io)

## Overview of Dataset
The dataset is organized into the following folders:

| FolderName | SubFolders | DataType | Contents |
|--|--|--|--|
| capturetimedata | None | CSV | capturetimedata.csv: A CSV file that provides the temporal difference (in days) between successive sessions for each of the 41 participants. |
| croppedvideos | cosmos_day1, cosmos_day2, quest_day1, quest_day2, vive_day1, vive_day2 | MP4 | Each subfolder (e.g. cosmos_day1) represents the name of the VR system and a numeric for the first or second day of capture. Within each of these subfolders (e.g. cosmos_day1) there are 41 subfolders titled in the format XXX_SystemDay, where XXX is a 3 digit participant ID, System is Cosmos, Quest, or Vive, and Day takes a value of 1 or 2 (e.g. 101_Cosmos1). Inside these 41 subfolders (e.g. 101_Cosmos1) there are 10 cropped GoPro videos numbered 0.mp4 to 9.mp4 for each of the 10 throws for that session. |
| demographics | None | CSV | demographics.csv: A CSV file that provides the following demographics: Self Identified Gender, Age, Height (in), Weight (lb), Writing Hand, Throwing Hand, Throwing Sport Experience, Type of Throwing Sport, and VR Experience for each of the 41 participants. |
| mmpose_results | cosmos_day1, cosmos_day2, quest_day1, quest_day2, vive_day1, vive_day2 | JSON | Each subfolder (e.g. cosmos_day1) represents the name of the VR system and a numeric for the first or second day of capture. Within each of these subfolders (e.g. cosmos_day1) there are 41 subfolders titled in the format XXX_SystemDay, where XXX is a 3 digit participant ID, System is Cosmos, Quest, or Vive, and Day takes a value of 1 or 2 (e.g. 101_Cosmos1). Inside these 41 subfolders (e.g. 101_Cosmos1) there are 10 JSON files for the body pose extracted using the MMPose toolbox numbered 0.json to 9.json for each of the 10 throws for that session. |
| openpose_results | cosmos_day1, cosmos_day2, quest_day1, quest_day2, vive_day1, vive_day2 | JSON | Each subfolder (e.g. cosmos_day1) represents the name of the VR system and a numeric for the first or second day of capture. Within each of these subfolders (e.g. cosmos_day1) there are 41 subfolders titled in the format XXX_SystemDay, where XXX is a 3 digit participant ID, System is Cosmos, Quest, or Vive, and Day takes a value of 1 or 2 (e.g. 101_Cosmos1). Inside these 41 subfolders (e.g. 101_Cosmos1) there are 10 JSON files for the body pose extracted using the OpenPose toolbox numbered 0.json to 9.json for each of the 10 throws for that session. |
| vrmotions | None | NPY | The folder contains 6 NumPy files cosmos_day1.npy, cosmos_day2.npy, quest_day1.npy, quest_day2.npy, vive_day1.npy, vive_day2.npy representing each of the 3 VR systems and 2 days of capture per system. These files represent NumPy arrays with the shape (41, 10, 135, 21), where the first dimension covers the 41 participants, the second the 10 throws, the third the 135 timestamps for each throw, and the fourth the 21 total features representing the position, orientation, and trigger value for the headset and hand controllers. |


## [Cropped Videos](https://github.com/Terascale-All-sensing-Research-Studio/VR_BallThrowing_Dataset/tree/main/CroppedVideos) 

We include the raw videos from a side view of the participants while they provided data.

## [VR_Motions_Numpy](https://github.com/Terascale-All-sensing-Research-Studio/VR_BallThrowing_Dataset/tree/main/VR_Motions_Numpy)

We also include compressed data obtained from the VR devices during the collection process.

## [mmpose_results](https://github.com/Terascale-All-sensing-Research-Studio/VR_BallThrowing_Dataset/tree/main/mmpose_results)

Uses COCO key points.

Visual examples:
<div align="left">
<img src="https://github.com/Terascale-All-sensing-Research-Studio/VR_BallThrowing_Dataset/blob/main/figs/mmpose_User25_Cosmos1_Session0.gif" width=60% height=60%>
</div>

<div align="left">
<img src="https://github.com/Terascale-All-sensing-Research-Studio/VR_BallThrowing_Dataset/blob/main/figs/mmpose_User28_Cosmos1_Session0.gif" width=60% height=60%>
</div>

### More information of keypoints strategy used in [MMPose](https://github.com/open-mmlab/mmpose/tree/main):
https://github.com/open-mmlab/mmpose/tree/main/mmpose/datasets/datasets/body

## [openpose_results](https://github.com/Terascale-All-sensing-Research-Studio/VR_BallThrowing_Dataset/tree/main/openpose_results_json)

Uses COCO key points.

<div align="left">
<img src="https://github.com/Terascale-All-sensing-Research-Studio/VR_BallThrowing_Dataset/blob/main/figs/User25_Cosmos1_Session0.gif" width=60% height=60%>
</div>

<div align="left">
<img src="https://github.com/Terascale-All-sensing-Research-Studio/VR_BallThrowing_Dataset/blob/main/figs/User28_Cosmos1_Session0.gif" width=60% height=60%>
</div>

## [List of the COCO key points](https://github.com/jin-s13/COCO-WholeBody/tree/master?tab=readme-ov-file)

```bash
0: 'nose',
1: 'left_eye',
2: 'right_eye',
3: 'left_ear',
4: 'right_ear',
5: 'left_shoulder',
6: 'right_shoulder',
7: 'left_elbow',
8: 'right_elbow',
9: 'left_wrist',
10: 'right_wrist',
11: 'left_hip',
12: 'right_hip',
13: 'left_knee',
14: 'right_knee',
15: 'left_ankle',
16: 'right_ankle'
```
