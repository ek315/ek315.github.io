---
layout: page
title: Optimizing Arm Swing for a Jumping Robot
description: Fall 2022, 2.740 - Bioinspired Robotics project
img: assets/img/jumping_robot_cover.png
redirect: 
importance: 3
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
  <li>Robotics & Control</li>
  <li>Simulation Experiments</li>
  <li>Physical Hardware Experiments</li>
  <li>Parameter Sweep</li>
  <li>C++</li>
  <li>Matlab</li>
  <li>mbed Microcontroller</li>
</ul>

<h3>Project Description</h3>
<p>Inspired by the way humans perform vertical jumps, in this project we studied the effect of arm swing loading of an elastic ankle joint on the jump height of a jumping robot.

Our hypotheses included:</p>

<ol>
  <li>Arm swing, in the presence of an elastic ankle, can increase maximum jump height</li>
  <li>The timing of the arm swing relative to the leg’s actuation time affects maximum jump height</li>
  <li>There exists an optimal arm swing timing that maximally exploits the elastic ankle for maximum jump height</li>
</ol>

Our device consisted of a robot with an actuated hip and shoulder joint, and a spring loaded ankle. We tested our hypotheses by measuring the maximum jump height achieved while varying the time delay between the shoulder and hip activation time and with and without arm swing. Experiments were performed with a simplified model in simulation and on physical hardware.

<div class="row">
    <div class="col-sm mt-3 mt-md-0 d-flex justify-content-center">
        {% include figure.liquid loading="eager" path="assets/img/jumping_robot_model.png" title="example image" class="img-fluid rounded z-depth-1" width ="75%" %}
    </div>
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0 d-flex justify-content-center">
        {% include figure.liquid loading="eager" path="assets/img/jumping_robot_results.png" title="example image" class="img-fluid rounded z-depth-1" width ="75%" %}
    </div>
</div>

<!-- <h3>Responsibilities</h3> -->

<h3>Learn More:</h3>
<p><a href="/assets/img/2.74_Presentation.pptx" target="_blank">Presentation</a></p>