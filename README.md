# Unscented Kalman Filter Project Starter Code
Self-Driving Car Engineer Nanodegree Program

---

## Dependencies

* cmake >= v3.5
* make >= v4.1
* gcc/g++ >= v5.4

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./UnscentedKF path/to/input.txt path/to/output.txt`. You can find
   some sample inputs in 'data/'.
    - eg. `./UnscentedKF ../data/obj_pose-laser-radar-synthetic-input.txt`

## Results
RMSE [px, py, vx, vy]

UKF Radar + Lidar: RMSE [0.0666965, 0.088302, 0.203527, 0.174157] 
![Fusion Plot](visualizations/fusionplot.png)

UKF Radar only: RMSE [0.234196, 0.265973, 0.329845, 0.285553]
![Radar Plot](visualizations/radarplot.png)

UKF Lidar only: RMSE [0.157616, 0.146517, 0.298011, 0.21496]
![Lidar Plot](visualizations/lidarplot.png)

EKF Fusion: Used different dataset so RMSE not valid. But you can see the difference in accuracy caused by the constant velocity motion model
![NIS Plot](visualizations/ekfplot.png)

NIS
![NIS Plot](visualizations/nisplot.png)
