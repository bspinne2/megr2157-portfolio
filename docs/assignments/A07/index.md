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
