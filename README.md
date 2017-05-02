# Self-Driving Car Engineer Nanodegree Program

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

UKF Radar + Lidar: RMSE [0.0658812, 0.0819983, 0.33095, 0.217116] 
![Fusion Plot](visualizations/fusionplot.png)

UKF Radar only: RMSE [0.209408, 0.259503, 0.455479, 0.283628]
![Radar Plot](visualizations/radarplot.png)

UKF Lidar only: RMSE [0.169299, 0.1477, 0.596994, 0.259302]
![Lidar Plot](visualizations/lidarplot.png)

EKF Fusion: Used different dataset so RMSE not valid. But you can see the difference in accuracy caused by the constant velocity motion model
![NIS Plot](visualizations/ekfplot.png)

NIS
![NIS Plot](visualizations/nisplot.png)
