# A7 – FEA On Bracket

For this assignment, I was tasked with taking the Bracket design I had already in a prior assignment and running a finite element analysis on it given fixtures and loads being applied to it. For this process, I was to perform a multi-loop process where I run studies on my current bracket design with differing mesh sizes, and record the values associate with each. After recording all of the values, the outer loop portion of the assignment tasks me with making adjustment to my bracket to optimize the material and stress and deflection concentrations on it and making for a more optimal bracket. 

## Inner Loop

The first step of this inner loop process was to apply the load enacting down on the pin in the form of the strap, as well as the fixtures that can be applied to the inside of where the bracket would mount. This part is essential before I can begin analyzing the bracket accurately. 

<img width="1237" height="727" alt="Screenshot 2026-10-21 231114" src="https://github.com/user-attachments/assets/34e913b1-1542-4c69-81b9-cce62f28bd08" />

I was having troubles applying the load directly onto the bottom face of the pin, so I had to utilize the top plane as a reference point for my load. 

Now that my constraints and loads were attributed to the bracket, I was able to begin running the simulation. 

### Coarse Mesh Analysis

I began by analyzing the bracket given a coarse mesh model, roughly 1500 elements. It was very evident from this initial study that my values for the stress and deflection was extremely high. This bracket regularly would fail almost immediately given the lack of support and modification it had. 

<img width="1476" height="661" alt="Screenshot 2026-10-21 231751" src="https://github.com/user-attachments/assets/16ccf6ee-110f-4be1-8840-a5c8ff06c04f" />

It is interesting to note how high the stresses are on the narrow arm of the bracket. This would definitely be something I would need to adjust during my design optimization section. 

### Medium Mesh Analysis

I then ran a medium size mesh analysis of the bracket with no adjustments to the geometry. It is with the higher mesh count that I could observe how the value altered given how many elements there are. In this run, there were around 7500 elements. Noticeably, the points of Von Mises stress and deflection values were higher in the medium size mesh as opposed to the coarse mesh. 

<img width="1106" height="562" alt="Screenshot 2026-10-21 234857" src="https://github.com/user-attachments/assets/7d9a9313-9813-479d-8eb8-b73b6c7dd006" />

 While many stress points still occurred on the arm of the bracket, there was interestingly more stress on the edges of the pin as well as the edges of the arm itself. A lot more red could be observed on the arm of the coarse mesh analysis than the medium mesh analysis.

 ### Fine Mesh Analysis

 The fine mesh analysis showed the biggest amount of elements to analyze the bracket. Approximately 66,000 elements were recorded. This amount was way more than I expected it to be. As predictable as well was that the stress and deflection magnitudes were marginally higher than the prior two meshes. 

 <img width="1091" height="570" alt="Screenshot 2026-10-21 235743" src="https://github.com/user-attachments/assets/8b90a2ab-24f8-473f-9d21-190dc0d1d1d8" />
 
I was surprised to find how little red I found on this analysis. There were a lot of yellow and green present, but only a few small concentrations of high stress marks. 

### Calculated Mesh Values

<img width="2287" height="3381" alt="IMG_3222" src="https://github.com/user-attachments/assets/65a13a40-2c35-43e9-95c6-8f9941cbb8fa" />

It can be observed pretty easily from these calculations how unstable this bracket stands with no moderation. Regardless of the mesh size, the safety factors for the bracket are not sustainable in practical application. It can also be noted how a higher/finer mesh size equates to a larger max stress as well as a larger max deflection. Given the bracket at its current state, it did not fall within the 7 percent threshold, therefore the results did not converge.

## Outer Loop

Now that an initial inner loop analysis was performed on the bracket, the next step was to make some serious modifications to the bracket itself. The purpose of these modifications include making the build have less material, lower stress points, less deflection, and higher strength and stiffness. My specific area of optimization resolved around ensuring that the criteria converges and lowering the stress and deflection concentrations on the bracket. 

My first coarse of action was to increase the thickness of the arm of the bracket. Given how long and slim it was, I was certain it caused a lot of stress points to be present that could have been avoided. I changed this value to 0.2mm thick. Additionally, I created a circular cut throughout the arm to remove extra material and get rid of some of those stress points. Since a circular cut leaves no sharp edges behind, it is optimal for reducing stress concentrations in a build. 

<img width="686" height="573" alt="Screenshot 2026-10-22 003329" src="https://github.com/user-attachments/assets/05da3e7d-906f-4037-a0e6-0807b6a92ac8" />

Now that I did some initial changes to the geometry of the bracket, it was time to reanalyze the concentrations present on it. 

<img width="1122" height="595" alt="Screenshot 2026-10-22 003430" src="https://github.com/user-attachments/assets/3c05bc52-1904-4aad-9c4d-ac1100c87536" />

<img width="1102" height="617" alt="Screenshot 2026-10-22 004106" src="https://github.com/user-attachments/assets/47bde21e-d84e-4d5e-9ba0-75220b49eb05" />

As can be observed above, the slight changes in geometry drastically altered the max concentrations present on the bracket. While red spots still appeared, it was a path in the right direction towards creating an optimal and safe bracket. The above analysis was ran on a fine mesh study. I compared these calculated values to a medium mesh study to see if the configurations converge or not.

<img width="3024" height="2179" alt="IMG_3223" src="https://github.com/user-attachments/assets/eb20dba5-4cc2-4073-9fd7-30c5f310f506" />

Given the percent change was less than the 7% threshold, this mesh does indeed converge unlike the original. 

Despite improvement being noticed, I decided to make a few more minor adjustments to the geometry. I added some fillets on any sharp edges in hopes that it would further reduce any stress concentrations. 

<img width="982" height="751" alt="Screenshot 2026-10-22 005256" src="https://github.com/user-attachments/assets/6c955599-54dd-4b48-911e-de614c6dde3e" />

<img width="1062" height="707" alt="Screenshot 2026-10-22 005407" src="https://github.com/user-attachments/assets/01c28376-0558-42f8-9c58-2895f67256d9" />

<img width="933" height="777" alt="Screenshot 2026-10-22 005608" src="https://github.com/user-attachments/assets/7bd27a6d-6c43-4759-8eea-ef5717e31c87" />

I was surprised that these changes in geometry did not actually reduce the max stresses on the bracket like I had hoped. There were many more changes that could have been made to further improve and make a fully functional bracket, however I was satisfied with what I had managed to accomplish.

## Lessons Learned

I spent a lot more time on this assignment than I had thought I would. I had done finite element analysis before, but I definitely believe I grasped a deeper understanding of different elements of a design and how different factors affect the overall stability and function of it. Specifically, I learned how a finer mesh with more elements creates areas with larger max Von Mises stresses and displacements than more coarse mesh. I also learned how to alter basic geometry in a build to reduce these stress points, such as adding fillets to reduce edges, or creating circular cuts to remove material and keep stresses to a minimum. Inclusively, I learned that FEA is a constant process and is crucial towards optimizing whatever it is that is being designed. 

## 2157 Only work

I had trouble understanding what to do for this part. It says repeat the process for the link but there is no link that brings me to a separate geometry or method for me to analyze. 




