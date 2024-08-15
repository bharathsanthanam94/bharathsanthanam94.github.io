---
title: "3D mesh reconstruction of sweet peppers leveraging RGB textures"
excerpt: " Built a deep learning based 3D mesh reconstruction pipeline that uses color information in addition to point cloud to reconstruct meshes  <br/><img src='/images/mesh_reconstruction.png'>"
collection: portfolio
---
Abstract:

Project done in [agricultural robotics](https://agrobotics.uni-bonn.de/) lab, University of Bonn.

This project aims to address the challenging task of estimating highly detailed 3D shapes of fruits from sensor data captured in the laboratory and potentially
from the real-world field settings. Accurately estimating the 3D shapes of fruits has many benefits. For instance, such 3D models could enable the detection of damage or defects in the fruits, which can significantly reduce their value. By ensuring that only high-quality fruits are provided to consumers, this can help to improve customer
satisfaction and increase market value.

Key steps:

- This work builds upon the foundation laid by [Federico et al](https://www.ipb.uni-bonn.de/wp-content/papercite-data/pdf/magistri2024icra.pdf)., who trained a deep learning model to predict sweet pepper shapes using only partial views.

* Our project explores whether incorporating RGB information into the network adds value, as color differences are clearly visible in peppers with defects.

![pepper_mesh](/images/mesh_reconstruction.png)

Code credits: 
The code is fully developed by the authors of the previous work[ (link)](https://github.com/PRBonn/TCoRe). I only added the RGB projection part as an extention to investigates if it improves the mesh reconstruction.
