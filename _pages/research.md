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
  <summary> <b>mixed finite element methods</b></summary><br />
  Most real-world problems involve more than one field. For example, Navier-Stokes equations involve velocity and pressure, and magnetohydrodynamics describes the coupling of fluids and magnetic fields. Finite element methods involving more than one field are referred to as <b>mixed methods</b>. 
A major message from the study of mixed methods (see [1] for a comprehensive account of this subject) is that different fields should be discretized differently to get correct solutions and efficient solvers.  The   <b><a href="https://en.wikipedia.org/wiki/Ladyzhenskaya–Babuška–Brezzi_condition">Ladyzhenskaya–Babuška–Brezzi (LBB) condition</a></b>, or the <b>inf-sup condition</b> provides a criterion for the choices of discretization (discrete spaces) for different fields. Roughly speaking, these conditions describe how (linear) differential operators should map one space to another. For example, for incompressible flows, one discretizes the velocity in one finite dimensional space (e.g., a certain finite element space) and the pressure in another. The inf-sup condition requires that divergence is surjective from the velocity space to the pressure space (with an analytic bound). Homological algebra and differential complexes (central subjects in FEEC) encode kernels and images of (linear) differential operators, and, therefore are proper tools. 

<br /><br />

References:
<ol>
  <li>Daniele Boffi, Franco Brezzi, and Michel Fortin. Mixed finite element methods and applications. Vol. 44. Heidelberg: Springer, 2013.</li>
</ol> 

</details>
 
<br />


<details>
  <summary> <b>structure-preserving and compatible discretization</b></summary><br />
  The idea of <b>structure-preserving discretization</b> or <b>compatible discretization</b> is to recognize key (algebraic, geometric, topological and physical) structures of problems (structure-awareness) and preserve them in the design of numerical methods. An eminent example is <b><a href="https://www.damtp.cam.ac.uk/user/na/NA_papers/NA2015_05.pdf">geometric numerical integration</a></b>, which discretizes classical mechanics in the Hamiltonian form and preserves symplectic forms in algorithms. <br />  <br />
  
   Finite element exterior calculus falls in the category of structure-preserving discretization by capturing cohomologies. This ensures correct numerical solutions, efficient solvers, and precise physical invariants. More precisely, cohomologies of discrete spaces should be compatible with the continuous version. In other words, differential structures are preserved. 
</details>


<br />


<details>
  <summary> <b>discrete topology and geometry</b></summary><br />
<b>Homology</b> is a tool for studying the topology of a domain. Roughly speaking, the idea is to look for loops which are not the boundary of any 2D cell, and higher dimensional versions of such objects (for example, on a 2D domain with a hole, one can draw a loop around the hole, which is not the boundary of any 2D patch). <b>Cohomology</b> comes from duality: one associates a number to each cell (lines, faces etc.) and defines the dual of the boundary operator (called coboundary). Functions with vanishing coboundaries which are not coboundary of another function represent cohomology.  <b>De Rham complex</b> provides a computable version of cohomology: integrating k-forms on k-dimensional cells provides such a function, and coboundary operators correspond to exterior derivatives (grad, curl, div and higher dimensional generalizations).

<br /><br />

The de Rham complex is related to PDEs. For example, the Maxwell equation can be formulated using differential forms and de Rham complexes. In finite element exterior calculus, one wants to discretize the de Rham complex, and use the resulting discrete version to compute. Around the 1970s-1980s, Raviart, Thomas, and Nédélec invented several vector-valued finite elements independently. Soon, Bossavit realized that those finite elements have a unified differential form interpretation and correspond to Whitney's definition in his Geometric Integration Theory, referred to as <b>Whitney forms</b>.  

<figure>
  <img src="../assets/img/deRham-3D.pdf" alt="Whitney forms in 3D" style="width:80%">
  <figcaption>Fig: Whitney forms in 3D.</figcaption>
</figure>

The Whitney forms form a discrete version of de Rham complexes. The algebraic structures are crucial for PDE solvers. The degrees of freedom for k-forms are located at k-dimensional cells (vertices, edges etc.), and therefore Whitney forms enjoy an elegant correspondence to <b>discrete topology</b>. The sequence of Whitney forms has correct cohomologies [2] (isomorphic to the continuous version).

  This differential form perspective was further pursued and led to Hiptmair's <b>canonical construction of finite elements</b> [3] based on Poincaré operators. FEEC develops further in this direction, leading to a <b><a href="https://www-users.cse.umn.edu/~arnold/femtable/">finite element periodic table</a></b>.
  <br /><br />
  
<b>Discrete differential geometry</b> enters the picture when Christiansen interpreted <b><a href="https://en.wikipedia.org/wiki/Regge_calculus">Regge calculus</a></b> (originally a coordinate-free scheme in quantum and computational relativity) as a finite element [4]. The <b>Regge element</b> fits in a discrete version of the elasticity complex (see BGG machinery below), which is often referred to as the elasticity complex, or <b>Calabi complex</b> in differential geometry:
<figure>
  <img src="../assets/img/regge.pdf" alt="Whitney forms in 3D" style="width:80%">
  <figcaption>Fig: Elasticity complex and Regge element.</figcaption>
</figure>

The Regge complex generalizes the concept of finite elements by allowing distributions (currents). Its connections to discrete differential geometry are under active development by several groups.   

Another discrete version of the elasticity with a differential geometry and discrete mechanics perspective is the diamond element [5]. Together with Regge calculus/element, this further demonstrates an interaction between <b>discretizations</b> and <b>discrete theories</b>. 

<br /><br />

References:
<ol>
  <li>Alain Bossavit. "Whitney forms: A class of finite elements for three-dimensional computations in electromagnetism." IEE Proceedings A (Physical Science, Measurement and Instrumentation, Management and Education, Reviews) 135.8 (1988): 493-500.</li>
  <li>  Snorre H. Christiansen. "Finite element systems of differential forms." arXiv preprint arXiv:1006.4779 (2010). </li>
  <li> Ralf Hiptmair. "Canonical construction of finite elements." Mathematics of computation 68.228 (1999): 1325-1346. </li>
<li>Snorre H. Christiansen. "On the linearization of Regge calculus." Numerische Mathematik 119 (2011): 613-640. </li>
<li>P., E. Hauret, Kuhl, and M. Ortiz. "Diamond elements: a finite element/discrete‐mechanics approximation scheme with guaranteed optimal convergence in incompressible elasticity." International Journal for Numerical Methods in Engineering 72.3 (2007): 253-294. </li>
</ol> 

 
</details>
<br /> 
 
I have been working on the following topics:

   
<details>
  <summary> <b>the Bernstein-Gelfand-Gelfand (BGG) machinery</b></summary><br />
  </details>
  <br />
  
<details>
  <summary> <b>finite elements, complexes and splines on triangulation</b></summary><br />
  </details>
  <br />
  
  <details>
  <summary> <b>multiphysics problems, magnetohydrodynamics</b></summary><br />
  </details>

<br />

  <details>
  <summary> <b>miscellany</b></summary><br />
  </details>

<br />
   
   
   

