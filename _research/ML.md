---
title: "High-Throughput Characterization with Machine Learning"
excerpt: "Following some of the most significant discoveries in physics made in the 20th century, modern breakthroughs in physical science have been closely correlated with the exponential growth in the computational power and advanced analytical algorithms. To tackle some of the urgent problems that our humanity faces such as global warming, scientists more actively seek for material solutions to lead a more sustainable future, for example, structural alloys that last longer in service and battery materials with higher energy storage capacity. Part of the so-called 'closed-loop' challenge in designing new materials is to integrate high-throughput characterization into the materials' design process. With ever more sophisticated machine learning algorithms... <br/><img src='/images/ML-importance.png'>"
permalink: /research/ml-characterization
date: 2019-11-01
collection: research
---

<div style="text-align: justify"> Following some of the most significant discoveries in physics made in the 20th century, modern breakthroughs in physical science have been closely correlated with the exponential growth in the computational power and advanced analytical algorithms. To tackle some of the urgent problems that our humanity faces e.g. global warming, scientists more actively seek for material solutions to lead a more sustainable future, for example, structural alloys that last longer in service and battery materials with higher energy storage capacity. Part of the so-called 'closed-loop' challenge in designing new materials is to integrate high-throughput characterization into the materials' design process. With ever more sophisticated machine learning algorithms, this 'closed-loop' approach will create an accelerated environment for computers to quickly filter through enormously large data of potential candidates and ultimately guide the design of new materials to achieve desirable properties. </div>
<br />

<div style="text-align: justify"> For many solid state materials, phase identification and mapping provides necessary structure-chemical information that will affect the thermal, mechanical, electrical properties. Typically, this would involve first identifying the phases present in the XRD and then spatially map these phases in EBSD. In other words, the identity of phases need be known prior to EBSD scan. Alternatively, one can also use the state-of-art combined EBSD/EDS technique to filter through the database based on chemical composition and then use Hough-indexing to determine the best-fit structure. However, this approach is not particularly accurate for diffraction patterns with pseudosymmetry and it requires use-defined reference points for mapping. </div>
<br />

<div style="text-align: justify"> A more direct approach to this phase classification problem is to solely reply on diffraction patterns since the features in diffraction patterns contains both the chemical and structure information i.e. a classical image classification problem for convolutional neural network (CNN). As the CNN continuously learn from a large collection of experimental patterns manually collected from different phases, it adjusts the millions of weights and biases in the network that would allow correct classification of different phases. Unlike feature engineering, the power of CNN lies in its ability in indiscriminately utilize all the available features to make decisions. Although the initial training process would require a large collection of data and computation power, the speed of classification using a deployed model is extremely fast. Future endeavor in this research area will be focusing on using dynamically simulated patterns to complete the database and expand its classification capability. </div>
<br />

<img src='/images/ML-importance.png' class="center"> 
<br />

Crystal symmetry determination in electron diffraction using machine learning
====
<img src='/images/cnn-ebsd.png' class="center"> 
<br />

<div style="text-align: justify"> Electron backscatter diffraction (EBSD) is one of the primary tools for crystal structure determination.
However, this method requires human input to select potential phases for Hough-based or dictionary pattern matching and is not well suited for phase identification. Automated phase identification is the first step in making EBSD into a high-throughput technique. We used a machine learning–based approach and developed a general methodology for rapid and autonomous identification of the crystal symmetry from EBSD patterns. We evaluated our algorithm with diffraction patterns from materials outside the training set. The neural network assigned importance to the same symmetry features that a crystallographer would use for structure identification</div>
<br />

Reference: Kaufmann, K., ***Zhu, C.***, Rosengarten, A.S., Maryanovsky, D., Harrington, T.J., Marin, E. and Vecchio, K.S., Science. 2020

<br />
<br />
<br />

Phase Mapping in EBSD Using Convolutional Neural Networks
====
<img src='/images/ML-phasemaps.png' class="center"> 
<br />
<img src='/images/ML-phasemaps-2.png' class="center"> 
<br />
<div style="text-align: justify"> The emergence of commercial electron backscatter diffraction (EBSD) equipment ushered in an era of information rich maps produced by determining the orientation of user-selected crystal structures. Since then, a technological revolution has occurred in the quality, rate detection, and analysis of these diffractions patterns. The next revolution in EBSD is the ability to directly utilize the information rich diffraction patterns in a high-throughput manner. Aided by machine learning techniques, this new methodology is, as demonstrated herein, capable of accurately separating phases in a material by crystal symmetry, chemistry, and even lattice parameters with fewer human decisions. This work is the first demonstration of such capabilities and addresses many of the major challenges faced in modern EBSD. Diffraction patterns are collected from a variety of samples, and a convolutional neural network, a type of machine learning algorithm, is trained to autonomously recognize the subtle differences in the diffraction patterns and output phase maps of the material. This study offers a path to machine learning coupled phase mapping as databases of EBSD patterns encompass an increasing number of the possible space groups, chemistry changes, and lattice parameter variations </div>
<br />

Reference: Kaufmann, K., ***Zhu, C.***, Rosengarten, A.S., Maryanovsky, D., Wang, H. and Vecchio, K.S., 2020. Phase Mapping in EBSD Using Convolutional Neural Networks. Microscopy and Microanalysis, pp.1-11. 

Deep Neural Network Enabled Space Group Identification in EBSD
=====

<img src='/images/space group-ml.png' class="center"> 
<br />

<div style="text-align: justify"> Electron backscatter diffraction (EBSD) is one of the primary tools in materials development and analysis. The technique can perform simultaneous analyses at multiple length scales, providing local sub-micron information mapped globally to centimeter scale. Recently, a series of technological revolutions simultaneously increased diffraction pattern quality and collection rate. After collection, current EBSD pattern indexing techniques (whether Hough-based or dictionary pattern matching based) are capable of reliably differentiating between a “user selected” set of phases, if those phases contain sufficiently different crystal structures. EBSD is currently less well suited for the problem of phase identification where the phases in the sample are unknown. A pattern analysis technique capable of phase identification, utilizing the information-rich diffraction patterns potentially coupled with other data, such as EDS-derived chemistry, would enable EBSD to become a high-throughput technique replacing many slower (X-ray diffraction) or more expensive (neutron diffraction) methods. We utilize a machine learning technique to develop a general methodology for the space group classification of diffraction patterns; this is demonstrated within the (4/m, 3 bar, 2/m) point group. We evaluate the machine learning algorithm's performance in real-world situations using materials outside the training set, simultaneously elucidating the role of atomic scattering factors, orientation, and pattern quality on classification accuracy. </div>
<br />

Reference: Kaufmann, K., ***Zhu, C.***, Rosengarten, A.S. and Vecchio, K.S., 2020. Deep Neural Network Enabled Space Group Identification in EBSD. Microscopy and Microanalysis, pp.1-11.