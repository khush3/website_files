+++
title = "Deep Learning-Based Stair Segmentation and Behavioral Cloning for Autonomous Stair Climbing"
date = 2019-12-01
authors = ["Navid Panchi", "**Khush Agrawal**", "Unmesh Patil", "Aniket Gujarathi", "Aman Jain", "Harsha Namdeo", "Shital S. Chiddarwar"]
publication_types = ["2"]

doi = "10.1142/S1793351X1940021X"
url_pdf = "https://drive.google.com/open?id=1swoHdIl4URGnOhiIu5IoJjmORl-KN76x"
url_video = "https://www.youtube.com/playlist?list=PLflR-cYaxOGFrR4ejMU8Mt5ZF5mPCZNmv"
url_code = "https://github.com/IvLabs/autonomous_stair_climbing_robot_v2"

abstract = "Mobile robots are widely used in the surveillance industry, for military and industrial applications. In order to carry out surveillance tasks like urban search and rescue operations, the ability to traverse stairs is of immense significance. This paper presents a deep learning based approach for semantic segmentation of stairs, behavioral cloning for star alignment, and a novel mechanical design for an autonomous stair climbing robot. The main objective is to solve the problem of locomotion over staircases with the proposed implementation. Alignment of a robot with stairs in an image is a traditional problem, and the most recent approaches are centred around hand-crafted texture-based Gabor filters and stair detection techniques. However, we could arrive at a more scalable and robust pipeline for alignment schemes. The proposed deep learning technique eliminates the need for manual tuning of parameters of the edge detector, the Hough accumulator, and PID constants. The empirical results and architecture of the stair alignment pipeline are demonstrated in this paper."
featured = true

publication = "*International Journal of Semantic Computing*"

+++
### Qualitative results

#### Stair segmentation
<iframe width="854" height="480" src="https://www.youtube.com/embed/agxyvn9lQmk" title="Stair Segmentation Results" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
We use a U-Net model for segmenting the stairs in the RGBD image input.

#### Stair alignment
<iframe width="854" height="480" src="https://www.youtube.com/embed/qudH-cXtLvo" title="Behavior Cloning Model Results" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
We use behavior cloning to learn a model that predicts actions (turn left/right, move forwards/backwards) per time step to align the TurtleBot2 with the stairs, given a segmented image of the stairs.

### Quantitative results
![](https://user-images.githubusercontent.com/34411770/74923881-89ac0100-53f7-11ea-9f8b-030d230c99db.png)