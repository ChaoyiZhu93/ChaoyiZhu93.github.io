---
title: "Materials Characterization Using Physics Based Forward Model"
excerpt: "Most characterization methods are ill-posed inverse problems which could benefit from some form of regularization. Physics based forward model serves as a strong form of regularization which allows us to accurately model the source (electron, x-ray, photons, neutrons, etc), source-sample interaction, detector behavior, and even take into account potential sources of measurement noise. It is then possible to iteratively infer material properties through direct comparison of the modeling results with experimental data by solving the inverse problem <br/><img src='/images/forward-model.png'>"
permalink: /research/forward-model
date: 2020-11-01
collection: research
---

<div style="text-align: justify"> Most characterization methods are ill-posed inverse problems which could benefit from some form of regularization. Physics based forward model serves as a strong form of regularization which allows us to accurately model the source (electron, x-ray, photons, neutrons, etc.), source-sample interaction, detector behavior, and even take into account potential sources of measurement noise. It is then possible to iteratively infer material properties through direct comparison of the modeling results with experimental data by solving the inverse problem. </div>
<br />

<div style="text-align: justify"> Within the framework of a forward model, the instrument produces a generalized forward projection of a specific property of interest from the material. The specific signal associated with that forward projection is then collected by a specific type of detector. Then, mathematical model can then be employed to extract useful features in order to estimate the property of interest. </div>
<br />

<div style="text-align: justify"> In a standard university laboratory, many different kinds of diffractometers and spectrometers are available to characterize structure and chemical properties of materials. Scanning electron microscopy is one of the most widely available and capable techniques for materials scientists because of the following reasons: (1) large sampling area to conduct statistically relevant analysis, (2) high spatial resolution over a wide range of magnifications, (3) equipped with multiple detectors to collect multiple signals coming out of the electron-matter interaction (X-ray, secondary electrons, backscattered , Auger electrons, etc.), (4) easy to operate with fully automated system and analytical software. </div>
<br />

<div style="text-align: justify"> In recent years, electron backscatter diffraction (EBSD) has emerged as a popular measurement technique in SEM to uncover mostly structure related properties of crystalline materials such as spatially resolved crystallographic orientation, texture, dislocations structures, grain boundaries, pseudosymmetry, phase mapping, and etc. This increasing popularity stemmed from the implementation of fully automated Hough indexing in the 90s, which has allowed enormous amount of information to be extracted at an extraordinary speed ~4k fps. Despite numerous studies that focus on extracting deformation information, there has been no systematic study to quantify the effect of deformation of EBSD patterns and currently no way of determining the absolute deformation tensor. In order to provide solutions to these problems through forward modeling, computationally efficient method is required to include deformation tensor to the simulation of deformed EBSD patterns. Moreover, simultaneous inclusion of the pattern center is critical to reduce error induced by pattern center uncertainty. </div>
<br />

EBSD Pattern Simulations for an Interaction Volume Containing Lattice Defects
======
<figure>
    <img src='/images/ebsd-ivol-01.png' class="center"> 
    <figcaption> The effect of deformation and interaction volume of electron interaction on the diffraction field surrounding single edge dislocation and low angle grain boundary.</figcaption>
</figure>

<br />

<div style="text-align: justify"> Despite the existence of numerous experimental studies on lattice defects with EBSD, there exists a lack of systematic understanding of the effects of defects on diffraction patterns. Early studies have shown that backscattered electrons are randomly generated inside the interaction volume, as prescribed by the Rutherford differential scattering cross-section. To accurately account for the effect of spatial distribution and density of defects on the diffraction pattern, interaction volume effect and depth-dependent local distortion of the crystal must be simultaneously considered. In this study, the integration of the approximate model for deformation inclusion in a master pattern with the depth-specific dynamical master pattern simulation allows us to produce a single weighted diffraction pattern summing up all the deformed depth master patterns contained within an interaction volume. Using this new method of pattern simulation, we have examined two cases: 1) a single edge dislocation; 2) a low angle grain boundary. </div>
<br />

Reference: ***Zhu, C***. and De Graef, M., 2020. EBSD Pattern Simulations for an Interaction Volume Containing Lattice Defects. Ultramicroscopy, p.113088
<br />
<br />
<br />

Deformation state extraction from electron backscatter diffraction patterns via simulation-based pattern-matching
====
<figure>
    <img src='/images/deformation-inference.png' class="center"> 
    <figcaption> Pattern matching based deformation tensor inference around a single dislocation (compared with HR-EBSD).</figcaption>
</figure>

<div style="text-align: justify"> Global optimization algorithms have been adopted to refine orientation and pattern center for electron backscatter diffraction patterns as well as deformation state extraction. Validation on a realistically simulated undeformed single crystal nickel sample reveals mean accuracy of ~0.03 degrees and ~0.01% detector width across a large field of view. In combination with high angular resolution-EBSD, this method enables determination of strain states of reference patterns, hence, mapping of absolute strain maps becomes possible. Validation using noisy simulated deformed patterns with known deformation state and pattern center shows that the mean accuracy of shear strain and rotation components ~0.001 and normal strain ~0.002. Combined with an additional optimization step for the pattern center and orientation, an experimentally collected fatigue cycled TRIP steel data set has been able to validate the consistency of strain maps with the use of different reference patterns. </div>

Reference: Kurniawan, C., ***Zhu, C.*** and DeGraef, M., Deformation state extraction from electron backscatter diffraction patterns via simulation-based pattern-matching. Scripta Materialia, 190, pp.147-152.