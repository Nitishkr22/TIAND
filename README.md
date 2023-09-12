# TI-AND

The dataset consists of three sensor data: RADAR, LiDAR and camera. The radar data is provided in .csv format, lidar in .pcd format and camera data in .jpg format. The data provided by the sensors is further segregated as shown below:
                                                      ├── Calibration files  
                                                      │   ├── Camera
                                                      │   ├── Radar
                                                      │   ├── Lidar
                                                      ├── CAMERA
                                                      │   ├── Front
                                                      │   │   ├── image_001.jpg
                                                      │   │   ├── image_002.jpg
                                                      │   │   ├── ...
                                                      │   └── Front-Right
                                                      │   │   ├── image_001.jpg
                                                      │   │   ├── image_002.jpg
                                                      │   │   ├── ...
                                                      │   └── Front-Left
                                                      │   │   ├── image_001.jpg
                                                      │   │   ├── image_002.jpg
                                                      │   │   ├── ...
                                                      │   └── Back
                                                      │       ├── image_001.jpg
                                                      │       ├── image_002.jpg
                                                      │       ├── ...
                                                      ├── RADAR
                                                      │   ├── Front
                                                      │   │   ├── radar_data_001.csv
                                                      │   │   ├── radar_data_002.csv
                                                      │   │   ├── ...
                                                      │   └── Front-Right
                                                      │   │   ├── radar_data_001.csv
                                                      │   │   ├── radar_data_002.csv
                                                      │   │   ├── ...
                                                      │   └── Front-Left
                                                      │   │   ├── radar_data_001.csv
                                                      │   │   ├── radar_data_002.csv
                                                      │   │   ├── ...
                                                      │   └── Back
                                                      │   │   ├── radar_data_001.csv
                                                      │   │   ├── radar_data_002.csv
                                                      │   │   ├── ...
                                                      │   └── Back-Left
                                                      │   │   ├── radar_data_001.csv
                                                      │   │   ├── radar_data_002.csv
                                                      │   │   ├── ...
                                                      │   └── Back-Right
                                                      │       ├── radar_data_001.csv
                                                      │       ├── radar_data_002.csv
                                                      │       ├── ...
                                                      ├── LIDAR
                                                      │   ├── lidar_data_001.pcd
                                                      │   ├── lidar_data_002.pcd
                                                      │   ├── ...

# Sensors
- RADAR:
The .csv files for radar scans have 9 rows each. Each of the row signify a different channel of radar data, as described below:
 1. Scan type
 2. Range
 3. Azimuth
 4. Relative Velocity
 5. Radial Cross-Section [RCS]
 6. Range Variance
 7. Relative Velocity Variance
 8. Azimuth Variance
 9. Signal-To-Noise Ratio [SNR]

- LiDAR:
The lidar data is provided in .pcd format like shown in the above data schema. These pcds consist the following information:
1. X
2. Y
3. Z
4. Intensity
5. Ambience
6. Range
7. Rings
