---
layout: project
title: ANSYS Design Project
description: Advanced CAD Project
skills: [ANSYS, Fusion 360]
image: /assets/images/Materials/MatCADmodel.jpg
---


For this project, I analyzed the structural behavior of an aluminum handle using both hand calculations and finite element modeling. My goal was to understand how well classical beam theory predicts real structural performance when compared to a full three dimensional simulation. I created a solid model of the handle, applied realistic boundary conditions, and evaluated the stress and displacement fields under load. This project helped me connect the idealized methods taught in class to the more detailed results produced by simulation tools such as ANSYS.
<div style="clear: both;"></div>


![Wheel assembly CAD]({{ "/assets/images/Materials/Normalstress.jpg" | relative_url }}){: .inline-image-r style="width: 260px;" }


A key part of the project was comparing maximum normal stress obtained from beam theory with the stress predicted by the finite element model. The hand calculation treated the handle as a simple prismatic beam and produced a maximum bending stress of 12.8 ksi. The finite element model showed a significantly higher peak of about 51.7 ksi. This difference occurred because the simulation captured local stress concentrations caused by the small load contact area and the geometric interface between bodies in the model. Classical beam theory gives a smooth stress distribution along the length of the beam, while the finite element model resolves the detailed three dimensional effects that dominate at the load application point. This comparison demonstrated the importance of combining analytical calculations with simulation when evaluating structural components.
<div style="clear: both;"></div>

![Cleat detail]({{ "/assets/images/Materials/MaterialsDeformation.jpg" | relative_url }}){: .inline-image-l style="width: 260px;" }


I also compared the predicted tip displacement from beam theory with the displacement from the finite element model. The hand calculation estimated a deflection of 0.28 inches using the standard Euler-Bernoulli beam formula. The simulation predicted a larger displacement of about 0.39 inches. The increase in the finite element result comes from geometric features such as fillets and varying thicknesses that are not represented in the hand model. The simulation also includes shear deformation and more realistic constraint behavior. By observing the deformation pattern in the finite element mesh, I confirmed that plane sections remain mostly plane, which supports the assumptions of beam theory for global bending. However, the detailed numerical model still gives a more accurate picture of the actual flexibility of the structure.
<div style="clear: both;"></div>

![Wedge CAD]({{ "/assets/images/Materials/normalelasticstrain.jpg" | relative_url }}){: .inline-image-r style="width: 260px;" }

I evaluated the maximum principal stress in the handle to understand how the material experiences tension in the most critical directions during loading. While the bending stress from beam theory provides a good baseline, the principal stress field from the finite element model reveals the true multi-axial state of stress near geometric transitions. The simulation showed elevated principal stresses around the load application region and at the interface between bodies, where local constraint effects amplify the stress field. These peaks did not appear in the hand calculations because classical beam theory assumes a single bending axis and does not account for three dimensional stress interactions. By examining principal stress contours, I was able to identify where the component is most likely to initiate failure and how the geometry directs the stress flow. This reinforced the value of using principal stress analysis when evaluating real components with complex loading and geometry.

<div style="clear: both;"></div>


![Wedge subassembly]({{ "/assets/images/Materials/Maxprincipalstress.jpg" | relative_url }}){: .inline-image-l style="width: 260px;" }

This project strengthened my understanding of when analytical methods are reliable and when numerical analysis becomes necessary. Beam theory provided a solid first estimate for the overall bending behavior, but the finite element model exposed local stresses and true deformation characteristics that cannot be captured by hand calculations. Working through this comparison helped me develop better intuition for structural mechanics and gave me experience validating analytical results with simulation. This approach is essential when designing real components that must withstand concentrated loads and complex geometry.