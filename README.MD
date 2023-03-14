# Yellow Line Follower

This program subscribes to an RGB image topic from a camera and attempts to follow a yellow line in the image. It does so by filtering everything else that isn't yellow and creating a centroid that follows the yellow line. If the centroid is not in the center, the robot will turn to where it is, staying on the yellow line. If the yellow line is lost, the robot stops moving and turns around to search for the line again, creating an infinite loop. 

### Run this program

In one termial tab run 

```bash
roslaunch prrexamples linemission.launch model:=waffle
```

In another run
```bash
rosrun follow_line follow.py
```
