# TIAND

The dataset consists of three sensor data: RADAR, LiDAR, and camera. The radar data is provided in .csv format, lidar in .pcd format and camera data in .jpg format. The data provided by the sensors is further segregated as shown below:
                                                    
                                            TIAND_DATASET_ROOT
                                            ├── calib
                                            │   ├── lidar
                                            │   │   ├── lidar_calibration.txt
                                            │   ├── radar
                                            │   │   ├── radar_calibration.txt
                                            │   ├── camera
                                            │   │   ├── camera_calibration.txt
                                            │  
                                            ├── camera
                                            │   ├── front
                                            │   │   ├── image_001.jpg
                                            │   │   ├── image_002.jpg
                                            │   │   ├── ...
                                            │   └── front-right
                                            │   │   ├── image_001.jpg
                                            │   │   ├── image_002.jpg
                                            │   │   ├── ...
                                            │   └── front-left
                                            │   │   ├── image_001.jpg
                                            │   │   ├── image_002.jpg
                                            │   │   ├── ...
                                            │   └── back
                                            │       ├── image_001.jpg
                                            │       ├── image_002.jpg
                                            │       ├── ...
                                            ├── radar
                                            │   ├── front
                                            │   │   ├── radar_data_001.csv
                                            │   │   ├── radar_data_002.csv
                                            │   │   ├── ...
                                            │   └── front-right
                                            │   │   ├── radar_data_001.csv
                                            │   │   ├── radar_data_002.csv
                                            │   │   ├── ...
                                            │   └── front-left
                                            │   │   ├── radar_data_001.csv
                                            │   │   ├── radar_data_002.csv
                                            │   │   ├── ...
                                            │   └── back
                                            │   │   ├── radar_data_001.csv
                                            │   │   ├── radar_data_002.csv
                                            │   │   ├── ...
                                            │   └── back-left
                                            │   │   ├── radar_data_001.csv
                                            │   │   ├── radar_data_002.csv
                                            │   │   ├── ...
                                            │   └── back-right
                                            │       ├── radar_data_001.csv
                                            │       ├── radar_data_002.csv
                                            │       ├── ...
                                            ├── lidar
                                            │   ├── lidar_data_001.pcd
                                            │   ├── lidar_data_002.pcd
                                            │   ├── ...

# Sensor Data
- RADAR:
The .csv files for radar scans have 9 rows each. Each of the rows signifies a different channel of radar data, as described below:
 1. Scan type
    > 0: Near Scan (Long-range radar)
    > 1: Far Scan (Long-range radar)
    > 2: Near Scan (Short-range radar)
    > 3: High Resolution-Range Scan (Short-range radar)
 2. Range
 3. Azimuth
 4. Relative Velocity
 5. Radial Cross-Section [RCS]
 6. Range Variance
 7. Relative Velocity Variance
 8. Azimuth Variance
 9. Signal-to-noise ratio [SNR]

- LiDAR:
The lidar data is provided in .pcd format as shown in the above data schema. These pcds consist of the following information:
1. X
2. Y
3. Z
4. Intensity
5. Ambience
6. Range
7. Rings

- CAMERA:
The camera data was captured using 4 cameras in .jpg format with a resolution of 1280x720p.

# Synchronisation
We have synchronized front radar and front camera and, lidar and front camera. The synchronization for these sensors is provided in .csv format, where the closest timestamp for the sensor is provided with respect to the front camera.

# Computer architecture used and sensor specifications
We have used Ubuntu 18.04 LTS for the ROS-based data recording.
- Camera : Baseler aCA1920-40gc
- Radar : Long Range - ARS430DI; Short Range - SRR520DI
- LiDAR : Ouster OS2, Velodyne VLS-128

# Download Link
https://iith-my.sharepoint.com/:f:/g/personal/ee22mtech02005_iith_ac_in/EnNXPXQMmidDl1QYOKIRhxkBtwoWCiG1gcGex9dvxVcfSQ?e=AVU4pS


