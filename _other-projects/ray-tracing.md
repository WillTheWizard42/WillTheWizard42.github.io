---
project_id: Ray-tracing
---
	
#### Context

This was a project I made with a classmate in my last year of engineering school. The goal was to learn about shaders, ray-tracing and openGL.

Each call of the main function will simulate one ray of light, with a random direction. Each ray helps calculate an average color value for the pixel it ends up landing on, and after a few frames, the picture stabilizes. 

The project contains many models and textures to try out, with quite a few parameters (transparence, phong exponent, light intensity ...) to play with. 

The user interface was made with Qt and the ray tracing and color calculations were made with GLSL shaders.

![Armadillo](/assets/pictures/Armadillo-preview.png)

#### Links

<!-- - [Source code](https://gitlab.com/adamsw/blobwar) -->
- [Qt](https://www.qt.io/)