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
        .lecture-title {
            font-weight: bold;
            font-size: 1.1em;
        }
    </style>
</head>
<body>
    <p>
        The ERC Starting Project <i>GeoFEM (Geometric Finite Element Methods)</i> explores the discretization of geometric objects using finite element methods, connections between finite elements and discrete differential geometry, and their applications.
    </p>
    <p>
        GeoFEM hosts lectures and short courses delivered by visitors, collaborators, and occasionally group members. These sessions focus on emerging topics and recent advances in finite element methods (broadly defined) and Finite Element Exterior Calculus, particularly those lacking comprehensive documentation, to contribute to broader research contexts and support local researchers. Some lectures offer online participation. To attend remotely, please contact <a href="mailto:kaibo.hu@ed.ac.uk">kaibo.hu@ed.ac.uk</a>.
    </p>
    <br>
    <h3>Lectures and Short Courses</h3>
    <ul>
        <li>
            <span class="lecture-title">Riemannian Geometry with Finite Elements</span><br>
            <a href="https://webpages.scu.edu/ftp/egawlik/">Evan Gawlik</a> (Santa Clara University), October 11–17, 2025<br>
            <strong>Location:</strong> Andrew Wiles Building, Oxford<br>
            <strong>Abstract:</strong> TBA
        </li>
        <li>
            <span class="lecture-title">Finite Element Systems</span><br>
            <a href="https://www.mn.uio.no/math/english/people/aca/snorrec/">Snorre Christiansen</a> (University of Oslo), October 6–14, 2025<br>
            <strong>Location:</strong> Andrew Wiles Building, Oxford<br>
            <strong>Abstract:</strong> TBA
        </li>
        <li>
            <span class="lecture-title">Title TBA</span><br>
            <a href="https://alisomia.github.io">Ting Lin</a> (Peking University), October 2025<br>
            <strong>Location:</strong> Andrew Wiles Building, Oxford<br>
            <strong>Abstract:</strong> TBA
        </li>
        <li>
            <span class="lecture-title">A Posteriori Error Estimation by Preconditioning</span><br>
            <a href="https://sites.google.com/view/liyuwen/">Yuwen Li</a> (Zhejiang University), August 4–8, 2025<br>
            <strong>Location:</strong> James Clerk Maxwell Building (JCMB), Edinburgh<br>
            <strong>Abstract:</strong> <span class="toggle-abstract" onclick="toggleAbstract('abstract0')">Show Abstract</span>
            <div id="abstract0" class="abstract">
                This short course explores preconditioning and a posteriori error estimation in finite element methods, focusing on H(curl) and H(div) spaces. We begin by reviewing fundamental concepts in a posteriori error estimates for adaptive methods and iterative solvers for linear algebraic systems. The course emphasizes the interplay between iterative solvers and a posteriori error estimates, demonstrating the derivation of novel parameter-robust and p-robust error estimators in H(curl) and H(div) using nodal auxiliary space preconditioning at the continuous level. For comparison, we also examine classical a posteriori error analysis in H(grad), H(curl), and H(div).
            </div>
        </li>
        <li>
            <span class="lecture-title">Spectral Theory and Spectral Practice</span><br>
            <a href="https://www.uzerbinati.eu">Umberto Zerbinati</a> (University of Oxford), May 13–16, 2025<br>
            <strong>Course Website:</strong> <a href="https://www.uzerbinati.eu/teaching/spectral_theory/">https://www.uzerbinati.eu/teaching/spectral_theory/</a><br>
            <strong>Location:</strong> James Clerk Maxwell Building (JCMB) 5328 (May 13–14), JCMB 5326 (May 16), Edinburgh<br>
            <strong>Time:</strong> May 13, 2025, 10:00–12:00; May 14, 2025, 14:00–16:00; May 16, 2025, 15:00–17:00<br>
            <span class="toggle-abstract" onclick="toggleAbstract('abstract1')">Show Abstract</span>
            <div id="abstract1" class="abstract">
                This short course explores finite element discretizations of eigenvalue problems involving non-normal operators, with a focus on the advection-diffusion equation as a guiding example. We begin by revisiting fundamental spectral notions—self-adjointness, normality, spectra, and pseudospectra—with particular emphasis on how an operator’s spectrum informs the physical behavior of time-dependent PDEs. The core of the course is devoted to the classical analysis of finite element approximations: we present the Bramble-Osborn results for non-self-adjoint eigenvalue problems, including full proofs, and discuss their implications for convergence and approximation quality. For comparison, we also review the celebrated Babuška-Osborn theory for self-adjoint cases. If time permits, we will conclude with a discussion on iterative solvers and preconditioning strategies tailored to non-normal eigenvalue problems. The course requires a basic background in functional analysis and finite element methods.
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