# FEM Simulation System
## Introduction
In this case, we will see a green house falling to the ground and being bounced off.

The task is based on Unity.

## Dynamics
We can choose to use the simple linear finite element methods or fem based on svd decomposision to acheive the effects.

The hyperelastic model is St.VK.

And We use explicit integral to update, which will cause numeric instability.

In the linear fem we calculate Green Strain and the 2nd Piola-Kirchhoff stress to get the 1st Piola-Kirchhoff stress. However in another case，We directly use the model's deformation map to differentiate the singular values to obtain the PK1 stress.

## Collision
Simple SDF collision detection and impulse responding.

## Interaction
Users can press 'space' to make it jump. If you press too hard, the impulse will be too much to make it explode.

## Effects

The effects of both methods are exactly the same.

https://user-images.githubusercontent.com/53171201/209669599-81fd3844-ce6f-40ca-9688-64c1679c2817.mov

