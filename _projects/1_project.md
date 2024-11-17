---
layout: page
title: Aorta Mapping
description: Fall 2023, 16.485 - Visual Navigation for Autonomous Vehicles project
img: assets/img/aorta_cover.png
importance: 1
category: coursework
related_publications: false
---

<h3>Skills Demonstrated</h3>
<style>
    .horizontal-word-bullets {
      list-style-type: none; /* Remove default bullets */
      padding: 0;
      margin: 0;
      display: flex; /* Use flexbox to display items horizontally */
    }

    .horizontal-word-bullets li {
      margin-right: 10px; /* Adjust spacing between list items */
      white-space: nowrap; /* Prevent line breaks */
    }

    .horizontal-word-bullets li::before {
      content: "•"; /* Unicode character for bullet (use \2022 for a bullet) */
      margin-right: 5px; /* Adjust spacing between bullet and text */
    }
</style>
<ul class="horizontal-word-bullets">
  <li>Team Work</li>
  <li>Machine Learning - CNN</li>
  <li>TSDF</li>
  <li>C++</li>
  <li>Python</li>
</ul>

<h3>Project Description</h3>

In this work we use data taken while inserting a surgical probe into a synthetic aorta model to reconstruct a 3D model of the dissected aorta. Note that this is part of a larger ongoing project conducted by Tom Dillon in the Therapeutic Technology Design & Development lab at MIT. The data consists of 2D ultrasound cross section images with accompanying 6DOF position data. A key challenge is to extract the 2D contour of the aortic wall and dissection flap. Ultrasound images are often noisy and the dissection flap can cause poor visualization of the far wall. We used machine learning to segment the two halves of the aorta to extract the contours for generating a 3D mesh using the truncated signed distance function (TSDF) and marching cubes algorithm. This enhanced visualization should aid surgeons performing aortic dissection operations.



<!-- <br/><br/>
<center>
    <img src="/assets/aorta_overview.png" style="width:50%;"/>
</center>
<span style="font-size:medium;"> -->

<h3>Responsibilities</h3>

I developed a CNN model using the UNet architecture to segment the ultrasound images. I then integrated this segmentation code with the Voxblox library TSDF implementation code to create a 3D mesh of the dissected aorta.

<div class="row">
    <div class="col-sm mt-3 mt-md-0 d-flex justify-content-center">
        {% include figure.liquid loading="eager" path="assets/img/aorta_training.png" title="example image" class="img-fluid rounded z-depth-1" width ="80%" %}
    </div>
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0 d-flex justify-content-center">
        {% include video.liquid path="assets/img/aorta_mesh_video.mp4"
                       width="80%" 
                       height="auto" 
                       autoplay="true" 
                       controls="true" 
                       loop="true" 
                       muted="true" 
                       class="img-fluid rounded z-depth-1" 
                      
        %}
    </div>
</div>

<!-- <br/><br/>
<center>
    <img src="assets/img/aorta_training.png" style="width:90%;"/>
</center>
<span style="font-size:medium;"> -->



<!-- <br/><br/>
<center>
    <img src="/assets/aorta_mesh.png" style="width:60%;"/>
</center>
<span style="font-size:medium;"> -->

<!-- <br/><br/>
<center>
<video width="640" height="480" autoplay muted>
  <source src="assets/img/aorta_mesh_video.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
</center> -->

<!-- <br/><br/>
<center>
    <img src="/assets/aorta_error.png" style="width:70%;"/>
</center>
<span style="font-size:medium;"> -->

<h3>Learn More:</h3>
<p><a href="https://" target="_blank">Presentation</a></p>
<p><a href="https://" target="_blank">Report</a></p>

