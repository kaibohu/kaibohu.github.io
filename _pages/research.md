---
layout: page
permalink: /research/
title: Research
description: 
nav: true
nav_order: 2
---

<strong>The page is still under construction.</strong>


I am a numerical analyst by training. I view numerical analysis as a <b>connection</b> between <b>continuous</b> and <b>discrete</b> (which are always central topics in mathematics), and pure and applied. Therefore I am keen to develop these connections: on the one hand, interactions between numerical analysis and 'pure mathematics' (homological algebra, differential and algebraic geometry etc.) and, on the other hand, computational approaches for scientific problems. 

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
  <img src="../assets/img/deRham-3D.png" alt="Whitney forms in 3D" style="width:80%" class="center">
  <figcaption>Fig: Whitney forms in 3D.</figcaption>
</figure>

The Whitney forms form a discrete version of de Rham complexes. The algebraic structures are crucial for PDE solvers. The degrees of freedom for k-forms are located at k-dimensional cells (vertices, edges etc.), and therefore Whitney forms enjoy an elegant correspondence to <b>discrete topology</b>. The sequence of Whitney forms has correct cohomologies [2] (isomorphic to the continuous version).

  This differential form perspective was further pursued and led to Hiptmair's <b>canonical construction of finite elements</b> [3] based on Poincaré operators. FEEC develops further in this direction, leading to a <b><a href="https://www-users.cse.umn.edu/~arnold/femtable/">finite element periodic table</a></b>.
  <br /><br />
  
<b>Discrete differential geometry</b> enters the picture when Christiansen interpreted <b><a href="https://en.wikipedia.org/wiki/Regge_calculus">Regge calculus</a></b> (originally a coordinate-free scheme in quantum and computational relativity) as a finite element [4]. The <b>Regge element</b> fits in a discrete version of the elasticity complex (see BGG machinery below), which is often referred to as the elasticity complex, or <b>Calabi complex</b> in differential geometry:
<figure>
  <img src="../assets/img/regge.png" alt="Regge complex" style="width:80%" class="center">
  <figcaption>Fig: Elasticity complex and Regge element.</figcaption>
</figure>

The Regge complex generalizes the concept of finite elements by allowing distributions (currents). Its connections to discrete differential geometry are under active development by several groups.   

Another discrete version of elasticity with a differential geometry and discrete mechanics perspective is the diamond element [5]. Together with Regge calculus/element, this further demonstrates an interaction between <b>discretizations</b> and <b>discrete theories</b>. 

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
 
I have been working on the following topics in relevant directions:

   
<details>
  <summary> <b>the Bernstein-Gelfand-Gelfand (BGG) machinery</b></summary><br />

  De Rham complexes encode crucial structures of some problems, e.g., those from electromagnetism. There are further examples from continuum mechanics, geometry and general relativity, where <b>tensors</b> with certain structures are the main variables. To tackle these problems in a structured way, one needs to discover and preserve differential and algebraic structures. The <b>Bernstein-Gelfand-Gelfand (BGG) construction</b> provides a tool for this purpose. 
  <br />  <br />
  
<b>History: pure and applied.  </b> BGG originated in representation theory and was later generalized to curved spaces by Čap, Slovák and Souček [1], encoding invariant operators in parabolic geometries (special cases of <b>Cartan geometry</b>).

 In numerical analysis, the first introduction of the idea of BGG started in around 2000 when Arnold, Falk and Winther worked on finite elements for linear elasticity in the mixed form (<b>Hellinger-Reissner principle</b>). The importance of complexes was gradually recognized at that time. In this concrete example of linear elasticity, one needs to characterize the kernel and image of divergence on symmetric tensor fields (stress). The symmetry makes the question rather different from the divergence in the de Rham complex, bringing in essential difficulties. To tackle this problem, Arnold, Falk and Winther started interactions with Eastwood and introduced ideas of BGG. Results from that time can be found in, e.g., [2,3]. Much progress on finite elements for linear elasticity has been achieved later, and some of them were based on BGG. The tools set up by Arnold, Falk and Winther also played a role in the Einstein equations [4]. 
 
  <br /><br /> 
