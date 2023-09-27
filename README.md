# TIAND

The dataset consists of three sensor data: RADAR, LiDAR, and camera. The radar data is provided in .csv format, lidar in .pcd format, and camera data in .jpg format. The data provided by the sensors is further segregated as shown below:
                                                    
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
                                            ├── GNSS
                                            │   ├── gnss_data.csv
                                            
        

# Sensor Data
- RADAR:
The .csv files for radar scans have nine rows each. Each of the rows signifies a different channel of radar data, as described below:
 1. X Distance
 2. Y Distance
 3. Standard Deviation in X Distance
 4. Standard Deviation in Y Distance
 5. Radial Cross-Section [RCS]
 6. Velocity in X direction
 7. Velocity in Y direction
 8. Acceleration in X direction
 9. Acceleration in Y direction
 10. Standard Deviation of Velocity in X direction
 11. Standard Deviation of Velocity in Y direction
 12. Standard Deviation of Acceleration in X direction
 13. Standard Deviation of Acceleration in Y direction

- LiDAR:
The lidar data is provided in .pcd format, as shown in the above data schema. These pcds consist of the following information:
1. X
2. Y
3. Z
4. Intensity
5. Ambience
6. Range
7. Rings

- CAMERA:
The camera data was captured using four cameras in .jpg format with a resolution of 1280x720p.

- GNSS:
The GNSS data consist of:
1. Time
2. Latitude
3. Longitude
4. Height
5. North Velocity
6. East velocity
7. Up velocity
8. Roll
9. Pitch
10. Azimuth

# Synchronization
We have synchronized front radar and front camera and lidar and front camera. The sensor synchronization is provided in .csv format, where the closest timestamp for the sensor is provided concerning the front camera. Synchronized Radar-Camera and Lidar-Camera timestamps are stored in .csv file which has a precision of up to 6 decimal places. To view these files please open in standard software like LibreOffice or Microsoft Office.

# Computer architecture used and sensor specifications
Ubuntu 18.04 LTS was used for ROS-based data recording.
The sensor configurations are:
- Camera: Baseler aCA1920-40gc
- RADAR: Long Range - ARS430DI; Short Range - SRR520DI
- LiDAR: Ouster OS2, Velodyne VLS-128
- GNSS: NovAtel PwrPak7

# Download Link
https://iith-my.sharepoint.com/:f:/g/personal/ee22mtech02005_iith_ac_in/EnNXPXQMmidDl1QYOKIRhxkBtwoWCiG1gcGex9dvxVcfSQ?e=
