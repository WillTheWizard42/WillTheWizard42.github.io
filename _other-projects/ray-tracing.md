---
project_id: Ray-tracing
---
	
#### Context

This was a project I made with a classmate in my last year of engineering school. The goal was to learn about shaders, ray-tracing and OpenGL.

Every frame, a random position within each pixel is chosen to cast a ray towards. The color obtained is averaged out over several frames, and after a few frames, the picture stabilizes.

The renderer can display a few different 3D models and ground textures. These ground textures sometimes have normal maps, which give a realistic 3D look as shown below.

![Teapot on ground](/assets/pictures/Teapot.png)

It can also display transparent objects, with a modifiable index of refraction to mimmic different types of transparent materials. Below is a transparent render of the armadillo model.

![Armadillo transparent](/assets/pictures/Armadillo-transparent.png)

One other feature the renderer has is to procedurally generate a marble like texture for the 3D object in the scene. The colors and periods (which control the surface area of each color) are modifiable with widgets in the user interface. Below is an example of such a texture on the dragon model.

![Dragon procedural](/assets/pictures/Dragon.png)

The renderer has a few additional parameters (phong exponent, light intensity ...) to play with.

The user interface and OpenGL wrapper were made with C++ and Qt and the ray tracing and color calculations were made with GLSL shaders.

#### Links

- [Source code](https://github.com/WillTheWizard42/raytracing)
- [Qt](https://www.qt.io/)