# Unscented Kalman Filter Project Starter Code
Self-Driving Car Engineer Nanodegree Program

In this project utilize an Unscented Kalman Filter to estimate the state of a moving object of interest with noisy lidar and radar measurements. Passing the project requires obtaining RMSE values that are lower that the tolerance outlined in the project rubric. 

## Your code should compile.
It compiles fine

# Accuracy
Criteria 	Meets Specifications

px, py, vx, vy output coordinates must have an RMSE <= [.09, .10, .40, .30] when using the file: "obj_pose-laser-radar-synthetic-input.txt", which is the same data file the simulator uses for Dataset 1.

I get RMS<=[0.0678,0.0831,0.3379,0.2211]

Hints are:
 - Init P_ .- I forgot to init it and yawd variance explodes
 - Not normalize angles	


# Criteria 	Meets Specifications

Your Sensor Fusion algorithm follows the general processing flow as taught in the preceding lessons.
	

While you may be creative with your implementation, there is a well-defined set of steps that must take place in order to successfully build a Kalman Filter. As such, your project should follow the algorithm as described in the preceding lesson.

# Your Kalman Filter algorithm handles the first measurements appropriately.	

## Your algorithm should use the first measurements to initialize the state vectors and covariance matrices.
Actually I have learned the lesson I didn't do it and after a good initialization everything started to work fine.


## Your Kalman Filter algorithm first predicts then updates.
Yes It does in that order.
	

## Your Kalman Filter can handle radar and lidar measurements.

Lidar update is usual kalman filter and radar is unscented.
	

# Your algorithm should avoid unnecessary calculations.

I init weights just at the beginning and pass parameters by reference when as much as I can.

