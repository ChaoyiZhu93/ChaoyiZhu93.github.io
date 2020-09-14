---
title: "EBSD pattern simulations for an interaction volume containing lattice defects"
excerpt: "The dynmamical electron scattering model taking into account of interaction volume effect and depth-dependent local distortion of crystal lattice <br/><img src='/images/ebsd-ivol.png'>"
permalink: /research/ebsd-ivol
date: 2020-11-01
---
.. image:: /images/ebsd-ivol.png
   :width: 500

Despite the existence of numerous experimental studies on lattice defects with EBSD, there exists a lack of systematic understanding of the effects of defects on diffraction patterns. Early studies have shown that backscattered electrons are randomly generated inside the interaction volume, as prescribed by the Rutherford differential scattering cross-section. To accurately account for the effect of spatial distribution and density of defects on the diffraction pattern, interaction volume effect and depth-dependent local distortion of the crystal must be simultaneously considered. 

In this study, we have modified our dynamical electron scattering model for EBSD pattern simulation to be depth-specific. The backscattered electron yield P(***k***, z<sub>p</sub>) in this case has been formulated as a function of the backscattered electron wave vector ***k*** and depth z<sub>p</sub>. The intensity of ***k*** can be obtained by summing up the properly weighted intensities of k from these slices of depth-specific master patterns. To account for the deformation of crystal, an approximate model for deformation inclusion has been incorporated. Namely, we apply the inverse of the deformation gradient tensor to the rotated positive vectors of detector pixels and then interpolate on the Lambert projection of the undistorted master pattern. However, the deformation considered in the approximate model assumes uniform deformation whereas the deformation field around dislocations is spatially non-uniform with a strong surface effect. The integration of the approximate model for deformation inclusion in a master pattern with the depth-specific dynamical master pattern simulation allows us to produce a single weighted diffraction pattern summing up all the deformed depth master patterns contained within an interaction volume. 

For validation purpose, we have implemented the Yoffe-Shaibani-Hazzeldine threading dislocation model, using nickel as an example material, to generate three-dimensional deformation tensor field for two case studies: 1) a single edge dislocation (including hydrostatic strain); 2) a low angle grain boundary (pile-up of edge dislocations). The imposed weighted deformation on simulated diffraction patterns is validated with the HR-EBSD method. Lastly, pattern diffuseness evolution as a function of defect density is quantitatively analyzed through inspecting the high-frequency components in the frequency domain.

Reference: ***Zhu, C***. and De Graef, M., 2020. EBSD Pattern Simulations for an Interaction Volume Containing Lattice Defects. Ultramicroscopy, p.113088