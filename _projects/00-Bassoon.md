---
title: "Bassoon"
excerpt: "Compiler for a simple typed procedural language, generating LLVM IR, or executables for (hopefully) any major platform."
collection: Projects
permalink: /projects/Bassoon/
order: 0

mandel_gallery:
  - url: mandel.png
    image_path: mandel.png
    alt: "Mandelbrot Set"
    title: "Mandelrbot Set"
---

Let's summarise the goals, achievements, next steps. Have some nice example programs and outputs. Also talk about design points and things to do next time round.

## Introduction

My plan for Bassoon was to design my own simple language and implement a compiler for it using LLVM. In preparation I had done some smaller projects with C++ and followed the [*Kaleidoscope*](https://llvm.org/docs/tutorial/MyFirstLanguageFrontend/index.html) tutorial to learn the basics of LLVM. My intention was to keep the scope of the language small, but have additional features that the *Kaleidoscope* tutorial did not cover so that I would have to solve some problems and come into contact with some new parts of the LLVM library.

## Goals

The main area I wanted to explore further was types, as the *Kaleidoscope* language had just one type.

### Aims
* `bool`, `int`, `double` types
* static compile time type checking
* `if`, `for`, `while` control flow constructs
* mutable variables
* function definitions
* recursive functions

Some extension aims that I would like to pursue in this or my next language are exceptions and arrays.

## So Far

All of the main aims have been achieved and Bassoon programs can be compiled and executed. Currently the only inputs are C-style arguments when calling the executable, and the only output is printing a single character at a time to `stdout`. This is sufficient for proof of concept programs, and can be easily expanded with further input and output options.

A really helpful thing about the LLVM library is that it makes it very easy to allow standard functions like `putchar()` to be used by the compiler.


## Example Programs

### Mandelbrot Set

Simply rendered with no optimisations. Character lookup is implemented as a sequence of `if` statements due to lack of any dictionary/array structures. 

{% include gallery id="mandel_gallery" caption="Mandelbrot Set, 2022 (Bassoon)" %}


## Next Steps

Definitely need some more tests

Try some arrays

Try some exceptions

Or move onto a new language

## Lessons Learnt

I learned and practiced a lot of aspects of maintaining larger C++ projects and CMake usage.