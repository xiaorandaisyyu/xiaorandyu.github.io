---
title: "C Compiler"
excerpt: "A C90 to RISC-V assembly compiler, written in C++. <br/><img src='/images/500x300.png'>"
collection: projects
---
[GitHub Repo](http://xiaorandyu.github.io/)  [TA's feedback](http://xiaorandyu.github.io/files/EEEBalanceBug.pdf)

## Overview
I built a C90 to RISC-V assembly compiler with my partner as part of my second year Compiler (Language Processing) coursework. The compiler was written in C++, and we used Flex for lexing and Bison for parsing. This coursework was completed in groups of two, and we received high marks for our compiler’s completeness (74.75% passed of all tests, 3rd highest of the year). This is the project that I enjoyed working on the most this year.

## Project Outline

The compiler reads C source code from a file, and writes RISC-V assembly to another file. 

We successfully implemented almost 30 features, from basics (variables; arithmetic and logical expressions) to intermediates (loop-related, inc. if-else, while, for, break, continue, goto, switch; arrays; enum; function call; recurssion) and finally to advanced ones (types; structs; pointer; scoped variables; typedef; strings). 

## Personal Contribution

In the coursework, I mainly contributed in building up the AST and modifying the parser correponding to C90 grammer. My partner and I splitted the features and were each responsible for a portion. I had fun and learned a lot during both the exploration of compiler-related concepts (e.g. LR parsing, symbol table, register allocation C being not context-free, etc.) and the implementation of object-oriented programming (e.g. inheritence).