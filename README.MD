# Yellow Line Follower

This program subscribes to an RGB image topic from a camera and attempts to follow a yellow line in the image. It does so by filtering out everything that isn't yellow and creating a centroid that follows the yellow line. If the centroid is not in the center, the robot will turn towards it and stay on the yellow line. If the yellow line is lost, the robot stops moving and turns around to search for the line again, creating an infinite loop.

### Run this program

To run this program, open a terminal and enter the following commands:

```bash
roslaunch prrexamples linemission.launch model:=waffle
```

```bash
rosrun follow_line follow.py
```

### Video Demo 

Here's a link to a video of the program running: https://brandeis.zoom.us/rec/share/gtFx7cQMK62fgG6wIHmXvKNlsrO4kxQOm8JVOkT5ii_fQdtFw5a9rn4XIZuNk-wl.1v5dEorXYZKIQAOs



