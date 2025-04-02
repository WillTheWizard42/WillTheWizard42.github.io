---
project_id: Mandelbrot
---

#### Context

The Mandelbrot set is one of the most famous fractal structures, and its definition is quite simple. For these reasons, I've always wanted to make my own Mandelbrot set visualizer.

Even though Unreal Engine is not the best tool to make this kind of project, I chose it because Unreal Engine is very popular and I wanted to learn how it works. <br/>
Since I already knew how to code in C++, I decided to only use Unreal Engine's blueprint system, and a little bit of HLSL.

![Mandelbrot full set](/assets/pictures/mandelbrot-full.png)

The features included are zooming, panning, and changing colors to one of the four options (blue, green, fire red, purple red).

![Mandelbrot set detail](/assets/pictures/Mandelbrot-detail.png)

The visualizer uses a slightly optimized escape time algorithm with 2048 iterations. Colors are decided based on the speed of divergence, that is, the number of iterations it takes for the sequence defining the set to diverge.
This is good enough to be able to zoom into the border of the set and see some of the interesting structures, such as the one above.

![Imprecisions after zooming far into the set](/assets/pictures/Mandelbrot-imprecision.png)

Once the zoom level gets too high, imprecisions start to appear. This is because the difference in position on the plane is so small that neighboring pixels can have their positions represented by the same floating point number (Unreal Engine uses double precision floationg point numbers, but even that has a limit). The above image shows what happens when we reach such a level of zoom.

You can check out the source "code" below, I am not including a build because Unreal Engine no longer builds to WebGL and requires third parties to do so. Additionally, the Windows build I made was 500 MB which is too much for a standard GitHub project. 

#### Links

- [Source code](https://github.com/WillTheWizard42/Mandelbrot)
- [Unreal Engine](https://www.unrealengine.com/en-US)
- [Mandelbrot Set](https://en.wikipedia.org/wiki/Mandelbrot_set)
- [Plotting algorithms for the Mandelbrot set](https://en.wikipedia.org/wiki/Plotting_algorithms_for_the_Mandelbrot_set)