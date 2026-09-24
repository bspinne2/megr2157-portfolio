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
