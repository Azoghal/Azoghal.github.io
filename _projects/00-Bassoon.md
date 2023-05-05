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

[Source Code](http://azoghal.github.io/files/brot.bs).

{% include gallery id="mandel_gallery" caption="Mandelbrot Set, 2022 (Bassoon)" %}

## Next Steps

* More complete test suite
* Add `global` variables
* Add array variables and indexed access
* Add exceptions

## Lessons Learnt

I learnt and practiced a lot of aspects of maintaining larger C++ projects and CMake usage. In the future I want to use CMake and CTest for test suites rather than cobbling together my own solution. On the programming language side, I think that next time round I'll use something like [Bison](https://www.gnu.org/software/bison/) to generate a parser. As long as the grammar of the language is context free, *Bison* can automatically generate a parser for the language, which is helpful as it minimizes the effort required to parse new language features. I do think that it was valuable to implement the parser from scratch for Bassoon. 

While writing the code generator I kept coming back to the question of whether implementing my own typechecker was necessary, as any type errors would be picked up by the LLVM IR builder during codegen, without my manual checking of types in the AST. In the end I'm glad I persisted with my own typechecker, firstly because it was interesting to build, but also because it means that the language's frontend is a properly abstracted from the exact types offered by LLVM for example. The language definition contains typing rules, and these should hold whether using an LLVM compiler or any other. In reality the scope of Bassoon's use means that this issue is redundant.

I used the visitor pattern a lot, for example in the AST visualiser, type checker and code generator. I enjoyed using the pattern and think it was very suitable for these use-cases, but think that my usage of stacks to effectively pass values between different calls to visitors (for example to get the value of a parent in the AST's visior call) feels a little clunky and prone to problems. 