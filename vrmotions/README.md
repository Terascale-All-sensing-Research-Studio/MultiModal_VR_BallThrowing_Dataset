## VR Motion 

Each NumPy (npy) represents one day of data collection using each VR systems and consists of NumPy arrays with the shape (41, 10, 135, 21): 

* The first dimension indexes the subject ID;
* The second corresponds to the sequential throws performed by the user;
* The third dimension represents the temporal sequence;
* and the fourth captures the feature set at each time step. 

**NOTE**: Each feature vector includes the position (x, y, z), Euler angles (x, y, z), and trigger pressure (ranging from 0 to 1) for the right-hand controller, headset, and left-hand controller. Trigger pressure values for the headset are always set to zero.

+ [Cosmos1.npy](Cosmos1.npy): Contains data for all 41 participants using the HTC Vive Cosmos on day 1 of usage with the HTC Vive Cosmos.
+ [Cosmos2.npy](Cosmos2.npy): Contains data for all 41 participants using the HTC Vive Cosmos on day 2 of usage with the HTC Vive Cosmos.
+ [Quest1.npy](Quest1.npy): Contains data for all 41 participants using the Meta Quest on day 1 of usage with the HTC Vive Cosmos.
+ [Quest2.npy](Quest1.npy): Contains data for all 41 participants using the Meta Quest on day 2 of usage with the HTC Vive Cosmos.
+ [Vive1.npy](Vive1.npy): Contains data for all 41 participants using the HTC Vive on day 1 of usage with the HTC Vive Cosmos.
+ [Vive2.npy](Vive2.npy): Contains data for all 41 participants using the HTC Vive on day 2 of usage with the HTC Vive Cosmos.

## Example Headset and Hand Controller Trajectories From Dataset

![](/figs/vrmotion/trajectories.png)
