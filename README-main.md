# Autonomous Robotics PAs

## What

### Overview

This repository is a collection of programming assignments ('PAs') for
Brandeis University's COSI 119: Autonomous Robotics course.

More precisely, it is a ROS workspace with five ROS packages:

1. `basic_mover`
2. `fiducial_nav`
3. `line_follower`
4. `maze_solver`
5. `wall_follower`

Each ROS package corresponds to a PA, and contains a README that describes the
package.

The 'real' versions of the code were tested on robc. They might have to be
tweaked to work on other robots.

### Details

Under the `src` directory of each package there is code relevant to the PA. For
every skeleton code `f.py` file that a student is expected to complete, there is
a corresponding `f_answer.py` file that contains a possible solution to the
skeleton.

Some of the packages also contain launch files under a `launch` directory. These
files shouldn't need changing, with the possible exception of
`fiducial_real.launch` in the `fiducial_nav` package. Here, the instructor may
want to modify the arguments to `aruco_detect` as necessary, or guide students
on how to do so (e.g., by adjusting the values of `fiducial_len` or
`dictionary`).

Finally, some packages contain `models` and `worlds` directories that are used
in running Gazebo simulations for their PAs. These should work as is.

## Why

This project was prepared for the Fall 2024 iteration of COSI 119.

## Acknowledgments

The aruco marker models used in the `fiducial_nav` package were developed by
[Jose-Luis Sanchez-Lopez](https://github.com/joselusl) and used with his
permission.
