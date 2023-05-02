---
title: "Fractals"
excerpt: "Lightning fast recap of my fractal explorations"
collection: Projects
permalink: /projects/Fractals/
order: 1

header_gallery:
  - url: budha.png
    image_path: budha.png
    alt: "Buddhabrot"
    title: "Buddhabrot"

gallery1:
  - url: csharp_mandel.jpg
    image_path: csharp_mandel.jpg
    alt: "C# Mandelbrot"
    title: "C# Mandelbrot"
  - url: java_mandel.png
    image_path: java_mandel.png
    alt: "Java Mandelbrot"
    title: "Java Mandelbrot"

gallery2:
  - url: dragon-curve.gif
    image_path: dragon-curve.gif
    alt: "Dragon Curve L-System"
    title: "Dragon Curve"
  - url: sier-arrow.gif
    image_path: sier-arrow.gif
    alt: "Sierpinski Arrowhead L-system"
    title: "Sierpinski Arrowhead"
  - url: koch.gif
    image_path: koch.gif
    alt: "Koch Snowflake"
    title: "Koch Snowflake"
  - url: tree.gif
    image_path: tree.gif
    alt: "L-system binary tree"
    title: "L-system binary tree"
  - url: menger.gif
    image_path: menger.gif
    alt: "Menger Sponge"
    title: "Menger Sponge"
  - url: menger-inverted.gif
    image_path: menger-inverted.gif
    alt: "Inverted Menger Sponge"
    title: "Inverted Menger Sponge"
  # - url: poster.png
  #   image_path: poster.png
  #   alt: ""
  #   title: ""
  # - url: spike-lsystem.png
  #   image_path: spike-lsystem.png
  #   alt: ""
  #   title: ""

coursework_gallery:
  - url: FracTool.png
    image_path: FracTool.png
    alt: "FracTool Example"
    title: "Mandelbrot Set and Julia"
  - url: FracTool2.png
    image_path: FracTool2.png
    alt: "FracTool Example 2"
    title: "Burning Ship Julia"

mandel_gallery:
  - url: fractalBlueSim.png
    image_path: fractalBlueSim.png
    alt: "Mandelbrot Set Detail"
    title: "Mandelbrot Set Detail"
  - url: fractalItSim.png
    image_path: fractalItSim.png
    alt: "Mandelbrot set with too few iterations"
    title: "Too few iterations"
  - url: fractalRedSim.png
    image_path: fractalRedSim.png
    alt: "Mandelbrot set detail red"
    title: "Mandelbrot set detail"
  - url: fractalSpeedSim.png
    image_path: fractalSpeedSim.png
    alt: "Mandelbrot set high contrast"
    title: "Mandelbrot set fast palette"
  - url: julia1.png
    image_path: julia1.png
    alt: "Julia Set"
    title: "Julia Set"
  - url: julia2.png
    image_path: julia2.png
    alt: "Rainbow Julia Set"
    title: "Rainbow Julia Set"
  - url: julia3.png
    image_path: julia3.png
    alt: "Julia Set for point outside of mandelbrot"
    title: "Julia Set dust"

burning_ship_gallery:
  - url: BSWhole.png
    image_path: BSWhole.png
    alt: "Burning Ship Fractal"
    title: "Burning Ship Fractal"
  - url: BSShips.png
    image_path: BSShips.png
    alt: "Burning Ship Detail"
    title: "Burning Ship Detail"
  - url: BSRepeat.png
    image_path: BSRepeat.png
    alt: "Burning Ship Detail 2"
    title: "Burning Ship Detail 2"
  - url: fractalBarcode.png
    image_path: fractalBarcode.png
    alt: "Burning Ship Detail Barcode"
    title: "Burning Ship Detail Barcode"
  - url: BSColumn.png
    image_path: BSColumn.png
    alt: "Burning Ship Detail Pillar"
    title: "Burning Ship Detail Pillar"
  - url: Looks3d.png
    image_path: Looks3d.png
    alt: "Burning Ship Detail 3"
    title: "Burning Ship Detail 3"
  - url: BJulia1.png
    image_path: BJulia1.png
    alt: "Burning Ship Julia 1"
    title: "Burning Ship Julia 1"
  - url: BJulia3.png
    image_path: BJulia3.png
    alt: "Burning Ship Julia 2"
    title: "Burning Ship Julia 2"
  - url: BJulia4.png
    image_path: BJulia4.png
    alt: "Burning Ship Julia 3"
    title: "Burning Ship Julia 3"

sactal_gallery:
  - url: sactalM.png
    image_path: sactalM.png
    alt: "Mandelbrot Set"
    title: "Mandelbrot Set"
  - url: sactalB.png
    image_path: sactalB.png
    alt: "Burning Ship Fractal"
    title: "Burning Ship Fractal"
  - url: sactalMB.png
    image_path: sactalMB.png
    alt: "Multibrot d=2"
    title: "Multibrot d=2"
  - url: sactalBMB.png
    image_path: sactalBMB.png
    alt: "Burning Multibrot d=2"
    title: "Burning Multibrot d=2"
  - url: sactalMH2.png
    image_path: sactalMH2.png
    alt: "Multibrot d=2.5"
    title: "Multibrot d=2.5"
  - url: sactalMH3.png
    image_path: sactalMH3.png
    alt: "Multibrot d=3.5"
    title: "Multibrot d=3.5"

buddha_gallery:
  - url: buddha.png
    image_path: buddha.png
    alt: "Buddhabrot"
    title: "Buddhabrot"
---

## Introduction

My interest with fractals started in 2017 when I was staying with my grandparents, and found an old book of fractals. Finding Daniel Shiffman's [*Nature of Code*](https://natureofcode.com/) website and [*The Coding Train*](https://www.youtube.com/@TheCodingTrain) YouTube channel soon after prompted me to start writing my own fractal renderers. This post will be a lightning fast review of these renderers and other related experiments.

{% include gallery id="header_gallery" caption="Buddhabrot" %}

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

## Other Escape Time Fractals

There are fractals generated in the same fashion as the Mandelbrot set but with different equations.

| Fractal Name          | Equation        |
| ----------------------| ----------------|
| Mandelbrot Set        |  z = z^2 + c    |
| Burning Ship Fractal  |  z = abs(z)^2+c |
| Multibrot Set         |  z = z^d + c    |
| "Burning" Multibrot   |  z = abs(z)^d+c |

{% include gallery id="sactal_gallery" caption="Mandelbrot, Burning Ship, Multibrot (d=2), Burning Multibrot (d=2), Multibrot (d=2.5), Multibrot (d=3.5) 2018 (Java, Processing)" %}

## Buddhabrot

A different method of rendering the Mandelbrot set that I want to explore further in the future. In this method, pixels are coloured based on the frequency of that pixel's location being "visited" by the iteration of a random sample of points in the complex plane. Only points that escape to infinity (hence are not in the Mandelbrot set) contribute to the frequency counts.

{% include gallery id="buddha_gallery" caption="Buddhabrot with RGB escape times of 20, 2000, 20000" %}


## Next Projects

I'm keen to explore using shaders to exploit parrallel computation and improve the render speed, and signed distance fields (SDFs) for 3D or higher dimensional fractals in my next project. [Inigo Quilez](https://iquilezles.org/articles/distfunctions/) has some fantastic resources about SDFs and their uses. 