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
        .references {
            margin-top: 12px;
            padding-top: 8px;
            border-top: 1px solid #ddd;
        }
    </style>
</head>
<body>
    <p>
        The ERC Starting Project <i>GeoFEM (Geometric Finite Element Methods)</i> explores the discretization of geometric objects using finite element methods, connections between finite elements and discrete differential geometry, and their applications.
    </p>
    <p>
        GeoFEM hosts lectures and short courses delivered by visitors, collaborators, and occasionally group members. These sessions focus on emerging topics and recent advances in finite element methods (broadly defined) and Finite Element Exterior Calculus, particularly those lacking comprehensive documentation. Some lectures offer online participation. To attend remotely, please <a href="mailto:kaibo.hu@maths.ox.ac.uk">contact</a>.
    </p>
    <br>
    <h3>Lectures and Short Courses</h3>
    <ul>
        <li>
            <span class="lecture-title">Auxiliary Space Theory: Simple Construction of Sophisticated Iterative Methods for Linear Systems</span><br>
            <a href="https://sites.google.com/view/jonghopark">Jongho Park</a>(KAUST)<br>
            <strong>Location:</strong> Andrew Wiles Building, Oxford<br>
            <strong>Time:</strong> To be confirmed (multiple sessions)<br>
            <strong>Abstract:</strong> <span class="toggle-abstract" onclick="toggleAbstract('abstract4')">Show Abstract</span>
            <div id="abstract4" class="abstract">
                We present an auxiliary space theory that provides a unified framework for analyzing various iterative methods for solving linear systems. By interpreting a given iterative method for the original system as an equivalent, yet more elementary, iterative method for an auxiliary system defined on a larger space, we derive sharp convergence estimates using elementary linear algebra. In particular, we establish identities for the error propagation operator and the condition number associated with iterative methods, which generalize and refine existing results. The proposed auxiliary space theory is applicable to the analysis of numerous advanced numerical methods in scientific computing. To demonstrate its utility, we present a variety of applications, including subspace correction methods, Hiptmair–Xu preconditioners, saddle point problems, and iterative substructuring methods, and show how the proposed framework yields refined analyses in each case.
                <div class="references">
                    <strong>References:</strong><br>
                    [1] Jongho Park. Unified analysis of saddle point problems via auxiliary space theory. arXiv preprint 2509.11434 (2025).<br>
                    [2] Jongho Park and Jinchao Xu. Auxiliary space theory for the analysis of iterative methods for semidefinite linear systems. arXiv preprint 2509.07179 (2025).<br>
                    [3] Jinchao Xu and Ludmil Zikatanov. Algebraic multigrid method. Acta Numer., 26 (2017), pp. 591–721. (Section 4 only)
                </div>
            </div>
        </li>

        <li>
            <span class="lecture-title">Riemannian Geometry with Finite Elements</span><br>
            <a href="https://webpages.scu.edu/ftp/egawlik/">Evan Gawlik</a> (Santa Clara University), October 11–17, 2025<br>
            <strong>Location:</strong> VC1, Andrew Wiles Building, Oxford<br>
            <strong>Time:</strong> October 13, 14:00–16:00; October 14, 10:00–12:00; October 15, 13:00–15:00<br>
            <strong>Abstract:</strong> <span class="toggle-abstract" onclick="toggleAbstract('abstract0')">Show Abstract</span>
            <div id="abstract0" class="abstract">
                This short course will cover techniques for discretizing the building blocks of Riemannian geometry---metrics, connections, and curvature---with finite elements. It will start with a brief introduction to the geometry of smooth surfaces and classical notions of discrete curvature on piecewise flat triangulated surfaces. We will explain how to generalize these notions of discrete curvature to triangulated manifolds equipped with piecewise polynomial metrics. Then we will explain how one can prove that these curvature discretizations converge to their smooth counterparts under refinement of the triangulation. Along the way, key concepts from Riemannian geometry will be reviewed, and links between discrete differential geometry and finite element theory will be highlighted and used extensively.
            </div>
        </li>

        <li>
            <span class="lecture-title">Finite elements in categorical language</span><br>
            <a href="https://www.mn.uio.no/math/english/people/aca/snorrec/">Snorre Christiansen</a> (University of Oslo), October 6–14, 2025<br>
            <strong>Location:</strong> VC1, Andrew Wiles Building, Oxford<br>
            <strong>Time:</strong> October 8, 14:00–16:00; October 10, 14:00–16:00; October 13, 11:00–12:00<br>
            <strong>Abstract:</strong> <span class="toggle-abstract" onclick="toggleAbstract('abstract1')">Show Abstract</span>
            <div id="abstract1" class="abstract">
                I will show how finite elements can be described in terms of constructs from category theory. In particular they may be interpreted as presheaves on the poset category of a mesh. I will assume no prior knowledge of categories or sheaves. Ciarlet's definition of a finite element imposes a unisolvency condition which can be related to softness of sheaves. De Rham theorems relating different cohomologies can be proved in the general setting. Examples will be discussed.
            </div>
        </li>

        <li>
            <span class="lecture-title">A Posteriori Error Estimation by Preconditioning</span><br>
            <a href="https://sites.google.com/view/liyuwen/">Yuwen Li</a> (Zhejiang University), August 4–8, 2025<br>
            <strong>Location:</strong> James Clerk Maxwell Building (JCMB), Edinburgh. August 7, 13:30–15:30: JCMB 6206; August 8, 13:30–15:30: JCMB 6201; August 11, 13:30–15:30: JCMB 6206 <br>
            <strong>Videos:</strong>
            <a href="https://drive.google.com/file/d/1YvWklp2JZ-AH7R1QrRuLEcbA0-bGBtbf/view?usp=sharing">Lecture 1</a>,
            <a href="https://drive.google.com/file/d/1JDWYS1lTmzWjF_IvnHgS0fo_Qb2PiIlv/view?usp=sharing">Lecture 2</a>,
            <a href="https://drive.google.com/file/d/1sx2DkO632NvZUIb6UoHH_ILPmy5O-ZfF/view?usp=sharing">Lecture 3</a><br>
            <strong>Lecture Notes:</strong> <a href="https://drive.google.com/file/d/1rlgzKqeud-cRulJgS5VMkIPQqaCfnx2q/view?usp=sharing">Download Notes</a><br>
            <strong>Abstract:</strong> <span class="toggle-abstract" onclick="toggleAbstract('abstract2')">Show Abstract</span>
            <div id="abstract2" class="abstract">
                This short course explores preconditioning and a posteriori error estimation in finite element methods, focusing on H(curl) and H(div) spaces. We begin by reviewing fundamental concepts in a posteriori error estimates for adaptive methods and iterative solvers for linear algebraic systems. The course emphasizes the interplay between iterative solvers and a posteriori error estimates, demonstrating the derivation of novel parameter-robust and p-robust error estimators in H(curl) and H(div) using nodal auxiliary space preconditioning at the continuous level. For comparison, we also examine classical a posteriori error analysis in H(grad), H(curl), and H(div).
            </div>
        </li>

        <li>
            <span class="lecture-title">Spectral Theory and Spectral Practice</span><br>
            <a href="https://www.uzerbinati.eu">Umberto Zerbinati</a> (University of Oxford), May 13–16, 2025<br>
            <strong>Course Website:</strong> <a href="https://www.uzerbinati.eu/teaching/spectral_theory/">https://www.uzerbinati.eu/teaching/spectral_theory/</a><br>
            <strong>Location:</strong> James Clerk Maxwell Building (JCMB) 5328 (May 13–14), JCMB 5326 (May 16), Edinburgh<br>
            <strong>Time:</strong> May 13, 2025, 10:00–12:00; May 14, 2025, 14:00–16:00; May 16, 2025, 15:00–17:00<br>
            <span class="toggle-abstract" onclick="toggleAbstract('abstract3')">Show Abstract</span>
            <div id="abstract3" class="abstract">
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