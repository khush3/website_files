---
title: Snake-like robots
summary: ROS packages for simulating and controlling biorobotics lab snake robots.

tags:
- Electronics
- Embedded systems
- Robotics
- ROS

date: "2023-04-01T00:00:00Z"

image:
  caption: ReU snake robot performing pole climbing
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: GitHub
  url: https://github.com/biorobotics/snakelib

- icon: youtube
  icon_pack: fab
  name: Demos
  url: https://www.youtube.com/playlist?list=PLflR-cYaxOGET1BmFWb5yX3YfZ67EYmAv

---

### Abstract
SnakeLib is a ROS-based package that holds past gait research on modular snake robots and serves as a platform to facilitate further development. SnakeLib’s basic gait implementations provide a user-friendly and intuitive way to operate the robot with a joystick.

### Contributions
- A set of ROS packages for simulating and controlling Biorobotics Lab snake robots.
- ROS based software to control ReU, SEA, and RSnake snake robots, receive sensor feedback, and create visualizations.
- ROS diagram
- HEBI ros node for sending joint commands to HEBI electronics and reading sensor feedback
- Camera node to read camera in the ReU snakehead
- Gait library to host manually programmed snake gaits
- Joystick node to convert joystick inputs to snake commands
- Robot class for easy to use IK and FK implementations
- RViz and PyQt based GUI to visualize state and camera feedback
- Snake state node for virtual chassis implementation for robot state visualization
- GUI node to create PyQt interface

### Demos
#### Sidewinding
<details><summary>Summary</summary>
$$
\alpha(n, t) = \beta_{even} + A_{even}sin(\omega_{t, even}t + \omega_{s, even}n) \forall \text{even n}
$$
$$
\alpha(n, t) = \beta_{odd} + A_{odd}sin(\omega_{t, odd} + \omega_{s, odd}n) \forall \text{odd n}
$$
Sideways moving gait inspired by snake's <a href="https://en.wikipedia.org/wiki/Sidewinding">sidewinding</a> motion.
</details>
<iframe width="854" height="480" src="https://www.youtube.com/embed/ca5w6SdWUuA" title="ReU - Sidewinding" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

#### Rolling
<details><summary>Summary</summary>
$$
\alpha(n, t) = \beta_{even} + A_{even}sin(\omega_{t, even}t + \omega_{s, even}n) \forall \text{even n}
$$
$$
\alpha(n, t) = \beta_{odd} + A_{odd}sin(\omega_{t, odd} + \omega_{s, odd}n) \forall \text{odd n}
$$
Sideways moving gait inspired rolling motion of a body. Here, the wave only propogates in time (i.e., $\omega_s = 0$) and the horizontal and vertical waves are offset by $\pi/2$.
</details>
<iframe width="854" height="480" src="https://www.youtube.com/embed/uk6MReCvLy8" title="ReU - Rolling" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

#### Linear progression
<details><summary>Summary</summary>
$$
\alpha(n, t) = \beta_{even} + A_{even}sin(\omega_{t, even}t + \omega_{s, even}n) \forall \text{even n}
$$
$$
\alpha(n, t) = \beta_{odd} + A_{odd}sin(\omega_{t, odd} + \omega_{s, odd}n) \forall \text{odd n}
$$
</details>
<iframe width="854" height="480" src="https://www.youtube.com/embed/VseLw1O8en0" title="ReU - Linear progression" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

#### Pole climbing
<details><summary>Summary</summary>
</details>
<iframe width="854" height="480" src="https://www.youtube.com/embed/ITlWLMf-Vw0" title="ReU - pole climbing" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

#### IK-based headlook
<details><summary>Summary</summary>
$$
\dot{q} = J(q)^{+}v
$$
Here, <br>
$\dot{q}$: Joint velocities <br>
$J^{+}$: Pseudo-inverse of the jacobian <br>
$v$: End-effector velocity <br>
Controls the end-effector (snake head) in cartesian space using inverse jacobian approach.
</details>
<iframe width="854" height="480" src="https://www.youtube.com/embed/7KOV2xjcpLo" title="ReU - IK-based headlook" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

#### Slithering
<details><summary>Summary</summary>
Forward moving gait inspired by snake's [slithering](https://en.wikipedia.org/wiki/Snake_locomotion#Slithering) motion.
</details>
<iframe width="854" height="480" src="https://www.youtube.com/embed/i-T2Yt1NjIw" title="ReU- slithering" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

#### Turn-in-place
<details><summary>Summary</summary>
$$
\alpha(n, t) = \beta_{even} + A_{even}sin(\omega_{t, even}t + \omega_{s, even}n) \forall \text{even n}
$$
$$
\alpha(n, t) = \beta_{odd} + A_{odd}sin(\omega_{t, odd} + \omega_{s, odd}n) \forall \text{odd n}
$$
Implemented by running opposite direction <a href="#sidewinding">sidewinding</a> gait in two halfs of the snake robot.
</details>
<iframe width="854" height="480" src="https://www.youtube.com/embed/b6cp0hJg4nQ" title="ReU - Turn-in-place" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<!-- [Check out the complete demonstration.](https://www.youtube.com/watch?v=XnrbU1050ls) -->
