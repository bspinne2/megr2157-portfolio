# A5 – Bracket Design

For this assignment, I was tasked with analyzing the minimum thickness/radius of different sections of a bracket design given a stress and stiffness analysis. I was given certain parameters, constraints, and figures to assist with modeling the bracket istelf;

<img width="937" height="747" alt="Screenshot 2026-09-23 204712" src="https://github.com/user-attachments/assets/9da2d0c5-9e99-49be-b1e6-e4043654809c" />

Before I begin the assignment, I was to pick certain representative values that satisfy all the prompt's boundary conditions. I decided on an applied load(F) of 600 lbf, a safety factor of 4, the material Aluminum 6016-T6, and allowable deflection of 0.005 in. and allowable stress of 10,000 psi. 

## Strap pin/Cylinder - Feature A

### Stress Analysis

<img width="3024" height="4032" alt="IMG_3015" src="https://github.com/user-attachments/assets/3340a78f-4e4d-4d54-9976-75eef718db15" />

Since the pin was in the shape of a cylinder, rather than searching for a thickness, I was trying to find the minimum radius that is satisfied by the stress on the pin. The length of the pin was assumed by the width of the strap. Since the pin was fixed at feature B, there was a max moment present at the root of the pin. I utilized the basic formulas for the cross section as well as the moment and rearranged them to solve for the minimum required radius given the stress. The diameter was solved to be around 0.674 inches.

### Stiffness Analysis

<img width="3024" height="4032" alt="IMG_3016" src="https://github.com/user-attachments/assets/7cd702f1-c0ef-4fc8-85f4-9d89e92ef4a3" />

This procedure was very similar to that of the stress analysis. The FBD, knowns and unknowns were practically the same. However, rather than utilizing a section modulus for a cross section, I utilized a deflection formula to locate the minimum required radius/diameter given the stiffness. This value was calculated to be a diameter of 0.418 inches. This means that when I would go to design this bracket I would opt to use the radius given by the stress analysis as it is greater and both minimums must be satisfied to prevent the bracket from failing in any way. 

## Vertical Support Arm - Feature B

### Stress Analysis

<img width="3024" height="4032" alt="IMG_3017" src="https://github.com/user-attachments/assets/8f30b0a4-ffd4-475f-be3d-181a2ff5d60f" />

These observations and calculations were very similar to that of the first stress analysis. A key difference in analyzing the arm is that it has a rectangular cross section, meaning I am analyzing the minimum required thickness rather than the radius/diameter. It is an interesting observation that the length of the arm is the same as that of the cylinder, only emphasizing their proportionality. Another observation that could be seen from my on-paper analysis is that the arm is in axial tension as the presence of the load is pulling the arm in an equal and opposite direction. The thickness was calculated to be 0.060 in. 

### Stiffness Analysis

<img width="3024" height="4032" alt="IMG_3018" src="https://github.com/user-attachments/assets/bff3f38c-94cb-4149-b24d-c4d1e97ceb08" />

An interesting observation that can be discerned from the stiffness analysis as opposed to the stress analysis is that the assumed arm length is different, as the length is assumed to be 1.5 inches given by the diagrams on the criteria page. Similar to the first stiffness analysis I performed, I rearranged a deformation equation to discover the minimum required thickness. This value was 0.018 inches, meaning that once again I would use the stress analysis value to accommodate both boundaries.

## Bottom Channel base Plate - Feature C

### Stress Analysis

<img width="3024" height="4032" alt="IMG_3019" src="https://github.com/user-attachments/assets/e3d2dae0-a1b1-4a28-a63b-0666ddab361d" />

For this long base plate, there is a point centralized force being enacted on the middle of the beam. This force is actually being transmitted from the arm in feature B. Because the force is being acted perfectly in the center of the beam, it is assumed there is equal reaction forces on either side acting in an equal yet opposite direction from the central force. The thickness of the plate due to stress was found to be 0.424 inches. 

### Stiffness Analysis 

