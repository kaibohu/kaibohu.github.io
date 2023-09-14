---
layout: page
permalink: /research/
title: Research
description: 
nav: true
nav_order: 2
---

<strong>The page is still under construction.</strong>


I am a numerical analyst by training. I view numerical analysis as a <b>connection</b> between <b>continuous</b> and <b>discrete</b> (which are always central topics in mathematics), and <b>pure</b> and <b>applied</b>. Therefore I am keen to develop these connections: on the one hand, interactions between numerical analysis and 'pure mathematics' (homological algebra, differential and algebraic geometry etc.) and on the other hand, computational approaches for scientific problems. 

Currently, most of my work is related to <b>finite element exterior calculus (FEEC)</b>. FEEC has its roots in the following contexts:

<details>
  <summary> <b>mixed finite element methods</b></summary>
  Most real-world problems involve more than one field. For example, Navier-Stokes equations involve velocity and pressure, and magnetohydrodynamics describes the coupling of fluids and magnetic fields. Finite element methods involving more than one field are referred to as <b>mixed methods</b>. 
A major message from the study of mixed methods (see [1] for a comprehensive account of this subject) is that different fields should be discretized differently to get correct solutions and efficient solvers.  The   <b><a href="https://en.wikipedia.org/wiki/Ladyzhenskaya–Babuška–Brezzi_condition">Ladyzhenskaya–Babuška–Brezzi (LBB) condition</a></b>, or the <b>inf-sup condition</b> provides a criterion for the choices of discretization (discrete spaces) for different fields. Roughly speaking, these conditions describe how (linear) differential operators should map one space to another. For example, for incompressible flows, one discretizes the velocity in one finite dimensional space (e.g., a certain finite element space) and the pressure in another. The inf-sup condition requires that divergence is surjective from the velocity space to the pressure space (with an analytic bound). Homological algebra and differential complexes (central subjects in FEEC) encode kernels and images of (linear) differential operators, and, therefore are proper tools. 
</details>
 
<br />


<details>
  <summary> <b>structure-preserving and compatible discretization</b></summary>
  The idea of <b>structure-preserving discretization</b> or <b>compatible discretization</b> is to recognize key (algebraic, geometric, topological and physical) structures of problems (structure-awareness) and preserve them in the design of numerical methods. An eminent example is <b><a href="https://www.damtp.cam.ac.uk/user/na/NA_papers/NA2015_05.pdf">geometric numerical integration</a></b>, which discretizes classical mechanics in the Hamiltonian form and preserves symplectic forms in algorithms. <br />  <br />
  
   Finite element exterior calculus falls in the category of structure-preserving discretization by capturing cohomologies. This ensures correct numerical solutions, efficient solvers, and precise physical invariants. More precisely, cohomologies of discrete spaces should be compatible with the continuous version. In other words, differential structures are preserved. 
</details>


<br />


<details>
  <summary> <b>discrete topology and geometry</b></summary>
<b>Homology</b> is a tool for studying the topology of a domain. Roughly speaking, the idea is to look for loops which are not the boundary of any 2D cell, and higher dimensional versions of such objects (for example, on a 2D domain with a hole, one can draw a loop around the hole, which is not the boundary of any 2D patch). <b>Cohomology</b> comes from duality: one associates a number to each cell (lines, faces etc.) and defines the dual of the boundary operator (called coboundary). Functions with vanishing coboundaries which are not coboundary of another function represent cohomology.  <b>De Rham complex</b> provides a computable version of cohomology: integrating k-forms on k-dimensional cells provides such a function, and coboundary operators correspond to exterior derivatives (grad, curl, div and higher dimensional generalizations).

<br />

The de Rham complex is related to PDEs. For example, the Maxwell equation involve grad, curl, and div, and can be written in terms of de Rham complexes. In finite element exterior calculus, one wants to discretize the de Rham complex, and use the resulting discrete version to compute. 

 
</details>

 

   

   

