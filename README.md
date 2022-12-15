# Introduction
In the future, there will be more and more cameras around us, especially after AR glasses become popular. Using these huge amount of visual information to build a virtual parallel world is a wonderful dream. The goal of this project is to provide vision-based positioning capabilities for this parallel world.
The specific goal in the near future is to establish a location system based on the map which is formed by feature points. And all data used to create map are from mobile phone level sensors (monocular camera, imu, gps). And provide a positioning service that give position with gps cordinate system.

# Main Content
Video data collection and LocalMap creation on the mobile phone.
Image data collection and feature point extraction. These means the system supports both sequence frame and single picture update.
After uploading the LocalMap or image feature points to the server, the server merges the data.
The merging process includes the culling of map to maintain trackable map size.
New data that is not matched by the map will be stored, waiting for matching with future data.

# Algorthim Flow
![image](https://user-images.githubusercontent.com/120680301/207954353-63ed66b7-715d-437f-a09b-f9425128bf1e.png)
