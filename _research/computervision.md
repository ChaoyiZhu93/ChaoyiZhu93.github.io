---
title: "Computer Vision Approach to Experimental Mechanics"
excerpt: "In experimental mechanics, understanding how materials deform and where they are most susceptible to failure is crucial for promoting safety and potentially guiding material design to alleviate catastrophic loss. Characterization methods at different length scales that can map strain in situ and probe residual deformation post-mortem are therefore very important to provide researchers with location-specific measurable quantities to study failure mechanisms. <br/><img src='/images/DIC Image Registration figures.png'>"
permalink: /research/computer-vision
date: 2019-11-01
collection: research
---

<div style="text-align: justify"> In experimental mechanics, understanding how materials deform and where they are most susceptible to failure is crucial for promoting safety and potentially guiding material design to alleviate catastrophic loss. Characterization methods at different length scales that can map strain in situ and probe residual deformation post-mortem are therefore very important to provide researchers with location-specific measurable quantities to study failure mechanisms. </div>
<br />

<div style="text-align: justify"> One of the most commonly used in situ strain mapping techniques within the mechanics community is the digital image correlation (DIC) technique. It tracks the displacement field of the artificially painted speckle patterns over a deforming surface and computes the corresponding time resolved Green-Lagrange or Eulerian-Almansi strain maps. The sub-pixel level spatial resolution of this technique is provided by the cross-correlation of pairs of images (deformed and undeformed) with subsequent up-sampling of the peak of cross-correlation function through high-order interpolation method. </div>
<br />

<div style="text-align: justify"> In the computer vision community, feature-based image registration, such as the Lucas–Kanade optical flow algorithm, has been widely used since 1981. Many other applications have emerged over the years from the image registration community to deal with tracking, face coding, medical image registration, parametric and layered motion estimation , mosaic construction, etc. One of these many applications involves the study of the deformation of objects by applying the demons algorithm on the objects’ natural patterns. The original demons algorithm was first developed by Thirion as an analogy of Maxwell’s demon, hence the name ***demons algorithm***. The demons algorithm has since been widely implemented in many radiotherapy applications, for example, to track the growth of a tumor. </div>
<br />

<div style="text-align: justify"> Therefore, it is clear that the state-of-the-art methodology for extracting feature variation in images is divided into two communities: the mechanics community and the computer vision community. Although these two communities share almost the same motivations, there has rarely been any dialogue between the two. The mechanics community seeks highly robust and accurate methodologies to map strains of artificial patterns painted on the objects of interest for deformation studies, whereas the computer vision community endeavors to implement a fast and simple feature- or intensity-based algorithm on an objects’ natural surface pattern or texture. </div>
<br />

<div style="text-align: justify"> We have demonstrated in our studies that computer vision could also be used to extract strain information with high accuracy, opening new collaborative opportunities between the two communities. </div>
<br />

<img src='/images/DIC Image Registration figures.png' class="center"> 
<br />

A computer vision approach to study surface deformation of materials
====
<img src='/images/computer-vision-diagram.png' class="center"> 
<br />

<div style="text-align: justify"> Characterization of the deformation of materials across different length scales has continuously attracted enormous attention from the mechanics and materials communities. In this study, the possibility of utilizing a computer vision algorithm to extract deformation information from materials has been explored, which greatly expands the use of computer vision approaches to studying the mechanics of materials and potentially opens new dialogues between the two communities. The computer vision algorithm is first developed and tested on computationally deformed images (% error < 0.035%, L2-norm < 2.5), before evaluating experimentally collected images on speckle painted samples before and after deformation. Moreover, a virtual experiment shows the feasibility of mapping the surface strain of a sample based on its natural pattern with significantly improved accuracy compared to the digital image correlation result obtained from the open-source software Ncorr, which provides new opportunities in experimentation and computer algorithms for studying the deformation mechanics of materials. Validation experiments include evaluating the performance of strain mapping using the computer vision approach in the uniaxial tensile test and three-point bending test, compared with extensometer reading and digital image correlation, respectively. </div>
<br />

Reference: ***Zhu, C.***, Wang, H., Kaufmann, K. and Vecchio, K., 2019. Computer Vision Approach to Study Deformation of Materials. Measurement Science and Technology. 2020

<br />
<br />
<br />

Novel remapping approach for HR-EBSD based on demons registration
====
<img src='/images/HR-EBSD registration.png' class="center"> 
<br />
<div style="text-align: justify"> In this study, the possibility of utilizing a computer vision algorithm, i.e., demons registration, to accurately remap electron backscatter diffraction patterns for high resolution electron backscatter diffraction (HR-EBSD) applications is presented. First, the angular resolution of demons registration is demonstrated to be lower than the conventional cross-correlation based method, particularly at misorientation angles > 0.157 rad. In addition, GPU acceleration has been applied to significantly boost the speed of iterative registration between a pair of patterns with 0.175 rad misorientation to under 1 s. Second, demons registration is implemented as a first-pass remapping, followed by a second pass cross-correlation method, which results in angular resolution of ~0.5×10−4 rad, a phantom stress value of ~35 MPa and phantom strain of ~2×10−4, on dynamically simulated patterns, without the need of implementing robust fitting or iterative remapping. Lastly, the new remapping method is applied to a large experimental dataset collected from an as-built additively-manufactured Inconel 625 cube, which shows significant residual stresses built-up near the large columnar grain region and regularly arranged GND structures. </div>
<br />

Reference: ***Zhu, C.***, Kaufmann, K. and Vecchio, K., 2019. Novel Remapping Approach for HR-EBSD based on Demons Registration. Ultramicroscopy. 2020