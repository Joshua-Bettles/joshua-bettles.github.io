---
title: "Planning and Control of Mobile Manipulators for Inspection of Clustered Environments"
collection: publications
category: preabstracts
permalink: /publication/2025-12-1-WBC-UKManipulator-2025
excerpt: 'This Abstract looks at formulating a whole-body controller for a mobile manipulator and applying coverage path planning techniques to allow inspection of clustered environments.'
date: 2025-12-1
venue: '7th UK Manipulation Workshop'
paperurl: 'http://joshua-bettles.github.io/files/Planning_and_Control_of_Mobile_Manipulators_for_Inspection_of_Clustered_Environments.pdf'
# citation: 'J. Bettles, A. West, J. Andrew, I. Darby, and B. Lennox, “Accessibility Framework for Determining Collisions and Coverage for Radiation Scanning.,” in Lecture Notes in Computer Science, Springer Nature Switzerland, 2024. '
---

Many industries have confined, clustered environments that require routine inspections. Nuclear facilities, in particular, have extensive pipe networks that pose additional radiological challenges, making human inspection unsuitable. A mobile manipulator can inspect areas unreachable by most mobile robots without the additional risks and hazards associated with using aerial robots. This work formulates a whole-body controller for a non-holonomic mobile manipulator as a Quadratic Program, utilising Vector Field Inequalities (VFIs) to constrain the system. We introduce a stochastic point-to-plane constraint to handle uncertainty in the walls’ localisation and an online path planner that combines coverage path planning and 3D reconstruction. We present our recent results on coverage path planning and discuss the process of redefining the task to combine it with the NBV into a single approach. We demonstrate how to extract constraints from point clouds and incorporate their uncertainties into the VFI framework, and we comment on the performance of these constraints at preventing violations. We demonstrate this through experimental results from a physical mobile manipulator operating in a confined environment, thereby proving the real-world viability of these approaches and concluding with a discussion of future work to generalise them to other primitives and environments and to provide formal guarantees.
