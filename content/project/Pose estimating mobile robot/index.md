---
title: 2-Dimensional Localization
summary: Algorithm and Hardware for 2-D pose estimation.

tags:
- Electronics
- Embedded systems
- Robotics

date: "2018-05-01T00:00:00Z"

image:
  caption: Custom built mobile robot setup
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: GitHub
  url: http://www.ivlabs.in/mobile-robot.html
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---
### Abstract
Robot localization is the process of determining where a mobile robot is located with respect to its environment. Localization is one of the most fundamental competencies required by an autonomous robot as the knowledge of the robot's own location is an essential precursor to making decisions about future actions. In the summer of my freshman year, I worked on developing an algorithm to localize a differential-drive robot using odometry from scratch. I performed UMBmark test to calibrate robot base and wheel diameter constants. Besides this, I also developed the hardware for the robot.
### Contributions
- Designed algorithm for pose (rectangular coordinates, angle) estimation of a robot in a two dimensional plane using odometry, and developed the hardware for robot.
- Used ROS framework to establish communication between the nodes.
- Performed UMBmark test to calibrate robot base and wheel diameter constants.
### Results
![](https://media.giphy.com/media/MdSNDislPQsoyDL4Is/giphy.gif)

|               | MEASURED DATA | REAL-TIME DATA | ACCURACY |
| :-----------: | :-----------: | :------------: | :------: |
| **ABSCISSA**  |    25.4 cm    |    25.2 cm     |  99.3%   |
| **ORDINATE**  |    8.3 cm     |     8.3 cm     |   100%   |
|   **ANGLE**   | 357.1 degree  |   356 degree   |  99.7%   |