<img width="3024" height="4032" alt="IMG_3020" src="https://github.com/user-attachments/assets/9b13fa1b-cd66-4025-af12-96477363affc" />

The same criteria applies for the stiffness analysis as the stress analysis. Utilizing a deformation equation, the thickness due to stiffness is uncovered to be 0.288 inches. This means that once again, the stress calculated value governs over the stiffness value.

## Channel Side Wall - Feature D

### Stress Analysis

<img width="3024" height="4032" alt="IMG_3021" src="https://github.com/user-attachments/assets/d5400cce-fabc-4af1-a902-c369523fe5b1" />

For this analysis, I am analyzing only one channel side wall as the bracket is symmetric and they are identical to one another. On each side wall, a tensile load is being applied due to the load acting on the bracket. It is assumed that the total load is split between the two sides in pure tension due to the symmetric geometry of the figure. The thickness due to stress of each individual wall would be 0.030 inches.

### Stiffness Analysis

<img width="3024" height="4032" alt="IMG_3022" src="https://github.com/user-attachments/assets/6b76429a-a3b5-4626-8a30-7816f8d21767" />

The criteria for the stiffness analysis is once again the same as with the stress analysis. There is 300lbf in axial tension on each individual wall. The thickness given substitution with formulas was solved to be 0.009 inches. It seems to be a common trend where the stress analysis is yielding a larger minimum thickness than that of the stiffness analysis.

## Engaging T-Beam - Feature E

### Stress Analysis

<img width="3024" height="4032" alt="IMG_3023" src="https://github.com/user-attachments/assets/6bc10e7a-5197-4929-9e6b-2ea1f0b0e5d0" />

For this feature we are analyzing the overhanging flanges of the bracket and our minimum thickness very similar to the prior features. An interesting aspect of this feature is that the flange is actually acting as a cantilever beam with a center point load acting right in the middle of the overhanging flange. A load of 300 lbf is on each side of the bracket. For this solution I evaluate as there is a moment present where the load is acting on the flange. The thickness was recorded to be 0.212 inches.

### Stiffness Analysis

<img width="3024" height="4032" alt="IMG_3024" src="https://github.com/user-attachments/assets/3c7a1385-1424-4fe6-af3c-fcb39d4b6723" />

It is also assumed there is bending with the point load as there is a clear overhang with the flanges. However, I still calculated in a very similar way and found that flange thickness for stiffness is 0.072 inches. 

## Multiview - Stress Analysis

<img width="3024" height="4032" alt="IMG_3025" src="https://github.com/user-attachments/assets/5bbd7e3e-f9c4-4be1-8005-c21f84402139" />

The objective of this part of the assignment is to create a bunch of 2D orthographic sketches utilizing all of the values and dimensions I just solved for assuming the bracket is exhibiting the minimum possible thickness. Given a safety factor of 4.5, when designing you would take whatever dimensions I evaluated for and multiply it by that factor to ensure that the bracket is structurally sound. There were some issues with proportionality I am sure with how big I made some of the walls and how much of a magnitude each dimension was. 

## Multiview - Stiffness Analysis

<img width="3024" height="4032" alt="IMG_3026" src="https://github.com/user-attachments/assets/82dc41d7-5665-4d41-bd7c-ddf2592784f1" />

In a probably unsurprising manner, the orthographic drawing for the stiffness diagram are nearly identical as they are nearly the same proportions and dimensions. However, there is definitely some minor dimension errors as all of the minimum required thicknesses for the stiffness analysis was much less, most likely meaning the size should be relatively smaller. 

## Lessons Learned

One of the major things I learned is for at least this bracket alone, the stress dimensions had a much larger impact on governing the actual thickness dimension of each of the features. The stress dimensions were always noticeably larger than the stiffness ones. An instance where a value was carried on from one feature to another was the axial load being carried on and then divided in half to account for the load being distributed on either side of the bracket. Going hand in hand with that, an assumption I made was that the bracket was in fact a symmetrical shape, meaning that the load was evenly distributed across it(300 lbf each). If this assumptionw as wrong, a lot of values would be altered significantly. 
