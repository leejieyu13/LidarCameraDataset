# LidarCameraDataset

This is a dataset of LiDAR and image data captured at the University of Notre Dame with different environments, a non-cluttered area, a cluttered area and a long corridor.
The LiDAR and the intensity camera are mounted with fixed relative location on a platform moving on the floor.
The floorplan and robot trajectories are shown in the figure. 
![alt text](https://github.com/leejieyu13/LidarCameraDataset/blob/main/floorplandataset.png)

## LiDAR
The LiDAR data is captured by a Slamtec's laser range scanner "RPLIDAR A3". In the .txt files, the first column is angle in degree and the second conlumn is range in mm.
The LiDAR poses (in cm and radius) are estimated by ICP algorithm. 

## Images
The images are captured by a camera with intrinsic matrix =
[1064.2, -4.0,  982.2;
  0,    1066.2, 519.8;
  0,       0,      1]

## Ground truth
The semantic segmentation ground truth is generated by manually labeling the planes for all pixels (i.e. the walls and the ground plane) without the ceiling.
The floor-plan ground truth is defined by a set of manually measured line segments, which is NOT in the same coordinate system of the LiDAR location. 
