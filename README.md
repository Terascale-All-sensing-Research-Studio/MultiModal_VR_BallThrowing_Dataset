# Multimodal Virtual Reality (VR) Ball Throwing Dataset for VR Biometrics

## Contents
[Description](#description)

[Contributors](#contributors)

[Overview of Dataset](#overview-of-dataset)

## Description
We provide a multimodal dataset for VR biometrics comprising of 41 participants performing a ball throwing task in VR, while simultaneously being recorded using an external camera. Each participant provides data using the headset and hand controllers of the Meta Quest, HTC Vive, and HTC Vive Cosmos. During the interaction, we capture an external profile video of the dominant side of the participant using a GoPro Hero 7 camera. Participants perform the ball throwing activity in VR for 10 trials in each session. We record data for 6 sessions, where each session is separated by at least 1 day and participants provide data for 2 sessions using each VR system. Data is first captured using the Meta Quest, then the HTC Vive, and finally from the HTC Vive Cosmos. In each VR system we capture position and orientation data from the headset and two hand controllers as well as the trigger value from the dominant hand controller. We provide cropped videos from the GoPro at 60 frames per second along with OpenPose and MMPose body keypoints. Our data provides the Self Identified Gender, Age, Height (in), Weight (lb), Writing Hand, Throwing Hand, Throwing Sport Experience, Type of Throwing Sport, and VR Experience as user demographics for each participant. We also provide session metadata recorded as the temporal difference between each session for each participant.  

**Example Headset and Hand Controller Trajectories From Dataset**

![](/figs/vrmotion/trajectories.png)

**Example Cropped Profile View GoPro Video With MMPose and OpenPose Body Keypoints From Dataset**

![](figs/videos/examplevideos.gif)

## Contributors
Mingjun Li, Natasha Kholgade Banerjee,  Sean Banerjee

[Terascale All-sensing Research Studio](https://tars-home.github.io)

## Overview of Dataset
The dataset is organized into the following folders:

| FolderName | SubFolders | DataType | Contents |
|--|--|--|--|
| [capturetimedata](/capturetimedata) | None | CSV | [capturetimedata.csv](/capturetimedata/capturetimedata.csv): A CSV file that provides the temporal difference (in days) between successive sessions for each of the 41 participants. |
| [croppedvideos](/croppedvideos) | [cosmos_day1](/croppedvideos/cosmos_day1), [cosmos_day2](/croppedvideos/cosmos_day2), [quest_day1](/croppedvideos/quest_day1), [quest_day2](/croppedvideos/quest_day2), [vive_day1](/croppedvideos/vive_day1), [vive_day2](/croppedvideos/vive_day2) | MP4 | Each subfolder (e.g. cosmos_day1) represents the name of the VR system and a numeric for the first or second day of capture. Within each of these subfolders (e.g. cosmos_day1) there are 41 subfolders titled in the format XXX_SystemDay, where XXX is a 3 digit participant ID, System is Cosmos, Quest, or Vive, and Day takes a value of 1 or 2 (e.g. 101_Cosmos1). Inside these 41 subfolders (e.g. 101_Cosmos1) there are 10 cropped GoPro videos numbered 0.mp4 to 9.mp4 for each of the 10 throws for that session. All cropped videos are at 60 frames per second. |
| [demographics](/demographics) | None | CSV | [demographics.csv](/demographics/demographics.csv): A CSV file that provides the following demographics: Self Identified Gender, Age, Height (in), Weight (lb), Writing Hand, Throwing Hand, Throwing Sport Experience, Type of Throwing Sport, and VR Experience for each of the 41 participants. |
| [mmpose_results](/mmpose_results) | [cosmos_day1](/mmpose_results/cosmos_day1), [cosmos_day2](/mmpose_results/cosmos_day2), [quest_day1](/mmpose_results/quest_day1), [quest_day2](/mmpose_results/quest_day2), [vive_day1](/mmpose_results/vive_day1), [vive_day2](/mmpose_results/vive_day2) | JSON | Each subfolder (e.g. cosmos_day1) represents the name of the VR system and a numeric for the first or second day of capture. Within each of these subfolders (e.g. cosmos_day1) there are 41 subfolders titled in the format XXX_System_Day, where XXX is a 3 digit participant ID, System is Cosmos, Quest, or Vive, and Day takes a value of 1 or 2 (e.g. 101_Cosmos1). Inside these 41 subfolders (e.g. 101_Cosmos_1) there are 10 JSON files for the body pose extracted using the MMPose toolbox numbered 0.json to 9.json for each of the 10 throws for that session. |
| [openpose_results](/openpose_results) | [cosmos_day1](/openpose_results/cosmos_day1), [cosmos_day2](/openpose_results/cosmos_day2), [quest_day1](/openpose_results/quest_day1), [quest_day2](/openpose_results/quest_day2), [vive_day1](/openpose_results/vive_day1), [vive_day2](/openpose_results/vive_day2) | JSON | Each subfolder (e.g. cosmos_day1) represents the name of the VR system and a numeric for the first or second day of capture. Within each of these subfolders (e.g. cosmos_day1) there are 41 subfolders titled in the format XXX_System_Day, where XXX is a 3 digit participant ID, System is Cosmos, Quest, or Vive, and Day takes a value of 1 or 2 (e.g. 101_Cosmos1). Inside these 41 subfolders (e.g. 101_Cosmos_1) there are 10 sub-subfolders named after each trial named in the format Y/json, where Y ranges from 0 to 9 for the 10 trials. Within these sub-subfolders named Y/json are 180 JSON files corresponding to 180 video frames. Each JSON file contains the body pose extracted using the OpenPose toolbox. |
| [vrmotions](/vrmotions) | None | NPY | The folder contains 6 NumPy files Cosmos1.npy, Cosmos2.npy, Quest1.npy, Quest2.npy, Vive1.npy, Vive2.npy representing each of the 3 VR systems and 2 days of capture per system. These files represent NumPy arrays with the shape (41, 10, 135, 21), where the first dimension covers the 41 participants, the second the 10 throws, the third the 135 timestamps for each throw, and the fourth the 21 total features representing the position, orientation, and trigger value for the headset and hand controllers. |


