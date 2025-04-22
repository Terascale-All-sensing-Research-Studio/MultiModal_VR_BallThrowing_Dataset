## Capture Time Data

### Contents
[Overview](#overview)

[Data](#data)

[Summary Statistics](#summary-statistics)

### Overview
The file capturetimedata.csv provides time difference (in days) between captures. All participants provided data on the systems in the following order: Quest, Vive, Cosmos. All participants provided data on two days. No two VR systems were used on the same day. The value of **ID** is matched to the same users in the [croppedvideo](../croppedvideos), [mmpose](../mmpose_results), and [openpose](../openpose_results) body pose data folders. The column names are as follows:

+ **Q1Q2Diff**: Difference in days between Quest Day 2 and Quest Day 2
+ **Q1V1Diff**: Difference in days between Quest Day 1 and Vive Day 1
+ **Q1V2Diff**: Difference in days between Quest Day 1 and Vive Day 2
+ **Q1C1Diff**: Difference in days between Quest Day 1 and Cosmos Day 1
+ **Q1C2Diff**: Difference in days between Quest Day 1 and Cosmos Day 2
+ **Q2V1Diff**: Difference in days between Quest Day 2 and Vive Day 1
+ **Q2V2Diff**: Difference in days between Quest Day 2 and Vive Day 2
+ **Q2C1Diff**: Difference in days between Quest Day 2 and Cosmos Day 1
+ **Q2C2Diff**: Difference in days between Quest Day 2 and Cosmos Day 2
+ **V1V2Diff**: Difference in days between Vive Day 1 and Vive Day 2
+ **V1C1Diff**: Difference in days between Vive Day 1 and Cosmos Day 1
+ **V1C2Diff**: Difference in days between Vive Day 1 and Cosmos Day 2
+ **V2C1Diff**: Difference in days between Vive Day 2 and Cosmos Day 1
+ **V2C2Diff**: Difference in days between Vive Day 2 and Cosmos Day 2
+ **C1C2Diff**: Difference in days between Cosmos Day 1 and Cosmos Day 2

### Data
Abbreviations are as follows Quest (Q), Vive (V), and Cosmos (C). A (1) represents the first day on the system and (2) represents the second day on the system. 

| ID | Q1Q2Diff | Q1V1Diff | Q1V2Diff | Q1C1Diff | Q1C2Diff | Q2V1Diff | Q2V2Diff | Q2C1Diff | Q2C2Diff | V1V2Diff | V1C1Diff | V1C2Diff | V2C1Diff | V2C2Diff | C1C2Diff |
|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|
| 100 | 1 | 2 | 3 | 24 | 30 | 1 | 2 | 23 | 29 | 1 | 22 | 28 | 21 | 27 | 6 |
| 101 | 1 | 2 | 3 | 22 | 24 | 1 | 2 | 21 | 23 | 1 | 20 | 22 | 19 | 21 | 2 |
| 102 | 1 | 2 | 3 | 24 | 30 | 1 | 2 | 23 | 29 | 1 | 22 | 28 | 21 | 27 | 6 |
| 103 | 1 | 2 | 3 | 25 | 30 | 1 | 2 | 24 | 29 | 1 | 23 | 28 | 22 | 27 | 5 |
| 105 | 1 | 2 | 3 | 28 | 29 | 1 | 2 | 27 | 28 | 1 | 26 | 27 | 25 | 26 | 1 |
| 106 | 1 | 2 | 3 | 21 | 22 | 1 | 2 | 20 | 21 | 1 | 19 | 20 | 18 | 19 | 1 |
| 108 | 1 | 2 | 3 | 22 | 23 | 1 | 2 | 21 | 22 | 1 | 20 | 21 | 19 | 20 | 1 |
| 109 | 1 | 2 | 3 | 21 | 22 | 1 | 2 | 20 | 21 | 1 | 19 | 20 | 18 | 19 | 1 |
| 110 | 1 | 2 | 3 | 21 | 22 | 1 | 2 | 20 | 21 | 1 | 19 | 20 | 18 | 19 | 1 |
| 111 | 1 | 2 | 3 | 21 | 23 | 1 | 2 | 20 | 22 | 1 | 19 | 21 | 18 | 20 | 2 |
| 112 | 1 | 2 | 3 | 21 | 23 | 1 | 2 | 20 | 22 | 1 | 19 | 21 | 18 | 20 | 2 |
| 113 | 1 | 2 | 4 | 24 | 25 | 1 | 3 | 23 | 24 | 2 | 22 | 23 | 20 | 21 | 1 |
| 114 | 2 | 3 | 10 | 21 | 25 | 1 | 8 | 19 | 23 | 7 | 18 | 22 | 11 | 15 | 4 |
| 115 | 1 | 3 | 10 | 21 | 22 | 2 | 9 | 20 | 21 | 7 | 18 | 19 | 11 | 12 | 1 |
| 116 | 1 | 2 | 3 | 23 | 24 | 1 | 2 | 22 | 23 | 1 | 21 | 22 | 20 | 21 | 1 |
| 117 | 2 | 10 | 13 | 27 | 30 | 8 | 11 | 25 | 28 | 3 | 17 | 20 | 14 | 17 | 3 |
| 120 | 1 | 9 | 13 | 19 | 21 | 8 | 12 | 18 | 20 | 4 | 10 | 12 | 6 | 8 | 2 |
| 121 | 1 | 9 | 13 | 19 | 21 | 8 | 12 | 18 | 20 | 4 | 10 | 12 | 6 | 8 | 2 |
| 122 | 1 | 2 | 8 | 10 | 13 | 1 | 7 | 9 | 12 | 6 | 8 | 11 | 2 | 5 | 3 |
| 123 | 1 | 8 | 10 | 13 | 14 | 7 | 9 | 12 | 13 | 2 | 5 | 6 | 3 | 4 | 1 |
| 124 | 1 | 2 | 6 | 7 | 8 | 1 | 5 | 6 | 7 | 4 | 5 | 6 | 1 | 2 | 1 |
| 125 | 1 | 2 | 7 | 8 | 9 | 1 | 6 | 7 | 8 | 5 | 6 | 7 | 1 | 2 | 1 |
| 126 | 1 | 7 | 8 | 9 | 13 | 6 | 7 | 8 | 12 | 1 | 2 | 6 | 1 | 5 | 4 |
| 127 | 1 | 2 | 7 | 8 | 9 | 1 | 6 | 7 | 8 | 5 | 6 | 7 | 1 | 2 | 1 |
| 128 | 1 | 2 | 7 | 8 | 9 | 1 | 6 | 7 | 8 | 5 | 6 | 7 | 1 | 2 | 1 |
| 131 | 1 | 6 | 7 | 8 | 10 | 5 | 6 | 7 | 9 | 1 | 2 | 4 | 1 | 3 | 2 |
| 132 | 1 | 2 | 7 | 9 | 10 | 1 | 6 | 8 | 9 | 5 | 7 | 8 | 2 | 3 | 1 |
| 135 | 1 | 5 | 6 | 7 | 8 | 4 | 5 | 6 | 7 | 1 | 2 | 3 | 1 | 2 | 1 |
| 136 | 1 | 2 | 8 | 9 | 10 | 1 | 7 | 8 | 9 | 6 | 7 | 8 | 1 | 2 | 1 |
| 137 | 1 | 2 | 6 | 7 | 8 | 1 | 5 | 6 | 7 | 4 | 5 | 6 | 1 | 2 | 1 |
| 138 | 1 | 5 | 6 | 7 | 8 | 4 | 5 | 6 | 7 | 1 | 2 | 3 | 1 | 2 | 1 |
| 139 | 1 | 2 | 7 | 8 | 13 | 1 | 6 | 7 | 12 | 5 | 6 | 11 | 1 | 6 | 5 |
| 140 | 1 | 2 | 8 | 9 | 10 | 1 | 7 | 8 | 9 | 6 | 7 | 8 | 1 | 2 | 1 |
| 141 | 6 | 7 | 8 | 9 | 10 | 1 | 2 | 3 | 4 | 1 | 2 | 3 | 1 | 2 | 1 |
| 142 | 1 | 8 | 10 | 13 | 14 | 7 | 9 | 12 | 13 | 2 | 5 | 6 | 3 | 4 | 1 |
| 143 | 1 | 2 | 7 | 8 | 9 | 1 | 6 | 7 | 8 | 5 | 6 | 7 | 1 | 2 | 1 |
| 144 | 1 | 2 | 7 | 8 | 13 | 1 | 6 | 7 | 12 | 5 | 6 | 11 | 1 | 6 | 5 |
| 145 | 1 | 2 | 7 | 8 | 13 | 1 | 6 | 7 | 12 | 5 | 6 | 11 | 1 | 6 | 5 |
| 146 | 1 | 2 | 6 | 7 | 9 | 1 | 5 | 6 | 8 | 4 | 5 | 7 | 1 | 3 | 2 |
| 147 | 1 | 2 | 6 | 7 | 8 | 1 | 5 | 6 | 7 | 4 | 5 | 6 | 1 | 2 | 1 |
| 148 | 1 | 5 | 6 | 7 | 8 | 4 | 5 | 6 | 7 | 1 | 2 | 3 | 1 | 2 | 1 |

### Summary Statistics
We provide summary statistics for the temporal difference (in days) between captures for each system pair. Abbreviation are as follows Quest (Q), Vive (V), and Cosmos (C). A (1) represents the first day on the system and (2) represents the second day on the system.

| SystemPair | Min |	Max |	Average |
|--|--|--|--|
| Q1Q2 | 1 | 6 | 1.17 |
| Q1V1 | 2 | 10 | 3.44 |
| Q1V2 | 3 | 13 | 6.44 |
| Q1C1 | 7 | 28 | 14.59 |
| Q1C2 | 8 | 30 | 16.63 |
| Q2V1 | 1 | 8 | 2.27 |
| Q2V2 | 2 | 12 | 5.27 |
| Q2C1 | 3 | 27 | 13.41 |
| Q2C2 | 4 | 29 | 15.46 |
| V1V2 | 1 | 7 | 3.00 |
| V1C1 | 2 | 26 | 11.15 |
| V1C2 | 3 | 28 | 13.20 |
| V2C1 | 1 | 25 | 8.15 |
| V2C2 | 2 | 27 | 10.20 | 
| C1C2 | 1 | 6 | 2.05 |
