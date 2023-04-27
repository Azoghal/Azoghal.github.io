---
title: "Fractals"
excerpt: "Lightning fast recap of my fractal explorations"
collection: projects
order: 1

gallery1:
  - url: /images/csharp_mandel.jpg
    image_path: /images/csharp_mandel.jpg
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: /images/java_mandel.png
    image_path: /images/java_mandel.png
    alt: "placeholder image 2"
    title: "Image 2 title caption"
---

## Introduction

My interest with fractals started in 2017 when I was staying at my grandparents', and found an old book of fractals. Finding Daniel Shiffman's [*Nature of Code*](https://natureofcode.com/) website and [*The Coding Train*](https://www.youtube.com/@TheCodingTrain) YouTube channel prompted me to start writing my own fractal renderers. This post will be a lightning fast review of these renderers and other related experiments.

## Early Fractal Renderers

<!-- <div><image src="../images/csharp_mandel.jpg"/><image  src="../images/java_mandel.png"/></div> -->

{% include gallery caption="This is a sample gallery with **Markdown support**." %}

Mandelbrot renderers, 2017 (C#, Java, Processing).
My very first attempt used C# and .NET libraries, and was as clunky as it could possibly have been. I then moved onto the more suitable Processing library for Java that I continued to use for many other projects. The Processing version of the renderer could be navigated naturally using the mouse, and had optimizations like increasing the number of iterations (i.e. accuracy of the fractal's shape) with the level of zoom. 

## Other Fractals

While 

## Better Renderers

## Next Areas

I'm keen to explore using shaders to exploit parrallel computation and improve the render speed, and signed distance fields (SDFs) for 3D or higher dimensional fractals in my next project. [Inigo Quilez](https://iquilezles.org/articles/distfunctions/) has some fantastic resources about SDFs and their uses.