<b>Connections.  </b> BGG is a systematic way of deriving differential complexes with operators such as hessian and linearized curvature (Riemann, Ricci, Cotton-York etc.) from simpler versions (mostly de Rham complexes; this explains the title of [5], ''complexes from complexes'').  The information encoded in BGG is much beyond linear elasticity even in the Euclidean case. In this direction, we carried out a systematic study of BGG [5,6]. On the one hand, these works simplified the geometric and algebraic context, leading to an <b>explicit form</b> of BGG complexes. On the other hand, <b>analysis</b> was incorporated in BGG.  In fact, this differential complex perspective reveals <b>connections</b> between various topics:
<ul>
<li> <b>algebra + topology</b>: Cohomologies of the derived complexes are isomorphic to de Rham cohomology, and therefore correspond to homologies of domains. </li>
<li> <b>analysis</b>: Information of cohomology implies that each derived complex corresponds to a version of Poincaré-Korn inequality, Hodge (Helmholtz), regular decompositions, and compactness.</li>
<li> <b>geometry</b>: Special cases of the BGG sequences correspond to the deformation of (Riemannian, conformal etc.) geometries. </li> 
<li> <b>mechanics and relativity</b>: The twisted de Rham complex is an intermediate step in the derivation of BGG complexes from de Rham complexes. There is an elegant and surprising correspondence between Hodge-Laplacian of these sequences and mechanics models [6]. In 1D, 2D, and 3D, respectively,
<ul>
<li> <b>twisted complexes:  Timoshenko beam, Reissner-Mindlin pate, Cosserat elasticity </b>  </li>
<li> <b>BGG complexes: Euler-Bernoulli beam, Kirchhoff-Love plate, linear elasticity </b>  </li>
</ul>
The models represented by the twisted complexes can be viewed as the BGG versions with additional <b>microscopic (rotational, micropolar) degrees of freedom</b> (giving a hint of the <b>Erlangen program</b> in a mechanics context?). The physical meaning of the BGG process is therefore a <b>cohomology-preserving model reduction</b> by eliminating microscopic variables.  Correspondingly, simplified models encoded in BGG sequences can be lifted to more complete models represented by twisted complexes. Such lifting also exists in the context of (Riemann, Cartan) geometries.

   <br /> 
   The elasticity complex (an example of BGG complexes) also bears the name of the <b>Kröner complex</b> in mechanics (and the <b>Calabi complex</b> in differential geometry). Kröner's work essentially modelled <b>continuum incompatibility</b> (<b>defects</b> caused by dislocations and disclinations etc.) with operators in complexes. Therefore, the BGG picture incorporates and generalizes Kröner's idea in several directions. For example, ''incompatibility operators'' in the twisted complex will correspond to defects in Cosserat continua (Timoshenko beam, Reissner-Mindlin pate).
   
 Further echoing the geometric mechanics perspective [7], we observe that the twisted complex has a close connection to Cartan's torsion and Riemann-Cartan geometry.  
    <br /> 
    
 Kröner [9] already pointed out relationships between generalized continuum theory and <b>general relativity</b> (GR) in an outlook.  This again brings GR into the picture.
 
 </li>
<li> <b>numerics</b>:  For the purpose of finite element exterior calculus, it is necessary to discretize the BGG complexes (also the twisted complexes, or the entire diagram, for generalized continua). In recent years, there has been significant interest in finite element versions of the BGG complexes.   While it is impossible to keep an up-to-date list for this fast-growing area, some results (up to 2022) can be found in the references in [8]. See <b><a href="https://lyc102.github.io/camtips/">here</a></b> for a series of blogs/notes that Long Chen and Xuehai Huang are writing, reflecting their work on finite element construction. See also  ''finite elements, splines on triangulation, and complexes'' below.
    </li>
</ul>

  <br /> 
<b>The machinery.  </b>
BGG is more than complexes. BGG provides explicit connections (cohomology-preserving projections) between de Rham complexes (electromagnetism) and the derived complexes (continuum mechanics, geometry etc.). Therefore, to answer a question from, say, linear elasticity, one may start with the analogous question for de Rham, and then run the machinery to get answers for elasticity. An example of using this machinery can be found in [9,10], where explicit (bounded) Poincaré operators are derived. In a special case, this rather algebraic construction recovers the path integral formulas by Cesàro and Volterra in 1906 and 1907 (sometimes referred to as <b>Cesàro-Volterra</b> path integral). 

  <br /> <br />
<b>Nonlinear versions.  </b>
So far all the complexes contain linear operators. This is natural from a differential geometric and algebraic point of view, as cohomology is defined. A lot of practical problems are nonlinear. FEEC still plays an important role in these problems, as once one linearizes the problems (Piccard or Newton iterations), one obtains linear problems. Moreover, the properties of many hyperbolic PDEs rely on the principal part, which is linear. Nevertheless, we want to ask the question of whether delicate and specific nonlinear structures can be incorporated in FEEC to improve and speed up numerical solutions. In some cases, the differential complexes come from the linearization of certain sequences with nonlinear operators. These sequences are still complexes, although cohomology is not defined.  We refer to such sequences as ''<b>nonlinear complexes</b>'' and observe that on the continuous level, the exactness of such complexes corresponds to important mathematical results. For example, for the elasticity complex, the <b>exactness of the nonlinear version</b> at indices 0 and 1 corresponds to the <b>rigidity theorem</b> and a '<b>fundamental theorem of Riemannian geometry</b>' (à la Ciarlet [12]). Further questions remain open, e.g., connections to the computation for nonlinear elasticity and discrete versions. See [13] for details. 
 
 <br /><br />
 References:
