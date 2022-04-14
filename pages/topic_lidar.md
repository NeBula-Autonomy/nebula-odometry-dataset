# LiDAR dataset 

## Husky

- LiDAR data (```${robot_name}_lidar_*.bag```)
  - LiDAR ```sensor_msgs/PointCloud2``` topics
    - ```${robot_name}/velodyne/velodyne_points```    
      - frame_id: ```${robot_name}/velodyne```
    - ```${robot_name}/velodyne_front/velodyne_points``` 
      - frame_id: ```${robot_name}/velodyne_front```
    - ```${robot_name}/velodyne_rear/velodyne_points``` 
      - frame_id: ```${robot_name}/velodyne_rear```
  - LiDAR packet ```velodyne_msgs/VelodyneScan``` topics
    - ```${robot_name}/velodyne_packets``` 
      - frame_id: ```${robot_name}/velodyne```
    - ```${robot_name}/velodyne_front/velodyne_packets``` 
      - frame_id: ```${robot_name}/velodyne_front```
    - ```${robot_name}/velodyne_rear/velodyne_packets``` 
      - frame_id: ```${robot_name}/velodyne_rear```
  - topics that you should not care about:
    - ```${robot_name}/velodyne_points_min_dist```

- IMU data (```${robot_name}_state_tcp_no_delay_*```)
  - ```${robot_name}/vn100/imu ```
  - ```${robot_name}/vn100/imu_wori_wcov ```
  - Topics that you shouldn't care about
    - ```${robot_name}/resiliency_logic/debug```  (not available in D and F)
    - ```${robot_name}/resiliency_logic/resiliency_status```  (not available in D and F)
- Odometry data (```${robot_name}_state_*```)
  - ```${robot_name}hero/odometry```  (not available in D and F)
  - ```${robot_name}hero/wio_ekf/odom```
  - ```${robot_name}wheel_odom``` (not available in D and F)
  - ```${robot_name}wheel_odom_wfid```  (not available in D and F)
  - Topics that you shouldn't care about
    - ```${robot_name}hero/lamp/odom         ```
    - ```${robot_name}hero/lio_lamp_ekf/odom ```
    - ```${robot_name}hero/wio_ekf/odom      ```
    - ```${robot_name}joint_states           ```
    -  /husky1/hero/husky_all_in/odom
    -  /husky1/hero/lamp/odom_wcov 



## Spot

- LiDAR data (```${robot_name}_lidar_*.bag```)
  - LiDAR ```sensor_msgs/PointCloud2``` topics
    - ```${robot_name}/velodyne/velodyne_points```    
      - frame_id: ```${robot_name}/velodyne```
  - LiDAR packet ```velodyne_msgs/VelodyneScan``` topics
    - ```${robot_name}/velodyne_packets``` 
  - topics that you should not care about:
    - ```${robot_name}/velodyne_points_min_dist```

- IMU data (```${robot_name}_state_tcp_no_delay_*```) 
  - **(Note: keep in mind that in B, E IMU is not available)**
  - ```${robot_name}/vn100/imu ```
  - ```${robot_name}/vn100/imu_wori_wcov ``` 
  - Topics that you shouldn't care about   - ```${robot_name}/resiliency_logic/debug```
    - ```${robot_name}/resiliency_logic/resiliency_status``` 
- Odometry data (```${robot_name}_state_*```)
    - ```${robot_name}/kinematic_odom``` 
    - ```${robot_name}/visual_odom ```
    - ```${robot_name}/hero/odometry```
    - ```${robot_name}/hero/hvm_ekf/odom``` (available only in K,P)
    - ```/${robot_name}/hero/amcckf/odom``` (available only in K,P)
  - Topics that you shouldn't care about
    - ```${robot_name}/joint_states```
    - ```${robot_name}/spot_driver/twist```
    - ```${robot_name}/hero/lamp/odom```
    - ```${robot_name}/hero/spot_all_in/odom```
    - ```${robot_name}/hero/lamp/odom_wcov```
    - ```$/joy_teleop/cmd_vel```