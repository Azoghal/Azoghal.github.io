---
title: "Fractals"
excerpt: "Lightning fast recap of my fractal explorations"
collection: projects
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
   - url: BSRepeat.png
    image_path: BSRepeat.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: BSColumn.png
    image_path: BSColumn.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: BJulia1.png
    image_path: BJulia1.png
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: BJulia2.png
    image_path: BJulia2.png
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
I came across [Lindenmayer Systems](https://en.wikipedia.org/wiki/L-system) and generated a number of different fractals using a basic stack based approach. I also tried rendering the Mandelbrot set in a different manner, intending to turn it into a poster of some sort.

I was interested upon revisiting L-Systems to read about their place in the family of formal grammars and variations upon the original formulation. I might explore these further soon.

## Better Renderers

{% include gallery id="burning_ship_gallery" caption="Burning Ship Fractal, Burning Ship Julia Sets" %}

{% include gallery id="coursework_gallery" caption="The FracTool renderer, showing simultaneous views of the Mandelbrot set and a Julia set of a selected point from it." %}

My next fractal project evolved into my project for A-Level Computing coursework. This is the most fully featured renderer I've made so far. It could render the Mandelbrot set and the Burning Ship Fractal, as well as the Julia sets that correspond to each point of those sets. It also had:
* feature 1
* feature 2
* feature 3

## Next Projects

I'm keen to explore using shaders to exploit parrallel computation and improve the render speed, and signed distance fields (SDFs) for 3D or higher dimensional fractals in my next project. [Inigo Quilez](https://iquilezles.org/articles/distfunctions/) has some fantastic resources about SDFs and their uses. 