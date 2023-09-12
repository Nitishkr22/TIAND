# TI-AND

The dataset consists of three sensor data: RADAR, LiDAR and camera. The radar data is provided in .csv format, lidar in .pcd format and camera data in .jpg format. The data provided by the sensors is further segregated as shown below:
                                                              
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

# Sensors
- RADAR
The .csv files for radar scans have 9 rows each. Each of the row signify a different type of radar data:
 1. Scan type
 2. Range
 3. Azimuth
 4. Relative Velocity
 5. Radial Cross-Section [RCS]
 6. Range Variance
 7. Relative Velocity Variance
 8. Azimuth Variance
 9. Signal-To-Noise Ratio [SNR]
