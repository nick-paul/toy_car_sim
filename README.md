# Toy Car Simulation

![](images/screenshot.png)

Workspace for simulation a toy Ackermann vehicle

## Setup

### Clone this repo

Note that this repo it a workspace. Clone it into your home directory.

```
$ cd
$ git clone <this repo>
```

### `ros_control`

Install `ros-control` packages:

```
sudo apt-get install ros-kinetic-ros-control ros-kinetic-ros-controllers
```

### Build

```
$ cd ~/toy_car_sim
$ catkin_make
```

### Floor Model

Go into the models directory and run the following script:

```
$ cd ~/toy_car_sim/models
$ sh copy_model.sh
```

## Running 

```
roslaunch ackermann_vehicle_gazebo ackermann_vehicle.launch
```

### Topics

  - **Camera:** `/car/camera1/image_raw`
  - Twist command: `/prizm_twist_controller/twist_cmd`
