---
layout: without-toc
title: Spreadsheet
---

# Spreadsheet Application Backend

> **Notice to Reader**<br>
> This page is work-in-progress


I'm sure you already know what a spreadsheet is. Tools like Google Sheets and Microsoft
Excel are widely used for organizing and analyzing data in a tabular form. A fundamental
feature of spreadsheet applications is the ability to write expressions in cells. ...

- Order of operations with arithmetic operators (e.g., `=3 + 5 * 2`)
- Expressions with cell references (e.g., `=4 * A2`)
- Aggregate operators with variadic arguments (e.g., `=SUM(A1:D5, C2, 10)`)
- Cascading cell updates (e.g., when `A2` updates, the expression `=A2 * 2` should update)


This spreadsheet app was a solo project as part of an Object-Oriented Analysis and Design
course at WPI. The project idea and starter code was developed by 
[Sakire Arslan Ay](https://www.wpi.edu/people/faculty/sarslanay){:target="_blank"}, the 
professor of the course.


<!---->
<!-- #todo Things to talk about: -->
<!-- - Representation of a spreadsheet expression (`Expression` tree) -->
<!--     - Distinction between terminal and composite nodes -->
<!--     - How I extended the existing interfaces to support new node types -->
<!---->
<!-- - Cell references -->
<!--     - Rewatch demo video and write about the things I talked about there -->
<!---->
<!-- - Cascading cell updates -->
<!--     - Make some diagrams that showcase the  -->
<!---->
<!-- - Parser -->
<!--     - Mention that this was *extra* credit -->
<!--     - Reuse the diagrams I have -->
<!---->
---


## Representation of cell expressions

The first fundamental design decision you have to make with cell expressions is
determining how to represent them in code. 

An expression can take many different forms. For example, `3`, `2 * 8`, and `SUM(A1:D3)`
are all expressions despite looking very different. It is natural to represent expressions
as a tree since some expressions can contain nested expression. For example, the
expression `4 + SUM(A1, 9 / 3, B2:C4)` would have the following representation:

![Expression tree](/assets/images/spreadsheet/Expression-tree.png) 


One operation that is common amongst all expressions is the ability to be evaluated.
Whenever you have shared functionality, you should create an interface. Thus, our
top-level `Expression` interface is born:

<img src="/assets/images/spreadsheet/Expression-interface.png" style="border: none"/>









