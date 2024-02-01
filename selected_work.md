---
layout: page
title: Selected Work
---

<style>
    /* Style for grid layout */
    .grid-container {
    display: grid;
    grid-template-columns: repeat(auto-fill, 200px);
    gap: 20px;
    padding: 20px;
    }

    .grid-item {
        position: relative;
        overflow: hidden;
        
    }

    .grid-item img {
        width: 100%;
        height: auto;
        display: block;
        transition: transform 0.3s ease;
    }

    .overlay {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
         text-align: center; /* Center-align the text */
        background-color: rgba(255, 255, 255, 0.7) /* Semi-transparent black background */
        color: black; /* Set text color to white */
        padding: 8px 12px; /* Adjust padding as needed */
        border-radius: 4px;
        transition: opacity 0.3s ease;
        opacity: 0;
        pointer-events: none;
        font-size: 20px; /* Increase text size */
        font-weight: bold; /* Make text bold */
    }

    .grid-item:hover::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(255, 255, 255, 0); /* Initialize mask as transparent */
        transition: background-color 0.3s ease; /* Transition for mask color change */
        pointer-events: none;
    }



    .grid-item:hover::before {
        background-color: rgba(255, 255, 255, 0.7); /* White mask over image on hover */
    }

    .grid-item:hover .overlay {
        opacity: 1; /* Show the overlay on hover */
    }
    
</style>




<div class="grid-container">
    <!-- Each anchor tag wraps an image and links to a different HTML file -->
    <div class="grid-item">
        <a href="fall_prediction.html">
            <img src="/assets/fall_pred_cover.png" alt="Image 1">
             <div class="overlay">Fall Prediction & Prevention</div>
        </a>
    </div>
    <div class="grid-item">
        <a href="aorta_mapping.html">
            <img src="/assets/aorta_cover.png" alt="Image 3">
            <div class="overlay">Aorta Mapping</div>
        </a>
    </div>
    <div class="grid-item">
        <a href="jumping_robot.html">
            <img src="/assets/jumping_robot_cover.png" alt="Image 2">
            <div class="overlay">Optimizing Arm Swing for Jumping Robot</div>
        </a>
    </div>
    <div class="grid-item">
        <a href="underactuated_project.html">
            <img src="/assets/underactuated_cover.png" alt="Image 2">
            <div class="overlay">Trajectory Optimization of Active Compass Gait Walker</div>
        </a>
    </div>
    <div class="grid-item">
        <a href="mechdesign.html">
            <img src="/assets/minicncmill_cover.jpg" alt="Image 2">
            <div class="overlay">Mech. Design Improvements of CNC Mill</div>
        </a>
    </div>
     <div class="grid-item">
        <a href="tree_robot.html">
            <img src="/assets/tree_robot_cover.png" alt="Image 2">
            <div class="overlay">Tree Robot</div>
        </a>
    </div>
    <div class="grid-item">
        <a href="3dprinter.html">
            <img src="/assets/3dprinter_cover.jpg" alt="Image 2">
            <div class="overlay">Prusa i3 3D Printer Build</div>
        </a>
    </div>

    <!-- Add more grid items for additional images -->
</div>