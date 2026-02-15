---
layout: page
permalink: /personal/
title: Miscellany
nav: true
nav_order: 10
---



- [Some Books](#some-books)
- [Cascading Principles](#cascading-principles)


### Some Books

Here are some books that are special to me — those that have shaped my taste or inspired research questions and ideas.

I am always drawn to new questions, but dynamics, geometry, mechanics and physics, and the interplay between continuous and discrete remain consistently at the heart of my mathematical interests.  

<style>
  .book-row {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 18px;
    margin: 30px 0;
  }

  .book-row img {
    height: 250px;
    width: auto;
    display: block;
  }
</style>

<div class="book-row">
  <img src="../assets/img/ArnoldKhesin.jpg" alt="Topological Methods in Hydrodynamics">
  <img src="../assets/img/book-arnold.png" alt="Mathematical Methods of Classical Mechanics">
  <img src="../assets/img/book-ciarlet.jpg" alt="Linear and Nonlinear Functional Analysis">
    <img src="../assets/img/book-feec.jpg" alt="Finite Element Exterior Calculus">
</div>

<div class="book-row">
  <img src="../assets/img/book-geometry.jpg" alt="Modern Geometry">
  <img src="../assets/img/book-elasticity.jpg" alt="Mathematical Foundations of Elasticity">
  <img src="../assets/img/book-sedov.jpg" alt="Mechanics of Continuous Media">
</div>


<!-- 你稍后提供具体内容，例如书单、推荐理由等，可以放在这里。
例如：

Here are some books that have deeply influenced my thinking in numerical analysis, geometry, and the continuous-discrete interplay:

- **Title** by Author — brief reason why it matters to me.
- ...

-->

### Cascading Principles

> “If an atom or electron is a basic unit for physicists, his unit is the tetrahedron.”  
> — [Cascading Principles exhibition page](https://www.maths.ox.ac.uk/node/61184)

I was fascinated by the exhibition ''Cascading Principles'' at the Andrew Wiles Building in Oxford by the artist Conrad Shawcross. The spirit, as I see it, explains a lot of my passion for the part of mathematics I do.

Finite element methods use tetrahedra (and other shapes) to approximate continua and solve equations on them. Tetrahedra, or more generally, simplices, are the source of many magics. The Whitney forms extend discrete topology encoded in simplices (chains) to everywhere defined fields; the Regge finite element extends discrete metric (edge lengths) and discrete curvature (angle deficit) to piecewise flat metric and curvature measures. This process of "filling in" is what makes finite elements rigorous, compared to more intuitive lattice-based methods. The key lies in the concept of unisolvency: degrees of freedom (discrete physical, topological, or geometric quantities) uniquely determine local shape functions (modes for approximating continuous fields). The unisolvency of Whitney forms and Regge elements, to me, demonstrates elegance and magic (and they are included in standard finite element packages and are useful as well).

The interplay between the continuous and the discrete is central to mathematics. Newton and Leibniz invented (discovered) calculus, introducing the notions of infinitesimals and limits (though the rigorous definitions we use today came later). In the computer age, discrete mathematics and physics have gained more attention, partly due to developments in quantum theory. In numerical PDEs, discretization is a key concept: we discretize the governing equations of physical processes while attempting to preserve their continuous structure. Meanwhile, another tradition focuses on establishing discrete models and theories as first principles in the discrete world. And once again, the building blocks are often tetrahedra.

As a numerical analyst, I feel lucky and passionate to work at this interface of continuous and discrete. To me, this work reflects a similar passion that I see from the artist's perspective.
 
 
<style>
  .row {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    margin: 20px 0;
  }

  .column {
    flex: 1 1 200px;
    padding: 5px;
    text-align: center;
  }

  .column img {
    max-height: 200px;   /* 控制图片大小 */
    width: auto;
    display: block;
    margin: 0 auto;
  }

  figure {
    margin: 0;
  }
</style>

<div class="row">
  <div class="column">
    <figure>
      <img src="../assets/img/exhi2.png" alt="Cascading Principles 1">
    </figure>
  </div>
  <div class="column">
    <img src="../assets/img/exhi3.png" alt="Cascading Principles 2">
  </div>
  <div class="column">
    <img src="../assets/img/exhi4.png" alt="Cascading Principles 3">
  </div>
</div>

<div class="row">
  <div class="column">
    <img src="../assets/img/exhi5.png" alt="Cascading Principles 4">
  </div>
  <div class="column">
    <img src="../assets/img/exhi6.png" alt="Cascading Principles 5">
  </div>
  <div class="column">
    <img src="../assets/img/exhi7.png" alt="Cascading Principles 6">
  </div>
</div>

Another reason I feel a special fondness for the Andrew Wiles Building, apart from its Escher-inspired staircase, is the presence of the "crystals." From these, one can glimpse the lively teaching and conference areas downstairs. The crystals in the south wing depict a surface plot of the first eigenfunction of the two-dimensional Laplacian (probably a finite element solution). I took a picture of these crystals on a quiet night during the pandemic and often use it to visualize Regge elements (piecewise-flat manifolds) in my presentations.

<style>
  .awb-image {
    max-width: 450px;
    max-height: 350px;
    width: auto;
    height: auto;
    display: block;
    margin: 0 auto;
  }
  figure {
    text-align: center;
    margin: 24px 0;
  }
  figcaption {
    font-size: 0.9em;
    color: #555;
    margin-top: 6px;
  }
</style>

<figure>
  <img src="../assets/img/andrewwiles.png"
       alt="South wing crystals at Andrew Wiles Building"
       class="awb-image">
</figure>

<figure>
  <img src="../assets/img/stair.png"
       alt="Escher-inspired staircase at Andrew Wiles Building"
       class="awb-image">
</figure>

**Reference**  
[Andrew Wiles Building leaflet](https://www.maths.ox.ac.uk/system/files/attachments/OxfordMathematics_ROQ_leaflet.pdf)  
[Exhibition main page](https://www.maths.ox.ac.uk/node/61184)

<!-- 未来可以继续加其他 section -->