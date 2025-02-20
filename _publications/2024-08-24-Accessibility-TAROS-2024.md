---
title: "Accessibility Framework for Determining Collisions and Coverage for Radiation Scanning."
collection: publications
category: conferences
permalink: /publication/2024-08-24-Accessibility-TAROS-2024
excerpt: 'This paper is about determining whether a probe model as a convex hull collides with point clouds enabling the analysis of coverage and accessibility. Future work will use this to form a path planner for complete coverage'
date: 2024-08-24
venue: 'TAROS'
paperurl: 'http://joshua-bettles.github.io/files/TAROS_2024.pdf'
slidesurl: 'http://joshua-bettles.github.io/files/TAROS_Presentation_2024.pdf'
citation: 'J. Bettles, A. West, J. Andrew, I. Darby, and B. Lennox, “Accessibility Framework for Determining Collisions and Coverage for Radiation Scanning.,” in Lecture Notes in Computer Science, Springer Nature Switzerland, 2024. '
---

Radioactive contamination monitoring is an important part of radiological protection. Automation of surface monitoring poses difficulties, with a major challenge being determining the coverage of a radiation probe over an object in close proximity without collision. We propose a new accessibility framework to determine if radiation probes, modelled as convex hulls, collide with 3D point clouds representing the objects. We explain how to structure and analyze point clouds to extract properties such as the surface normal for each point. Our method for approximating radiation probes is demonstrated using the BP4 probe. This approach models both the probe and the sensor&apos;s effective scan volume with geometric primitives, providing a computationally efficient way to detect collisions with flat surfaces. The accessibility assessment builds on common methods within computer science for determining intersections. A laptop in various positions was used to demonstrate that the framework can efficiently categorise points as accessible or inaccessible, identifying unscannable regions. The output of this framework can then be used to plan collision-free paths over objects and will be the foundation of a robotic survey assistant. 
