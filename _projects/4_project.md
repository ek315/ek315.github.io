---
layout: page
title: Improving Performance of Hobbyist CNC Mill
description: Spring 2021, 2.72 - Elements of Mechanical Design project
img: assets/img/minicncmill_cover.jpg
importance: 5
category: coursework
---

<h3>Skills Demonstrated</h3>
<style>
    .horizontal-word-bullets {
        list-style-type: none; /* Remove default bullets */
        padding: 0;
        margin: 0;
        display: flex; /* Use flexbox to display items horizontally */
        flex-wrap: wrap; /* Allow items to wrap to the next line */
        gap: 10px; /* Adjust the gap between items */
    }

    .horizontal-word-bullets li {
        white-space: nowrap; /* Prevent line breaks */
        display: inline-block; /* Keep items on the same line */
        margin-bottom: 2px; /* Add some space between rows */
        
        padding: 2px 2px; /* Padding for each item */
        border-radius: 5px; /* Rounded corners for each item */
    }

    .horizontal-word-bullets li::before {
        content: "•"; /* Unicode character for bullet (use \2022 for a bullet) */
        margin-right: 5px; /* Adjust spacing between bullet and text */
    }
</style>

<ul class="horizontal-word-bullets">
  <li>Team Work</li>
  <li>Simulation Experiments</li>
  <li>Physical Hardware Experiments</li>
  <li>Matlab</li>
  <li>Stress Analysis</li>
  <li>Machine Design</li>
</ul>


<div class="row">
    <div class="col-sm mt-3 mt-md-0 d-flex justify-content-center">
        {% include figure.liquid loading="eager" path="assets/img/mechedesign_snapmaker.png"  title="example image" class="img-fluid rounded z-depth-1" width ="45%" %}
    </div>
</div>

<h3>Project Description</h3>
<p>This purpose of this project was to improve certian performance metrics of the Snap Maker 1.0. This included:</p>

<ol>
  <li>Reduce total position error in y to < 100 μm</li>
  <li>Kinematic coupling repeatability in positioning in x and y to be < 25 μm</li>
  <li>Deflection of Kinematic coupling in x,y,& z < 25 μm</li>
  <li>Improve axes alignment to <0.5 degrees</li>
  <li>Decrease nosie level 30 cm away to less than 75 dB</li>
  <li>Vibration deflection to less than 25 μm</li>
</ol>

Additionally, we made small design changes to the sliding carriage to increase stiffness to reduce position error at the tool tip.


<div class="row justify-content-center">
    <div class="col-sm-8 mt-3 mt-md-0 mx-auto">
        {% include video.liquid path="assets/img/mechdesign_video.mp4"
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

<!-- <div class="caption">
    Problem: play in sliding carriage due to lack of preload on bearings.
</div> -->
<p> Above shows a source of the positional error - play in the sliding carriage due to a lack of preload on the bearings. </p> 

<div class="row justify-content-center">
    <div class="col-sm-8 mt-3 mt-md-0 mx-auto">
        {% include figure.liquid loading="eager" path="assets/img/mechedesign_carriage.png"  title="example image" class="img-fluid rounded z-depth-1" width ="45%" %}
    </div>
</div>

 <p> Above shows the design changes to properly preload the bearings.</p> 
<!-- <div class="caption">
    Solution: design change in carriage to properly preload bearings.
</div> -->



<h3>Results:</h3>

<ul>
  <li>Reduced tool tip deflection from 0.060” to 0.039” (1.52 mm to 0.99 mm) under applied load of 𝐹_𝑦=-15 N (35% reduction in error).
</li>
  <li>Kinematic Coupling: Repeatability: x, y = 0.001” (25.4 μm) Deflection: < 25.4 μm/0.001”  for 15 N load in x, y, z
</li>
  <li>Z and Y rail: 𝜃_𝑧 = 0.21° -> 𝜃_𝑧 = 0.0713° angular misalignment, => 34% reduction, Z to X rail: 𝜃_𝑧 = 0.5° -> 𝜃_𝑧 = 0.2° => 60% reduction
</li>
<li>Decreased reduced measured deflection at CNC head by 0.002” & noise by 10 dB
</li>
</ul>




<h3>Learn More:</h3>
<p><a href="/assets/2.72_ProjectPresentation_EmilyKamienski.pptx" target="_blank">Presentation</a></p>