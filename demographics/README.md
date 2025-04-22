## User Demographics

### Contents
[Overview](#overview)

[Data](#data)

[Summary Statistics](#summary-statistics)

### Overview
The file demographics.csv provides user demographics for: **Self Identified Gender**, **Age**, **Height (in)**, **Weight (lb)**, **Writing Hand**, **Throwing Hand**, **Throwing Sport Experience**, **Type of Throwing Sport**, and **VR Experience**. The value of **ID** is matched to the same users in the [croppedvideo](../croppedvideos), [mmpose](../mmpose_results), and [openpose](../openpose_results) body pose data folders and [vrmotions](../vrmotions) VR system NumPy files. 

+ **Throwing Sport Experience** is a Likert-like scale with values ranging from none, low, low-medium, medium, medium-high, high.
+ **VR Experience** is a Likert-like scale with values ranging from none, low, low-medium, medium, medium-high, high.
+ **Type of Throwing Sport** can take multiple values separated by a '/'.
+ A (blank) indicates that the participant did not provide data for that field. 

### Data
| ID | Self Identified Gender | Age | Height (in) | Weight (lbs) | Writing Hand | Throwing Hand | Throwing Sport Experience | Type of Throwing Sport | VR Experience |
|--|--|--|--|--|--|--|--|--|--|
| 100 | Female | 32 | 63 | 124 | right | right | low | badminton | medium |
| 101 | Male | 30 | 67 | (blank) | right | right | low | no | low |
| 102 | Male | 38 | 72 | 165 | right | right | low | tennis | medium |
| 103 | Male | 18 | 69.5 | 145 | right | right | low | baseball | low-medium |
| 105 | Male | 22 | 63 | (blank) | right | right | low | football | low-medium |
| 106 | Male | 21 | 69 | 200 | right | right | medium | baseball | medium-high |
| 108 | Male | 21 | 72 | 164 | right | right | medium | baseball | low |
| 109 | Male | 19 | 72 | 180 | left | right | high | baseball/basketball/football | low-medium |
| 110 | Male | 19 | 75 | 170 | right | right | medium | dodgeball | low-medium |
| 111 | Male | 19 | 73 | 180 | right | right | low-medium | basketball/football | low |
| 112 | Male | 20 | 72.5 | 170 | right | right | high | baseball | medium |
| 113 | Male | 19 | 71 | 160 | right | right | none | no | high |
| 114 | Male | 21 | 74 | 180 | right | right | medium | baseball | medium |
| 115 | Male | 19 | 72 | 142 | right | right | medium | basketball | low |
| 116 | Female | 20 | 68.5 | 150 | right | right | low | none | medium |
| 117 | Female | 19 | 66 | (blank) | right | right | medium | basketball | low |
| 120 | Male | 20 | 70 | 130 | right | right | medium | no | medium |
| 121 | Male | 20 | 67 | 175 | right | right | medium-high | baseball/football | low |
| 122 | Male | 20 | 73 | 157 | right | right | medium-high | frisbee/basketball/baseball/football/soccer | medium |
| 123 | Male | 20 | 78 | 285 | right | right | medium-high | basketball | low-medium |
| 124 | Male | 19 | 77 | 250 | right | right | medium-high | basketball | low |
| 125 | Male | 20 | 73 | 185 | left | right | medium | baseball | low |
| 126 | Male | 21 | 70 | (blank) | right | right | medium | no | none |
| 127 | Male | 19 | 69 | 134 | right | right | medium | baseball | low |
| 128 | Male | 20 | 70 | 155 | right | right | high | baseball | none |
| 131 | Male | 19 | 72 | 260 | right | right | high | baseball/dodgeball | none |
| 132 | Male | 19 | 70 | 193 | right | right | none | no | low-medium |
| 135 | Male | 21 | 71 | 180 | right | right | high | football/baseball | none |
| 136 | Male | 19 | 67 | 170 | right | right | low | none | low-medium |
| 137 | Male | 19 | 71 | 230 | right | right | high | baseball | none |
| 138 | Male | 20 | 70 | 155 | right | right | medium-high | baseball/football | low |
| 139 | Male | 21 | 69 | 210 | right | right | none | no | low |
| 140 | Male | 19 | 68 | 160 | right | right | low-medium | no | none |
| 141 | Male | 19 | 76 | 190 | right | right | medium-high | baseball | low |
| 142 | Male | 21 | 72 | 180 | right | right | high | baseball | low |
| 143 | Male | 20 | 65 | 160 | right | right | high | football/bbaseball | low |
| 144 | Male | 20 | 71 | 174 | right | right | medium | baseball | medium |
| 145 | Male | 20 | 71 | 230 | right | right | medium | no | none |
| 146 | Male | 19 | 76 | (blank) | right | right | medium | football/baseball | low |
| 147 | Male | 20 | 75 | 230 | right | right | medium-high | basketball/baseball | none |
| 148 | Male | 19 | 78 | 225 | right | right | high | dodgeball/football/baseball | none |
 

### Summary Statistics
We provide summary statistics of our user demographics below:

**Age, Height, Weight Summary**
| Demographic |	Min |	Max |	Average |
|--|--|--|--|
| Age	| 18	| 38	| 20.76 |
| Height (in) |	63	| 78	| 70.94 |
| Weight (lbs) | 124	| 285 |	181.89 |

**Self Identified Gender**
|Self Identified Gender|Count|
|--|--|
| Female |	3 |
| Male	| 38 |

**Throwing Sport Experience**
|Level|Count|
|--|--|
| none |	3 |
| low	| 7 |
| low-medium |	2 |
| medium |	13 |
| medium-high |	7
| high |	9 |

**VR Experience**
|Level|Count|
|--|--|
| none	| 9 |
| low	| 15 |
| low-medium |	7 |
| medium |	8 |
| medium-high |	1 |
| high |	1 |


