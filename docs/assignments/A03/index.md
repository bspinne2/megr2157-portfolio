# A3 – Parametric and FEA

## Parametric Design

The first steps for this assignment is to analyze the problem and gather what exactly we are looking to design. A sketch was already provided so there was no need for me to sketch out an FBD of the bar on paper. It is important to recognize that the bar has a distributed load being acted by it, one that we can choose between 300lbf and 500lbf to satisfy the criteria. It is to have no more than an Axial deflection of 0.009 inches and the bar is to be constructed of Aluminum with a Young's Modulus of between 8.5-11.5 x 10^6 psi. 

![Screenshot](Screenshot%202026-09-09%20130419.png)

### Solve for Values

Before I can focus on designing the beam in Solidworks, I first have to establish a few measurements that are well within the criteria. When taking into account what was already provided, the only thing still left unknown is the length of the bar. I solved for this using the direct tension elongation equation;

![Image Description](IMG_2927.jpeg)

I assigned the distributed force to be 400lbf and the Modulus of Elasticity to be 10 x 10^6 psi as both values are directly in the middle of the provided ranges. I also chose a random value for the width and height/thickness of the bar, and used these randomly selected values to solve for the length of the bar as demonstrated above. I did make a calculation error, the final length calculated is actually 56.25 inches. 

### CAD Design

When starting my design process, it was time to start creating some variables I can use to make assigning numerical values a lot easier. 

![Screenshot](Screenshot%202026-09-09%20144416.png)

It took me a few minutes to discover how to work this table and assign the equations and variables the right away. i attempted to use the variable, "Thickness," however the computer was unable to allow it for some reason. I changed it to "height" instead. 

![Screenshot](Screenshot%202026-09-09%20144427.png)

After finishing the rough geometry of the bar, I went back to read the instructions. I noticed a critical error I had missed, the cross sectional area must be circular. While I was confident I could recover from this mistake, I was frustrated I had missed such a significant detail. 

I knew I had to redefine my variables and guarantee that they all have values that satisfy the conditions. 




