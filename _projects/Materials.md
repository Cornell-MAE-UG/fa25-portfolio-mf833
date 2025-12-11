---
layout: project
title: ANSYS Design Project
description: Advanced CAD Project
skills: [ANSYS, Fusion 360]
image: /assets/images/Materials/MaterialsCAD.jpg
---


For this project, we analyzed the structural behavior of an aluminum handle using both hand calculations and finite element modeling. My goal was to understand how well classical beam theory predicts real structural performance when compared to a full three dimensional simulation. I created a solid model of the handle, applied realistic boundary conditions, and evaluated the stress and displacement fields under load. This project helped me connect the idealized methods taught in class to the more detailed results produced by simulation tools such as ANSYS.
<div style="clear: both;"></div>

![Wheel assembly CAD]({{ "/assets/images/Materials/MaterialsCAD.jpg" | relative_url }}){: .inline-image-r style="width: 500x;" }

For this project we selected Aluminum 7075 T6 because it offers one of the highest strength-to-weight ratios among common aluminum alloys. It is widely used in aerospace and high-performance mechanical systems where low mass and high stiffness are important. The T6 tempering process provides excellent tensile strength and good fatigue resistance, which makes the material suitable for components subjected to repeated loading. In this analysis, 7075 T6 satisfied the project requirements by delivering the necessary stiffness, strength, and durability while keeping the overall weight low. Using this material allowed me to evaluate how a high-strength aluminum alloy responds to both global bending loads and the localized stresses captured in the finite element model. This material has a Young's modulus of 10.4 Mpsi and poisson's ratio of 0.3.

![Wheel assembly CAD]({{ "/assets/images/Materials/Diagram.jpg" | relative_url }}){: .inline-image-l style="width: 500px;" }

To evaluate the structural response of the handle, we applied realistic loads and boundary conditions within the finite element model. One end of the handle was fully constrained with a displacement boundary condition that prevented translation and rotation, representing a fixed support. The opposite end of the handle received a concentrated force of 37.5 lbf applied over the end face, which simulated the loading scenario defined in the project requirements. 

<div style="clear: both;"></div>

![Cleat detail]({{ "/assets/images/Materials/MaterialsDeformation.jpg" | relative_url }}){: .inline-image-l style="width: 500px;" }


We also compared the predicted tip displacement from beam theory with the displacement from the finite element model. The hand calculation estimated a deflection of 0.28 inches using the standard Euler-Bernoulli beam formula. The simulation predicted a larger displacement of about 0.39 inches. The increase in the finite element result comes from geometric features such as fillets and varying thicknesses that are not represented in the hand model. The simulation also includes shear deformation and more realistic constraint behavior. By observing the deformation pattern in the finite element mesh, We confirmed that plane sections remain mostly plane, which supports the assumptions of beam theory for global bending. However, the detailed numerical model still gives a more accurate picture of the actual flexibility of the structure.
<div style="clear: both;"></div>

![Wedge CAD]({{ "/assets/images/Materials/normalelasticstrain.jpg" | relative_url }}){: .inline-image-r style="width: 500px;" }

We evaluated the maximum principal stress in the handle to understand how the material experiences tension in the most critical directions during loading. The simulation showed elevated principal stresses around the load application region and at the interface between bodies, where local constraint effects amplify the stress field. These peaks did not appear in the hand calculations because classical beam theory assumes a single bending axis and does not account for three dimensional stress interactions. By examining principal stress contours, I was able to identify where the component is most likely to initiate failure and how the geometry directs the stress flow. This reinforced the value of using principal stress analysis when evaluating real components with complex loading and geometry.

<div style="clear: both;"></div>


![Wedge subassembly]({{ "/assets/images/Materials/Maxprincipalstress.jpg" | relative_url }}){: .inline-image-l style="width: 500px;" }

From the FEM analysis of our final design, the maximum normal stress anywhere in the model is about 51.7 ksi, the deflection at the load point is approximately 0.39 in, and the strain at the strain-gauge location is 1152.7 microstrain.

From the hand calculations, we obtained a maximum bending stress of 12.8 ksi, a tip deflection of 0.28 in, and a strain at the gauge of about 1153.9 microstrain. Compared to these values, the FEM stress is roughly four times higher, the FEM deflection is about 39 percent higher, and the FEM strain is almost identical (within about 0.1 percent). The large differences in stress and deflection come from the simplifying assumptions in the hand model, which treats the handle as a uniform beam with pure bending and a perfectly rigid support. 

Our torque wrench sensitivity Using the FEM strain at the gauge location, ε≈1152.7 microstrain, and a gauge factor of 2 in a half-bridge configuration, the torque wrench sensitivity is about 1.15 mV/V. This value essentially matches the sensitivity obtained from the hand-calculation strain (also about 1.15 mV/V), confirming that both the analytical model and the FEM predict nearly the same strain in the gauge region and that the design meets the required sensitivity.

![Wedge subassembly]({{ "/assets/images/Materials/sensitivity.jpg" | relative_url }}){: .center-image style="width: 600px;" }

The selected strain gauge is the Vishay Micro-Measurements CEA-06-125UN-350, which is about 0.18 in × 0.28 in, with a 0.125-in grid length and a grid width of about 0.10–0.12 in. This fits perfectly. 

This project strengthened my understanding of when analytical methods are reliable and when numerical analysis becomes necessary. Beam theory provided a solid first estimate for the overall bending behavior, but the finite element model exposed local stresses and true deformation characteristics that cannot be captured by hand calculations. Working through this comparison helped me develop better intuition for structural mechanics and gave me experience validating analytical results with simulation. This approach is essential when designing real components that must withstand concentrated loads and complex geometry.