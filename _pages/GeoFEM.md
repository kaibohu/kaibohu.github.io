---
layout: page
permalink: /geofem/
title: GeoFEM
nav: true
nav_order: 8
---

 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GeoFEM Homepage</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 20px;
        }
        .abstract {
            display: none;
            margin-top: 10px;
            padding: 10px;
            background-color: #f9f9f9;
            border-left: 3px solid #007bff;
        }
        .toggle-abstract {
            color: #007bff;
            cursor: pointer;
            text-decoration: underline;
        }
        .toggle-abstract:hover {
            color: #0056b3;
        }
    </style>
</head>
<body>
    <p>
        The ERC Starting Grant <i>GeoFEM (Geometric Finite Element Methods)</i> investigates discretization of geometric objects with finite elements, connections between finite elements and discrete differential geometry, and applications.
    </p>
    <p>
        GeoFEM will host lectures and short courses given by visitors and collaborators.
    </p>
    <br>
    <h3>Lectures and Short Courses</h3>
    <ul>
        <li>
            <strong>Riemannian geometry with finite elements</strong><br>
            <a href="https://webpages.scu.edu/ftp/egawlik/index.html">Evan Gawlik</a> (Santa Clara University), October 11-17, 2025<br>
            <strong>Location:</strong> Andrew Wiles Building, Oxford<br>
            <strong>Abstract:</strong> TBA<br>
        </li>
        <li>
            <strong>Finite Element Systems</strong><br>
            <a href="https://www.mn.uio.no/math/english/people/aca/snorrec/">Snorre Christiansen</a> (University of Oslo), October 6-14, 2025<br>
            <strong>Location:</strong> Andrew Wiles Building, Oxford<br>
            <strong>Abstract:</strong> TBA<br>
        </li>
        <li>
            <strong>Title TBA</strong><br>
            <a href="https://alisomia.github.io">Ting Lin</a> (Peking University), October 2025<br>
            <strong>Location:</strong> Andrew Wiles Building, Oxford<br>
            <strong>Abstract:</strong> TBA<br>
        </li>
        <li>
            <strong>Spectral Theory and Spectral Practice</strong><br>
            <a href="https://www.uzerbinati.eu">Umberto Zerbinati</a> (University of Oxford), May 2025<br>
            <strong>Course Website:</strong> <a href="https://www.uzerbinati.eu/teaching/spectral_theory/">https://www.uzerbinati.eu/teaching/spectral_theory/</a><br>
            <strong>Location:</strong> James Clerk Maxwell Building (JCMB) 5328 (May 13, 14), JCMB 5326 (May 16)<br>
            <strong>Time:</strong> May 13, 2025, 10:00 AM - 12:00 PM; May 14, 2025, 2:00 PM - 4:00 PM; May 16, 2025, 3:00 PM - 5:00 PM<br>
            <span class="toggle-abstract" onclick="toggleAbstract('abstract1')">Show Abstract</span>
            <div id="abstract1" class="abstract">
                This short course explores finite element discretisations of eigenvalue problems involving non-normal operators, with a focus on the advection-diffusion equation as a guiding example. We begin by revisiting fundamental spectral notions—self-adjointness, normality, spectra, and pseudospectra—with particular emphasis on how an operator spectrum informs us about the physical behaviour of the time-dependent PDEs. The core of the course is devoted to the classical analysis of finite element approximations: we present in detail the Bramble-Osborn results for non-self-adjoint eigenvalue problems, including full proofs, and discuss their implications for convergence and approximation quality. For comparison, we also review the celebrated Babuška-Osborn theory in the self-adjoint case. If time permits, we will conclude with a discussion on iterative solvers and preconditioning strategies tailored to non-normal eigenvalue problems. The course requires basic background in functional analysis and finite element methods.
            </div>
        </li>
    </ul>

    <script>
        function toggleAbstract(id) {
            const abstract = document.getElementById(id);
            const toggleText = abstract.previousElementSibling;
            if (abstract.style.display === 'none' || abstract.style.display === '') {
                abstract.style.display = 'block';
                toggleText.textContent = 'Hide Abstract';
            } else {
                abstract.style.display = 'none';
                toggleText.textContent = 'Show Abstract';
            }
        }
    </script>
</body>
</html>