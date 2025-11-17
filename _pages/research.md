---
layout: page
permalink: /research/
title: Research
description: 
nav: true
nav_order: 2
---

A significant focus of my current research lies in **structure-preserving and compatible discretization**, with a particular emphasis on **Finite Element Exterior Calculus (FEEC)**. This field, however, extends beyond its name: "finite element" may extend to discrete patterns like finite/lattice differences, currents, or networks, while "exterior calculus" can integrate Cartan’s full formalism (particularly with connections to differential geometry) or, more broadly, tensor analysis.  The Bernstein-Gelfand-Gelfand (BGG) construction and representation theory are languages for expressing tensor symmetries. 

Some specific topics I am interested in now include: 

 - **General theories of FEEC and Finite Element Tensor Calculus**: This includes tensor finite elements (discretizing geometric objects such as metrics, curvature, torsion, connection forms, form-valued forms, double forms, or bundle-valued forms), links to discrete differential geometry, BGG machinery and representation theory. Construction of finite elements and complexes (connections to spline theories), high-order methods and solvers in the finite element context. 

 - **Computational topological hydrodynamics and magnetohydrodynamics (MHD)**: Topology-preserving numerical methods for fluid and plasma systems, relaxation problems (self-organization), dynamo problems and applications in solar physics, astrophysics, and fusion energy. 

	From Kelvin and Helmholtz to Arnold, Khesin, and Moffatt (among others), topology has become central to fluid dynamics. Quantities such as helicity and enstrophy encode knotting, topological constraints, and the fine structure such as turbulence energy cascades in both fluid and MHD systems.

	Despite these elegant theories, practical applications remain limited, largely due to the lack of topology-preserving numerical methods. Recent advances in FEEC sheds new light on the numerical realization of topological hydrodynamics and MHD.

	My PhD research centered on *how to preserve* geometric and physical structures in MHD computation. More recently, I have been drawn to *why such preservation matters*: the mathematical and physical consequences of structure-preservation, and to the limits of structure-preservation (e.g., the failure of energy and helicity conservation in weak solutions, as predicted by the Onsager conjecture). The ultimate goal is reliable computation under weak regularity, over long-time evolution, and on general manifold geometries, topologies, and symmetries.


 - **Algebraic and geometric modeling of generalized continua, discretization and solvers**: This involves micropolar continua, defect theories, and multidimensional models, drawing inspiration from rational mechanics (e.g., the Cosserat brothers’ models, Eringen’s micropolar theory, Kröner and Nye’s defect modeling, and Yavari-Goriely’s geometric dislocation/disclination theory). Hilbert complexes and BGG constructions offer computationally friendly tools with built-in analysis. 

 - **Numerical relativity**: Solving linearized and nonlinear Einstein equations numerically, with applications in astrophysics and gravitational wave sciences.

- **Discrete differential geometry**: Christiansen’s pioneering work of interpreting Regge calculus as a finite element opens a door for designing, analysing, and generalising discrete geometric patterns from the finite element point of view. In addition, I am interested in a PDE analysis perspective, and interactions and applications with computer graphics, discrete physics (Lattice Gauge Theory, quantum and numerical gravity), and materials (origami etc.)

 - **Geometry, topology, PDEs, and physics on graphs**:  The broad idea is to discretize continuous theories on graphs or networks. Finite Element Exterior Calculus (in the narrow sense) is a special case on triangulation. In fact, for differential forms, Finite Element Exterior Calculus and graph (co)homology and Hodge-Laplacian share many common definitions and properties. Other problems include random graphs and phase transition (statistical topology) and topological/geometric data analysis etc. 

Although my perspective on these topics continually evolves, I maintain a consistent interest in investigating continuous and discrete structures,  using them to design reliable, efficient, and high-fidelity numerical methods, and investigating the interactions between numerical analysis (finite elements) and other areas.

[**These slides**](https://kaibohu.github.io/homepage/2025-general-research.pdf) summarized part of my current research interests.
