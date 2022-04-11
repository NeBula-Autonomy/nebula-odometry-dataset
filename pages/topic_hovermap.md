# Hovermap dataset

## Husky

- Hovermap data (```${robot_name}_lidar_*.bag```)
  - Hovermap ```sensor_msgs/PointCloud2``` topics
    - ```${robot_name}/hvm/lidar/points```    
      - frame_id: ```${robot_name}/hovermap```
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
  - Topics that you shouldn't care about
    - ```/${robot_name}/spot_driver/local_grid``` 

- IMU data (```${robot_name}_state_tcp_no_delay_*```)
  - ```${robot_name}/vn100/imu ```
  - ```${robot_name}/vn100/imu_wori_wcov ```
  - Topics that you shouldn't care about
    - ```${robot_name}/resiliency_logic/debug```
    - ```${robot_name}/resiliency_logic/resiliency_status```
- Odometry data (```${robot_name}_state_*```)
  - ```${robot_name}/hero/odometry```
  - ```${robot_name}/hero/wio_ekf/odom```
  - ```${robot_name}/hvm/odometry```
  - ```${robot_name}/hvm/odometry_transformed``` 
  - ```${robot_name}wheel_odom```
  - ```${robot_name}wheel_odom_wfid```
  - Topics that you shouldn't care about
    - ```${robot_name}/hero/husky_all_in/odom```
    - ```${robot_name}/hero/lamp/odom_wcov```
    - ```${robot_name}/hero/lio_lamp_ekf/odom```
    - ```${robot_name}/joint_states```
    - ```${robot_name}/joy_teleop/cmd_vel``` 

## Spot

- LiDAR data (```${robot_name}_lidar_*.bag```)
  - Hovermap ```sensor_msgs/PointCloud2``` topics
    - ```${robot_name}/hvm/lidar/points```    
      - frame_id: ```${robot_name}/hovermap```
- IMU data (```${robot_name}_state_tcp_no_delay_*```) 
  - **(Note: keep in mind that in B, E IMU is not available)**
  - ```${robot_name}/vn100/imu ```
  - ```${robot_name}/vn100/imu_wori_wcov ``` 
  - Topics that you shouldn't care about  
    - ```${robot_name}/resiliency_logic/debug```
    - ```${robot_name}/resiliency_logic/resiliency_status``` 
- Odometry data (```${robot_name}_state_*```)
  - ```${robot_name}/hero/hvm_ekf/odom       ```
  - ```${robot_name}/hero/odometry           ```
  - ```${robot_name}/hvm/odometry            ```
  - ```${robot_name}/hvm/odometry_transformed```
  - ```${robot_name}/kinematic_odom          ```
  - ```${robot_name}/visual_odom             ```
  - Topics that you shouldn't care about  
  - ```${robot_name}/joint_states            ```
  - ```${robot_name}/spot_driver/twist       ```
