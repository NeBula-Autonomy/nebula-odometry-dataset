# Datasets

Here, you can download the datasets. 
- ```Rosbags``` - bag files to run
- ```Ground truth``` - rosbag file **odometry.bag** that has a ground truth trajectory
- ```Sensor calibration files``` - stores information about relative transformation between frames and sensors
- ```Extra files``` - 3D map provides information of the scanned 3D map
- ```2D image``` - provides information of the enviornment from bird's-eye-view


|  ID | Place  | Domain  | Robot   | Distance (m) | Duration (min)  | rosbags  | Extra files  | 2D image | 
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| A  | Satsop Power Plane Elma, WA              |Urban | Husky | 631.53   |59:56   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)  |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |
| B  | Satsop Power Plane Elma, WA              |Urban | Spot  | 664.27   |32:26   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   | 
| C  | Satsop Power Plane Elma, WA              |Urban | Husky | 757.40   |24:21   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)  |
| D  | Bruceton Mine Pittsburgh, PA             |Tunnel| Husky | 1795.88  |65:36   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |
| E  | Lava Beds National Monument, CA          |Cave  | Spot  | 590.85   |25:20   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |
| F  | Bruceton Mine Pittsburgh, PA             |Tunnel| Husky | 1569.73  |49:13   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)  |
| G  | Satsop Power Plane Elma, WA              |Urban | Husky | 877.21   |93:10   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)  |
| H  | Subway Station Los Angeles, CA           |Urban | Spot  | 1777.45  |46:57   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |
| I  | Kentucky Underground Limestone Mine, KY  |Tunnel| Spot  | 768.82   |19:28   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |
| J  | Kentucky Underground Limestone Mine, KY  |Tunnel| Husky | 2339.81  |57:55   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)  |
| K  | DARPA Final Louisville Cave, KY          |Mix   | Spot  | 798.24   |30:56   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |
| L  | DARPA Final Louisville Cave, KY          |Mix   | Spot  | 245.13   |11:41   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)  |
| M  | DARPA Final Louisville Cave, KY          |Mix   | Spot  | 722.37   |19:57   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)  |
| N  | DARPA Final Louisville Cave, KY          |Mix   | Husky | 325.30   |24:08   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |
| O  | DARPA Final Louisville Cave, KY          |Mix   | Husky | 488.48   |23:48   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |
| P  | DARPA Final Louisville Cave, KY          |Mix   | Spot  | 571.79   |34:13   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |
| Q  | DARPA Final Louisville Cave, KY          |Mix   | Spot  | 744.60   |26:55   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |
| R  | DARPA Final Louisville Cave, KY          |Mix   | Husky | 328.42   |13:02   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)   |[click](https://makeameme.org/meme/weve-got-some-ywcih8)    |
 
# Ground truth

To determine the ground truth of the robot in the environment, a survey-grade $3D$ map (provided by DARPA in the Subterranean Challenge or produced by the team) is used (see Extra files).
The ground-truth trajectory is produced by running [LOCUS](https://github.com/NeBula-Autonomy/LOCUS) against the survey-grade map (i.e., scan-to-map is scan-to-survey-map). In this mode, LOCUS is tuned for maximum accuracy at the cost of computational efficiency, as it does not need to be run in real-time.  

# Recorded topics


# Extrinsic Calibration

# Initial Pose
