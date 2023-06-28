---
title: Harmonic Motion Analyzer
summary: MATLAB program to analyze motion of a target object.

tags:
- Computer vision
- Image processing

date: "2018-05-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link:

image:
  caption: Sample Result
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: GitHub
  url: https://github.com/khush3/HarmonicMotionAnalyser
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---
### Abstract
Simple harmonic motion can serve as a mathematical model for a variety of motions, such as the oscillation of a spring. Intending to learn computer vision and MATLAB, I worked on analyzing the motion of a target-object undergoing a damped harmonic motion. The target-object was separated from the background using color thresholding and estimated as a point object. Coordinates of this point were recorded and used to estimate the parameters associated with the mathematical model of the system like maximum displacement, mean position, the velocity at different time instants. A mathematical model was estimated by fitting a curve to the recorded data using MATLAB Curve Fitting Toolbox.
### Contributions
- Estimated the equation of motion of a target-object video is selected to analyze its motion.
- Retrieved data associated with the motion of target-object using  elementary mathematics.
- *This project was made for TechnoSeason, 2017 and was awarded first prize.*