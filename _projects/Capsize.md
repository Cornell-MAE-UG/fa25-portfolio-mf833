---
layout: project
title: Capsize
description: Advanced CAD Project
skills: [Autodesk Fusion][testing][materials][FEA]
image: /assets/images/Capsizeforkconfig.jpg
---


Capsize is a 12 lb Sportsman-class combat robot that we made the year I lead the subteam on Combat Robotics @ Cornell. I focused on the drivetrain, traction system, and front armor geometry to keep the bot maneuverable while surviving repeated high-energy impacts. The design went through several CAD and physical iterations before we finalized a competition-ready build. 


![Wheel assembly CAD]({{ "/assets/images/CapsizeWheelAssembly.jpg" | relative_url }}){: .inline-image-r style="width: 260px;" }

I designed the custom wheel assemblies around off-the-shelf motors and sprockets, targeting a balance between top speed and pushing power. The hubs, spacers, and bearing seats were modeled for easy machining and assembly while maintaining alignment under load. Chain routing and tension were verified in CAD and then adjusted after real-world testing.



![Cleat detail]({{ "/assets/images/CapsizeCleats.jpg" | relative_url }}){: .inline-image-l style="width: 260px;" }

To maximize traction on the NHRL floor, I developed a cleated tread system. The cleats were positioned to increase the effective contact area without making the bot sluggish or overly aggressive on turning. I iterated on cleat spacing and height to avoid wheel slip while keeping manufacturing simple and repeatable for spares.




![Wedge CAD]({{ "/assets/images/Capsizewedge.jpg" | relative_url }}){: .inline-image-r style="width: 260px;" }

The front wedge is the primary contact surface during a match. I tuned the approach angle and ground clearance so Capsize can get underneath opponents while staying robust against direct hits. Mounting locations were chosen to spread impact loads into the main chassis rails and keep the wedge easy to replace between fights.



![Wedge subassembly]({{ "/assets/images/Capsizewedgeassembly.jpg" | relative_url }}){: .inline-image-l style="width: 260px;" }

The wedge assembly ties into side armor and top plates with a mix of slotted and fixed holes. This let us adjust alignment after assembly and quickly swap between practice and competition wedges using the same mounting pattern.




![Sprocket testing]({{ "/assets/images/Capsizesprockettesting .jpg" | relative_url }}){: .inline-image-r style="width: 260px;" }

Before committing to the final layout, I ran sprocket and chain tests to check alignment, tension, and backlash under load. These tests helped confirm that the drivetrain could handle rapid direction changes without derailing the chain or overloading the motors.


![Fork configuration]({{ "/assets/images/Capsizeforkconfig.jpg" | relative_url }}){: .inline-image-l style="width: 260px;" }

I also explored a fork configuration as an alternate front attachment. The goal was to give the driver more control in lifting and destabilizing opponents while keeping the same chassis and drivetrain. This modular approach allowed us to experiment with different matchups without redesigning the entire robot.



![Bare chassis]({{ "/assets/images/Capsizewheelbare.jpg" | relative_url }}){: .inline-image-r style="width: 260px;" }

This is what the wheel looks like underneath the uretheane. The reason for the geometry is so that the uretheane could grip onto the wheel as best as it could. If it had a weak geometry with not enough contact points with the uretheane, the casting would grip onto the floor weakly or even slide off after high energy impacts.


![Drive testing circle]({{ "/assets/images/CapsizeNarayanCircle.jpg" | relative_url }}){: .inline-image-l style="width: 260px;" }

We used this circle to test the tension between the pulley and the wheel. This is crucial because if the pulley is too loose we risk it falling off and not driving our wheel. The opposite happens when it is too tight, the pulley runs risk of snapping. 


<div style="text-align: center;">
  <img src="{{ '/assets/images/Capsizecomp.jpg' | relative_url }}" style="width: 260px;">
</div>

This is capsize at competition!
