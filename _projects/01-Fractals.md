---
title: "Fractals"
excerpt: "Lightning fast recap of my fractal explorations"
collection: Projects
permalink: /projects/Fractals/
order: 1

gallery1:
  - url: csharp_mandel.jpg
    image_path: csharp_mandel.jpg
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: java_mandel.png
    image_path: java_mandel.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"

gallery2:
  - url: dragon-curve.gif
    image_path: dragon-curve.gif
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: sier-arrow.gif
    image_path: sier-arrow.gif
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: koch.gif
    image_path: koch.gif
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: tree.gif
    image_path: tree.gif
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: menger.gif
    image_path: menger.gif
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: menger-inverted.gif
    image_path: menger-inverted.gif
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  # - url: poster.png
  #   image_path: poster.png
  #   alt: "placeholder image 2"
  #   title: "Image 2 title caption"
  # - url: spike-lsystem.png
  #   image_path: spike-lsystem.png
  #   alt: "placeholder image 2"
  #   title: "Image 2 title caption"

coursework_gallery:
  - url: FracTool.png
    image_path: FracTool.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: FracTool2.png
    image_path: FracTool2.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"

mandel_gallery:
  - url: fractalBlueSim.png
    image_path: fractalBlueSim.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: fractalItSim.png
    image_path: fractalItSim.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: fractalRedSim.png
    image_path: fractalRedSim.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: fractalSpeedSim.png
    image_path: fractalSpeedSim.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: julia1.png
    image_path: julia1.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: julia2.png
    image_path: julia2.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: julia3.png
    image_path: julia3.png
    alt: "placeholder image 1"
    title: "Image 1 title caption"

burning_ship_gallery:
  - url: BSWhole.png
    image_path: BSWhole.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: BSShips.png
    image_path: BSShips.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: BSRepeat.png
    image_path: BSRepeat.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: fractalBarcode.png
    image_path: fractalBarcode.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: BSColumn.png
    image_path: BSColumn.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: Looks3d.png
    image_path: Looks3d.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: BJulia1.png
    image_path: BJulia1.png
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: BJulia3.png
    image_path: BJulia3.png
    alt: "placeholder image 3"
    title: "Image 2 title caption"
  - url: BJulia4.png
    image_path: BJulia4.png
    alt: "placeholder image 3"
    title: "Image 2 title caption"

sactal_gallery:
  - url: sactalM.png
    image_path: sactalM.png
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: sactalB.png
    image_path: sactalB.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: sactalMB.png
    image_path: sactalMB.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: sactalBMB.png
    image_path: sactalM.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
---

## Introduction

My interest with fractals started in 2017 when I was staying with my grandparents, and found an old book of fractals. Finding Daniel Shiffman's [*Nature of Code*](https://natureofcode.com/) website and [*The Coding Train*](https://www.youtube.com/@TheCodingTrain) YouTube channel soon after prompted me to start writing my own fractal renderers. This post will be a lightning fast review of these renderers and other related experiments.

## Early Fractal Renderers


{% include gallery id="gallery1" caption="Mandelbrot renderers, 2017 (C#, Java, Processing)" %}
My very first attempt used C# and .NET libraries, and was as clunky as it could possibly have been. I then moved onto the more suitable Processing library for Java that I continued to use for many other projects. The Processing version of the renderer could be navigated naturally using the mouse, and had optimizations like increasing the number of iterations (i.e. accuracy of the fractal's shape) with the level of zoom. 

## Other Fractals

{% include gallery id="gallery2" caption="L-Systems, 2017 (Java, Processing)" %}
I came across [Lindenmayer Systems](https://en.wikipedia.org/wiki/L-system) and generated a number of different fractals using a basic stack based approach. I also tried rendering the basic Menger Sponge and Inverted Menger Sponge 3D fractals.

I was interested upon revisiting L-Systems to read about their place in the family of formal grammars and variations upon the original formulation. I might explore these further soon.

## Better Renderers

{% include gallery id="mandel_gallery" caption="Colourful Mandelbrot Sets and Julia Sets, 2018 (Java, Processing)" %}

My next fractal project evolved into my project for A-Level Computing coursework. This is the most fully featured renderer I've made so far. It could render the Mandelbrot set and the Burning Ship Fractal, as well as the Julia sets that correspond to each point of those sets. It also had:
* GUI
* Two Rendering Windows
* 3 Levels of Detail
* Multithreaded Rendering
* Multiple Colour Palettes
* Looping Colour Palettes

{% include gallery id="coursework_gallery" caption="The FracTool renderer, showing simultaneous views of the Mandelbrot set and a Julia set of a selected point from it, 2018 (Java, Processing)" %}

{% include gallery id="burning_ship_gallery" caption="Burning Ship Fractal, Burning Ship Julia Sets, 2018 (Java, Processing)" %}

There are fractals generated in the same fashion as the Mandelbrot set but with different equations.

| Fractal Name          | Equation        |
| ----------------------| ----------------|
| Mandelbrot Set        |  z = z^2 + c    |
| Burning Ship Fractal  |  z = abs(z)^2+c |
| Multibrot Set         |  z = z^d + c    |
| "Burning" Multibrot   |  z = abs(z)^d+c |

<!-- {% include gallery id="sactal_gallery" caption="Mandelbrot, Burning Ship, Multibrot, Burning Multibrot, 2018 (Java, Processing)" %} -->


## Next Projects

I'm keen to explore using shaders to exploit parrallel computation and improve the render speed, and signed distance fields (SDFs) for 3D or higher dimensional fractals in my next project. [Inigo Quilez](https://iquilezles.org/articles/distfunctions/) has some fantastic resources about SDFs and their uses. 