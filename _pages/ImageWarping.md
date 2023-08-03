---
layout: page
permalink: /warping/
title: ImageWarping
description: 
nav: true
nav_order: 4
---

#### **Problems and Goals**
- <span style="font-size: 18px;"> Due to physical constraints of scanner room (e.g., location of projector, projection angle), only a part of display pixels (currently about 30%) can be projected onto a screen, and the rest of pixels fall outside of the screen. Thus, it is crucial to know which pixels are actually usable for presenting stimuli. </span>
- <span style="font-size: 18px;"> A regular image looks distorted, because the screen is curved and tilted from a participant’s eyes. Thus, a projected image needs to be warped in a reverse direction, such that the image on the curved screen looks “normal”. </span>


<br>
#### **Compute the shape of screen**
<figure style="display: flex; align-items: center;">
  <div style="padding: 10px;">
    <img src="../images/imageWarping_helpers.001.png" alt="Image 1" style="width: 100%; height: auto;">
    <!-- <figcaption style="text-align: center;"></figcaption> -->
  </div>
  <div style="padding: 10px;">
    <img src="../images/imageWarping_helpers.002.png" alt="Image 2" style="width: 100%; height: auto;">
    <!-- <figcaption style="text-align: center;">Back</figcaption> -->
  </div>
</figure>

- <span style="font-size: 18px;"> Get 3 or more coordinates (dots) along a horizontal axis of the screen using mouse clicks.  </span>
- <span style="font-size: 18px;"> Using those dot coordinates, fit a curve. </span>
- <span style="font-size: 18px;"> Compute the curvature separately for upper and lower screen boundary as the curvature is slightly different. </span>
- <span style="font-size: 18px;"> Compute the curvature of horizontal lines between the upper and lower boundary by interpolating them. </span>
- <span style="font-size: 18px;"> This step results in the shape of screen, described in terms of coordinates within the display resolution. </span>


<br>
#### **Map input image to the screen shape**
- <span style="font-size: 18px;"> Now we have the number of usable pixels (i.e., can be projected onto the screen) for each X and Y axis.</span>
- <span style="font-size: 18px;"> However, the number of those pixels will be lower than the original input image. Thus, we need to downsample the input image. </span>
- <span style="font-size: 18px;"> This step results in the mapping function indicating which pixel in the input image should be mapped onto a pixel in the output image (curved screen). </span>


<div style="padding: 10px;">
    <img src="../images/warp_example.jpeg" alt="img transform" style="width: 100%; height: auto;">
    <figcaption style="text-align: center;"><em>Image Warping Example</em></figcaption>
</div>


<br><br>
- - - - 
#### **Warping Code**

- <span style="font-size: 18px;"> The code for image warping is available on GitHub. </span>
- <span style="font-size: 18px;"> Click [HERE](https://github.com/jpark203/FullField-ImageWapring.git) </span>
