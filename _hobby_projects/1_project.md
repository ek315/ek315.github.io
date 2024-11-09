---
layout: page
title: End grain cutting board
description: Fall 2023 - Visual Navigation for Autonomous Vehicles Final Project
img: assets/img/aorta_cover.png
importance: 1
category: woodworking
related_publications: true
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




<br/><br/>
<center>
    <img src="/assets/aorta_training.png" style="width:90%;"/>
</center>
<span style="font-size:medium;">



<!-- <br/><br/>
<center>
    <img src="/assets/aorta_mesh.png" style="width:60%;"/>
</center>
<span style="font-size:medium;"> -->

<br/><br/>
<center>
<video width="640" height="480" autoplay muted>
  <source src="/assets/aorta_mesh_video.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
</center>

<!-- <br/><br/>
<center>
    <img src="/assets/aorta_error.png" style="width:70%;"/>
</center>
<span style="font-size:medium;"> -->

<h3>Learn More:</h3>
<p><a href="https://" target="_blank">Presentation</a></p>
<p><a href="https://" target="_blank">Report</a></p>

Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
