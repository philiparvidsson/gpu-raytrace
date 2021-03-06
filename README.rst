Raytracing in real-time on the GPU
##################################
Real-time raytracer implemented in HLSL. The raytracer runs on the GPU, not the CPU. This allows for parallelization pf pixel calculations on the GPU's shader units, resulting in thousand-fold speedup for the raytracing process, compared to `software rendering <https://github.com/philiparvidsson/raytracing>`_.

Features
========
* Adaptive antialiasing (not working too well)
* Keyboard controls
* Parallelization through use of shader units on GPU
* Specular materials (Phong illumination)
* Refractions (Snell's law)
* Reflections
* Soft shadows/shadow ray sampling (Monte Carlo integration)

Building and Running
====================
1. Clone this repository.
2. Chdir into the project root.
3. Type :code:`python make.py init`
4. Type :code:`python make.py scene0` to run the first scene, or :code:`python make.py scene1` to run the second scene.

**NOTE**: *Scenes can take a long time to load!*

Video
=====
.. image:: https://img.youtube.com/vi/6DbfnCAce4Y/0.jpg
   :target: https://youtu.be/6DbfnCAce4Y
