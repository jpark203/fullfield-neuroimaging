---
layout: page
permalink: /stimuli/
title: Stimuli
description: 
nav: true
nav_order: 3
---

<blockquote style="background-color: #f2e6ff;">
<strong><em>Key Idea</em></strong> : 
Images should have compatible properties (e.g., field-of-view, height of camera) to avoid perceptual distortions of space. 
</blockquote>



<br>
- <span style="font-size: 22px;"> The compatible Field-of-View (FOV) was crucial for a wide screen. </span>
    - <span style="font-size: 18px;"> The Field-of-View is the angular extent of the world that can be seen at any given moment. It can be mesured horizontally or vertically. </span>
    - <span style="font-size: 18px;"> Typically, humans have a binocular FOV of around 120 deg horizontally. </span>
    <div style="padding: 10px; text-align: center;">
        <img src="../images/FieldofView-1.jpg" alt="FOV" style="width: 60%; height: auto; margin: 0 auto;">
        <figcaption><em>Horizontal FOV</em></figcaption>
    </div>
    - <span style="font-size: 18px;"> However, when taking a picture, the FOV can be varied across a wide range, depending on the camera settings. </span>
    - <span style="font-size: 18px;"> When an image taken with a narrow FOV is projected onto a much wider screen (e.g., our custom-built screen), viewers are prone to experience distortions of space. </span>


<br>
- <span style="font-size: 22px;"> How do we ensure the wide FOV for stimuli? </span>
    - <span style="font-size: 18px;"> We took advantage of virtual reality (VR) game engine, where we have a complete control over the FOV and other camera parameters. </span>
    - <span style="font-size: 18px;"> The camera FOV was set at 120.2 deg horozontally and 105 deg vertically. </span>
    <div style="padding: 10px; text-align: center;">
        <img src="../images/fov_unity.003.jpeg" alt="FOV-unity" style="width: 75%; height: auto; margin: 0 auto;">
        <figcaption><em>Horizontal FOV in VR</em></figcaption>
    </div>
    - <span style="font-size: 18px;"> This FOV was chosen based on the chord angle of our physical screen (120 deg) and empirical testing by experimenters. </span>
    - <span style="font-size: 18px;"> Since there was no ground truth for the size of VR environments (e.g., how large the space should be), experimenters compared a few different FOVs and made subjective judgements on which parameter feels most natural. </span>



<br>
- <span style="font-size: 22px;"> Other camera parameters were also set to mimic the view of an adult standing in a room looking at the object on the back counter/surface. </span>
    - <span style="font-size: 18px;"> E.g., the height was set to be 1.6 (arbitrary units), and the angle was tilted down (about 5.2 deg) such that the center object was always at the center of the image. </span>
    - <span style="font-size: 18px;"> Note that these parameter values are specific to our VR environments.
    - <span style="font-size: 18px;"> With these camera parameters, we rendered an image view for each VR environment. </span>
    - <span style="font-size: 18px;"> The captured images were 1024 x 768 pixels 2D images, and later computationally warped before the projection. </span>


<br>
- - -

<!-- <br> -->
- <span style="font-size: 22px;"> All VR environments were generated using the Unity game engine (Version 2017.3.0).</span>
    - <span style="font-size: 18px;"> All rooms had the same physical dimensions (4 width x 3 height x 6 depth arbitrary units).</span>
    - <span style="font-size: 18px;"> Each environment has an extended horizontal surface along the back wall, containing a centrally positioned object. Then, the room was additionally populated with the kinds of objects typically encountered in those locations, creating naturalistic computer generated images. </span>
    - <span style="font-size: 18px;"> These environments were also used in Park, Josephs, & Konkle 
    ([2021](https://psyarxiv.com/84exs);
    [2022](https://konklab.fas.harvard.edu/Papers/Park_2022_SciReports.pdf)). </span>
