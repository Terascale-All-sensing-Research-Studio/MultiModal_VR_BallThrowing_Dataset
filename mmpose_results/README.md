## MMPose Body Keypoints

For each participant we use the [croppedvideos](../croppedvideos) to generate [COCO key points](https://github.com/jin-s13/COCO-WholeBody/tree/master?tab=readme-ov-file) using [MMPose](https://github.com/open-mmlab/mmpose/). We generate the following body keypoints: 

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

## Directory Structure
We provide individual directories for each VR system, namely Meta Quest, HTC Vive, and HTC Vive Cosmos, and day. The folder structure is as follows:

+ [cosmos_day1](cosmos_day1): contains individual subfolders for each participant's day 1 throw using the HTC Vive Cosmos. The subfolder is named as XXX_Cosmos_1, where XXX is a 3-digit participant ID. Each subfolder contains 10 JSON files named 0.json to 9.json for each of the 10 trials for the day. 
+ [cosmos_day2](cosmos_day2): contains individual subfolders for each participant's day 2 throw using the HTC Vive Cosmos. The subfolder is named as XXX_Cosmos_2, where XXX is a 3-digit participant ID. Each subfolder contains 10 JSON files named 0.json to 9.json for each of the 10 trials for the day. 
+ [quest_day1](quest_day1): contains individual subfolders for each participant's day 1 throw using the Meta Quest. The subfolder is named as XXX_Quest_1, where XXX is a 3-digit participant ID. Each subfolder contains 10 JSON files named 0.json to 9.json for each of the 10 trials for the day. 
+ [quest_day2](quest_day2): contains individual subfolders for each participant's day 2 throw using the Meta Quest. The subfolder is named as XXX_Quest_2, where XXX is a 3-digit participant ID. Each subfolder contains 10 JSON files named 0.json to 9.json for each of the 10 trials for the day. 
+ [vive_day1](vive_day1): contains individual subfolders for each participant's day 1 throw using the HTC Vive. The subfolder is named as XXX_Vive_1, where XXX is a 3-digit participant ID. Each subfolder contains 10 JSON files named 0.json to 9.json for each of the 10 trials for the day. 
+ [vive_day2](vive_day2): contains individual subfolders for each participant's day 2 throw using the HTC Vive. The subfolder is named as XXX_Vive_2, where XXX is a 3-digit participant ID. Each subfolder contains 10 JSON files named 0.json to 9.json for each of the 10 trials for the day. 

## Example Cropped Profile View GoPro Video With MMPose and OpenPose Body Keypoints
![](../figs/videos/examplevideos.gif)
