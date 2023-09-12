# TI-AND

The dataset consists of three sensor data: RADAR, LiDAR and camera. The radar data is provided in .csv format, lidar in .pcd format and camera data in .jpg format. The data provided by the sensors is further segregated as shown below:
                                                    
                                                    TI-AND_DATASET_ROOT
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

- CAMERA:
The camera data was captured using 4 cameras in .jpg format with a resolution of 1280x720p.

# Synchronisation
We have synchronised front radar and front camera and, lidar and front camera. The synchronisation for these sensors are provided in .csv format, where the closest timestamp for the sensor is provided with respect to the front camera.
