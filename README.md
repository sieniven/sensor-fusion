# Senor Fusion with State Estimation techniques

[//]: # (Image References)

[image1]: ./sensor-fusion-using-ekf/data/dataset_1_results.png "Dataset 1 Results"
[image2]: ./sensor-fusion-using-ekf/data/dataset_2_results.png "Dataset 2 Results"

## Introduction

Hello and welcome to my project on sensor fusion! This project is to develop methodologies for fusing various sensors together to improve perception capabilities in autonomous systems. In my project, I have developed an algorithm that implements a kalman filter to estimate the state of a moving object of interest with noisy lidar and radar measurements. We evaluate our estimations using root mean square error values (RMSE).


## Setup

This project involves the use of a simulator which can be downloaded [here](https://github.com/udacity/self-driving-car-sim/releases).

This repository includes two files that can be used to set up and install [uWebSocketIO](https://github.com/uWebSockets/uWebSockets) for either Linux or Mac systems. For windows you can use either Docker, VMware, or even [Windows 10 Bash on Ubuntu](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/) to install uWebSocketIO. Please see the uWebSocketIO Starter Guide page in the classroom within the EKF Project lesson for the required version and installation scripts.

Once the install for uWebSocketIO is complete, the main program can be built and run by doing the following from the project top directory.

1. mkdir build
2. cd build
3. cmake ..
4. make
5. ./ExtendedKF


## Dependencies

* cmake >= 3.5
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)


## Results

I ran our extended kalman filter software with the dataset containing lidar and radar measurements to test the software, and obtained the results as seen below.

![image1][image1]

The results above is applied on dataset 1, which is our original dataset. Subsequently, I applied the algorithm on dataset 2, which is the reversed version of dataset 1.

![image2][image2]