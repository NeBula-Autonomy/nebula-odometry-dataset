# Overview.

The dataset is provided by the [Team CoSTAR](https://costar.jpl.nasa.gov/) that has been intensively testing the multi-robot system in real world environments such as caves, tunnels, abandoned factories and industrial plants for [DARPA Subterranean Challenge](https://www.google.com/search?q=darpa+subt+challenge&oq=darpa+subt&aqs=chrome.1.69i57j35i39j0i512l2j69i60l2j69i65j69i60.2114j0j7&sourceid=chrome&ie=UTF-8)
<p align="center">
<img src="../images/all_robots2.png" alt="drawing" width="1000"/>
</p>


# Dataset real-world places.

## [Power plant located in Elma, WA](https://www.google.com/maps/place/Satsop+Nuclear+Power+Plant/@46.9616165,-123.472372,16z/data=!4m5!3m4!1s0x0:0x8a108aba7feb7724!8m2!3d46.9616231!4d-123.4675564)

<img src="../images/powerplant.jpg" alt="drawing" width="800"/>

## [Los Angeles Subway Station](https://www.google.com/maps?sxsrf=APq-WBs2xsWuIbnKaUCng_E2JNoqyeyrBA:1649605757386&uact=5&gs_lcp=Cgdnd3Mtd2l6EAMyBwghEAoQoAEyBwghEAoQoAEyBwghEAoQoAE6BwgAEEcQsANKBAhBGABKBAhGGABQgQJYgQJg2wNoAXABeACAAXqIAXqSAQMwLjGYAQCgAQKgAQHIAQjAAQE&q=South+Hill+Street+near+Pershing+Square&um=1&ie=UTF-8&sa=X&ved=2ahUKEwinstSs7In3AhXsAxAIHZALCW8Q_AUoAXoECAEQAw)

<img src="../images/la_old_subway_old.jpeg" alt="drawing" width="400"/> <img src="../images/la_old_subway.png" alt="drawing" width="400"/>

## [Bruceton Research Mine in Pittsburgh, PA](https://www.google.com/maps/place/Bruceton+Research+Mine/@40.3040108,-79.978597,15z/data=!4m2!3m1!1s0x0:0xa44441e8bb7eb69f?sa=X&ved=2ahUKEwi4vrCP4Yn3AhVumIsKHT19BY4Q_BJ6BAhGEAM)

<img src="../images/tunnel_circuit.jpg" alt="drawing" width="800"/>

## [Valentine Cave](https://www.google.com/maps?q=valentine+cave&um=1&ie=UTF-8&sa=X&ved=2ahUKEwjA5ouf4Yn3AhWLuYsKHYgoCzYQ_AUoAnoECAEQBA)

<img src="../images/spot.jpg" alt="drawing" width="400"/> <img src="../images/valentine_cave2.png" alt="drawing" width="400"/>

## [Kentucky Mine](https://www.google.com/maps/place/Kentucky+Mine+Rd,+Sierra+City,+CA+96125,+USA/@39.5726142,-120.6238181,17z/data=!3m1!4b1!4m5!3m4!1s0x809c769dc30942d9:0xe860a5889640f52f!8m2!3d39.5726142!4d-120.6216294)

<img src="../images/kentucky_cave3.png" alt="drawing" width="400"/><img src="../images/kentucky_cave4.png" alt="drawing" width="400"/>

## [Louisville Mine, artificially made circuit](https://www.google.com/maps?q=Louisville+Mine&um=1&ie=UTF-8&sa=X&ved=2ahUKEwjFiLa47In3AhXpk4sKHb7pAZIQ_AUoAnoECAEQBA)

<img src="../images/darpa1.png" alt="drawing" width="400"/><img src="../images/darpa2.png" alt="drawing" width="400"/>

<img src="../images/darpa4.png" alt="drawing" width="400"/><img src="../images/darpa4.png" alt="drawing" width="400"/>

Each dataset is selected to contain components that are challenging for LiDAR odometry. The datasets have different duration lengths from 20~min up to 1~h (see [here](dataset.md)). The dataset provides LiDAR scans, Inertial Measurement Unit (IMU) and wheeled inertial odometry (WIO) measurements, and cameras stream (**low frequency**). All datasets have been recorded on different robotics platforms, e.g., Husky and Spot with vibrations and large, sudden accelerations as is characteristic of both a skid-steer wheeled robot traversing rough terrain (husky) and a legged robot that slips and acts dynamically in rough terrain (spot).
The dataset is synchronized by window time stamp approach where the current time stamp looks for the closest time stamps available with maximum threshold time distance.
LiDAR scans are recorded at 10~Hz. WIO and IMU are recorded at 50~Hz in the Urban datasets, while a higher-rate IMU recording (100~Hz) is available for the Tunnel and Cave dataset.

# Robot Equipment

## Husky

<img src="../images/husky_equpiment.jpg" alt="drawing" width="400"/>

### Equipment
- 3 on-board [Velodyne’s Puck lidar sensor (VLP-16)](https://velodynelidar.com/products/puck/) LiDAR sensors (one flat, one pitched forward ~30 &deg;, one pitched backward ~30 &deg;).
- 6 on-board cameras: 5 RealSense D455 (DATASET FOR THIS IS NOT AVAILABLE)
- IMU
- wheel encoders


## Spot
  <img src="../images/spot_equipment.png" alt="drawing" width="400"/>

### Equipment
- 1 on-board [Velodyne’s Puck lidar sensor (VLP-16)](https://velodynelidar.com/products/puck/) LiDAR sensors 
- Out-of-the-box kinematic-ineratial odometry (KIO) and visual-inertial odometry (VIO) measurements implemented by [Boston Dynamics](https://www.bostondynamics.com/) 
- 6 on-board cameras: 5 RealSense D455 (DATASET FOR THIS IS NOT AVAILABLE)
- IMU


