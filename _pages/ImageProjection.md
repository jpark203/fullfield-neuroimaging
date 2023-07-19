---
layout: page
permalink: /projection/
title: ImageProjection
description: 
nav: true
nav_order: 1
---

#### **MRI Room and Constraints**
- <span style="font-size: 18px;"> The Harvard CBS Neuroimaging facility relies on a LCD projector that is placed  on a stable table outside the shielded scanner room. In most visual experiments, images are projected onto a screen at the back of the bore that is viewed via a small mirror positioned above the subject’s eyes.
- <span style="font-size: 18px;"> To increase the spatial extent of stimulus, our goal was to project onto the inner wall of the cylinder bore. This simple idea is constrained by both physical and organizational limitations.
- <span style="font-size: 18px;"> The MRI serves many labs. Any alterations must be minimally intrusive so as not to alter the operation of any other ongoing study. Practically, this meant that we were discouraged from attaching anything, such as a uniform diffusive screen, to the scanner bore.
- <span style="font-size: 18px;"> We could not add structures to the space behind the scanner that would alter access to the space. Introducing a second projection system into the setup was not encouraged.

<div style="padding: 10px;">
    <img src="../images/mriRoomGeometry.png" alt="mri room" style="width: 100%; height: auto;">
    <figcaption style="text-align: center;"><em>General geometry of the room and our projection path</em></figcaption>
</div>


<br>
- - -
#### **Our Approach**
- <span style="font-size: 22px;"> Mirrors
    - <span style="font-size: 18px;"> We constructed an inverted periscope from a pair of front surface mirrors supported on a non-ferromagnetic stand. The lower mirror remains fixed, the upper mirror is hinged.
    - <span style="font-size: 18px;"> Tilting the mirror up removes the periscope from the projection path.
    - <span style="font-size: 18px;"> With the periscope in place, the projector appears to originate from a virtual point further back and below the floor of the room.

<div style="padding: 10px; text-align: center">
    <img src="../images/mirrorStand.png" alt="mirror stand" width="300">
    <figcaption style="text-align: center;"><em>A periscope stand with lower and upper mirrors</em></figcaption>
</div>


<br>
- <span style="font-size: 22px;"> Potential Projection Paths
    - <span style="font-size: 18px;"> Ideally, the projector would be incident on the screen at 90 degrees. The physical geometry of the scanner bore makes this near impossible. 
    - <span style="font-size: 18px;"> The next best solution would be to place the projector (or the final mirror) closer to the cylinder bore in order to obtain the steepest angle possible. We did not pursue this route for the reasons mentioned above.
    - <span style="font-size: 18px;"> If we projected directly onto the MRI bore, the light rays would be incident at just over 18 degrees. This shallow angle results in large distortion along the vertical (Y) axis of the projected image. 
    - <span style="font-size: 18px;"> To somewhat mitigate this, we angled the projection screen. Rather than being parallel to the magnet bore, we tilted it by 10 degrees.
    - <span style="font-size: 18px;"> The edge of the screen at the top of the subject’s head nearly touches the bore. The screen edge near their collarbone is closer to the subject than the bore. Tilting angles larger than 10 degrees were ruled out for reasons of comfort- eye strain, feelings of confinement, etc.


<br>
- <span style="font-size: 24px;"> Determined Projection Setup
    - <span style="font-size: 18px;"> The net result is that that projector is angled at just over 28 degrees relative to the screen.
    - <span style="font-size: 18px;"> As a result approximately 1⁄3 of the Y pixels of the projector fall onto the screen, limiting our vertical resolution to 284 pixels rather than the native 768.
    - <span style="font-size: 18px;"> The total screen extends over 2.3 degrees. The ultra long throw lens we used, ratio=9, creates an image that spans 4.8 degrees.
    - <span style="font-size: 18px;"> _**Note**_ : The current limits on the low resolution (i.e., number of pixels projected onto a screen) can be overcome by our new projector that has a much higher maximum resolution (4k). 

<div style="padding: 10px;">
    <img src="../images/setup_overall.png" alt="set up schema" style="width: 90%; height: auto;">
    <figcaption style="text-align: center;"><em>Image projection path</em></figcaption>
</div>