---
layout: post
author: Ayoub
date: 2022-07-19
title: Camera Calibration
description: In this post we will review what's camera calibration, why it's needed and how to do it.
tags: camera calibration computer-vision python camera-calibration
---

- [Camera Calibration Theory](#camera-calibration-theory)
  - [Why camera calibration ?](#why-camera-calibration-)
  - [Different Classifications:](#different-classifications)
- [References:](#references)

In this post we will review what's camera calibration, why it's needed and how to do it.

## Camera Calibration Theory

### Why camera calibration ?

- When setting up a measurement system, it has to be carefully calibrated before any use, to get accurate results measurements. (Yes! you can use camera to take measures, see e.g. _photogrammetry_)

- To remove the distortions introduced by the camera [lens]

- Ensure that the features of the image behave according to the laws of projective geometry (The most important preserved property is _COLINEARITY_)

- Definition of the precise direction of the projection ray for each pixel.

### Different Classifications:

**1**. **Linear** vs **Non-linear**: "usually differentiated depending on the modelling of lens distortion".

**2**. **Intrinsic** vs **Extrinsic**: "Intrinsic calibration is concerned only with obtaining the physical and optical parameters of the camera. Besides, extrinsic calibration concerns the measurement of the position and orientation of the camera in the scene".

**3**. **Implicit** vs **Explicit**: "Implicit calibration is the process of calibrating a camera without explicitly computing its physical parameters. Although, the results can be used for 3D measurement and the generation of image coordinates, they are useless for camera modelling as the obtained parameters do not correspond to the physical ones".

**4**. **Use of 3D points** vs **Use of geometrical properties**: "the methods which use known 3D points as a calibrating pattern or even a reduced set of 3D points, with respect to others which use geometrical properties in the scene such as vanishing lines or other line features".

## References:

- Salvi, Joaquim, Xavier Armangué, and Joan Batlle. “A Comparative Review of Camera Calibrating Methods with Accuracy Evaluation.” Pattern Recognition 35, no. 7 (July 2002): 1617–35. https://doi.org/10.1016/S0031-3203(01)00126-1.
