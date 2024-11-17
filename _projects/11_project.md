---
layout: page
title: Estimating Fall Risk
description: Masters/Phd Research
img: assets/img/fall_pred_overview.png
importance: 1
category: research
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
  <li>Machine Learning</li>
  <li>Robotics & Control</li>
  <li>Human Subject Testing</li>
  <li>Python</li>
  <li>Pytorch</li>
  <li>CAD</li>
</ul>



<h3>Project Description</h3>

<p>This project includes advancements in predicting falls using data driven methods and exploring novel physical injury prevention mechanisms. Data is gathered from human subjects experiencing various loss-of-balance scenarios while utilizing a walker. A predictive model based on multiple Long-Short Term Memory (LSTM) networks is formulated using three innovative approaches. Initially, distinct fall types are identified from limited data by learning rapid and gradual falls separately. Next, a "Timer LSTM" is developed to estimate the remaining time before an imbalance becomes irrecoverable and requires activating the fall prevention mechanism. Subsequently, if time permits, additional data is collected and further evaluated for the potential of a fall. This methodology reduced the false positive rate in fall prediction. Additionally, complex cases are analyzed using a metric of data insufficiency termed the Lipschitz quotient. Features that reduce the Lipschitz quotients, thus enhancing data predictability, are identified and included with the original input signals. </p>



<h3>Outcome</h3>

<p>Using these additional features further enhanced performance, with the most effective model achieving a 97% success rate in identifying falls at a 0.17% false positive rate. The predictive approach is implemented within an innovative walker-type fall prediction and prevention prototype. This walker has high maneuverability due to its compact footprint and becomes untippable by deploying its expandable legs when a fall is predicted.</p>


<div class="row">
    <div class="col-sm mt-3 mt-md-0 d-flex justify-content-center">
        {% include figure.liquid loading="eager" path="assets/img/fall_pred_overview.png"  title="example image" class="img-fluid rounded z-depth-1" width ="98%" %}
    </div>
</div>



<h3> Paper: </h3>
<a href="https://ieeexplore.ieee.org/document/10374122" target="_blank">Paper</a>