<ol>
<li>Andreas Čap, Jan Slovák, and Vladimír Souček. "Bernstein-Gelfand-Gelfand sequences." Annals of Mathematics (2001): 97-113.</li>
   <li>Douglas N. Arnold, Richard S. Falk, and Ragnar Winther. "Differential complexes and stability of finite element methods II: The elasticity complex." Compatible spatial discretizations. Springer New York, 2006.</li>
    <li>  Michael Eastwood. "A complex from linear elasticity." Proceedings of the 19th Winter School" Geometry and Physics". Circolo Matematico di Palermo, 2000.</li>
    <li> Vincent Quenneville-Belair. "A new approach to finite element simulations of general relativity." PhD thesis at the University of Minnesota, 2015. </li>
    <li>Douglas N. Arnold, and Kaibo Hu. "Complexes from complexes." Foundations of Computational Mathematics 21.6 (2021): 1739-1774. </li>
  <li>  Andreas Čap, and Kaibo Hu. "BGG sequences with weak regularity and applications." Foundations of Computational Mathematics, 2023.  </li>
  <li> Arash Yavari and Alain Goriely. "Riemann–Cartan geometry of nonlinear dislocation mechanics." Archive for Rational Mechanics and Analysis 205 (2012): 59-118.</li>
    <li> Kaibo Hu. "Oberwolfach report: Discretization of Hilbert complexes." arXiv preprint arXiv:2208.03420 (2022).</li>
    <li> Ekkehart Kröner. "General continuum theory of dislocations and proper stresses." Arch. Rat. Mech. Anal 4 (1960): 273-334.</li>
    <li>Snorre H. Christiansen, Kaibo Hu, and Espen Sande. "Poincaré path integrals for elasticity." Journal de Mathématiques Pures et Appliquées 135 (2020): 83-102. </li>
        <li>Andreas Čap, and Kaibo Hu. "Bounded Poincaré operators for twisted and BGG complexes."  Journal de Mathématiques Pures et Appliquées (2023). </li>
        <li>Philippe G. Ciarlet. Linear and nonlinear functional analysis with applications. Vol. 130. Siam, 2013.</li>
    <li>     Kaibo Hu. "Nonlinear elasticity complex and a finite element diagram chase." arXiv preprint arXiv:2302.02442 (2023).</li>
</ol> 
 
 
      </details>
 

  <br />
  
<details>
  <summary> <b>finite elements, splines on triangulation, and complexes</b></summary><br /> 
  
There are motivations for <b> discrete de Rham sequences with higher regularity</b>. For example, for (Navier-)Stokes equations, the inf-sup condition requires that divergence of the velocity space  \(\nabla\cdot V_{h}  \) is ''larger than'' the pressure space \(Q_{h} \), while precise mass conservation requires \(\nabla\cdot V_{h} \subset Q_{h} \). Thus a balance leads to the condition \(\nabla\cdot V_{h}= Q_{h} \). This means that \(V_{h} \) and \(Q_{h} \) should fit in a de Rham complex. However, conforming discretization requires \(V_{h}\subset H^{1} \). Therefore the complex has higher continuity than the H(curl)/H(div) version, and is sometimes referred to as <b> Stokes complexes </b>.

<br />

The first construction of finite element Stokes pairs from this perspective was by Falk and Neilan [1].  There were significant follow-ups, generalizaitons, and variants of this work, including, 3D conforming simplicial finite element Stokes complex   [2] and de Rham complexes with arbitrarily higher regularity [3].

<br />

 

 
 <br /><br />
 References:
<ol>
<li> Richard S. Falk, and Michael Neilan. "Stokes complexes and the construction of stable finite elements with pointwise mass conservation." SIAM Journal on Numerical Analysis 51, no. 2 (2013): 1308-1326.</li>
<li>Michael Neilan. "Discrete and conforming smooth de Rham complexes in three dimensions." Mathematics of Computation 84, no. 295 (2015): 2059-2081.</li>
<li>Long Chen, and Xuehai Huang. "Finite element de Rham and Stokes complexes in three dimensions." Mathematics of Computation 93, no. 345 (2024): 55-110.</li>
</ol> 
  
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
   
   
   

