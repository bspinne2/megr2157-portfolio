# A8 – Gear Box Design

For the purpose of this project, I was tasked with taking two already suggested and evaluating a proper gearbox design for them that will allow them to function accurately. This project required a lot of preparing and research work in order to ensure that the many components to the gear box were practically and numerically sound. 

<img width="510" height="575" alt="Screenshot 2026-10-29 050655" src="https://github.com/user-attachments/assets/95bad481-6399-423b-a30b-b0c52d03ce89" />

## Design and Calculations

To begin this project, a major portion of it is to analyze both input and output components within the gearbox. The input components are where the kinetic energy is dispersing into first within the system. The movement then transitions to the output components, which in terms of gears are often a direct result of the movement on the input components. 

<img width="3013" height="1174" alt="IMG_3257" src="https://github.com/user-attachments/assets/04cba3f1-f1df-4a0d-b910-fe74ddfe38c8" />

The first step is to list all of the givens and constraints for the project that will be useful for future calculation. An interesting part of these values are that they all represent a proportionality between an input and output component.

### Input Shaft

The first direct focus of analysis would be the input shaft. This would be the cylindrical member that is being rotated to propel the mechanism to work in the first place. When constructing these shafts, I decided to keep it easy for myself and neglect any friction forces being acted on by the shafts. In real life, this can be a purpose of lubrication or clearances to prevent any ware on the mechanism.

<img width="2408" height="2509" alt="IMG_3258" src="https://github.com/user-attachments/assets/4efd04ef-1fb7-4940-badc-6b64d3842e67" />

I followed very closely with the procedure and rubric for this analysis section. I first listed knowns given by the constraints as well as my previously calculated values, and the unknowns are simply what is important to analyze about the shaft to ensure optimization is being achieved. The next step was to build an FBD of the shaft. To maintain simplicity, I used a straight line as symbol for the cylinder that the shaft would typically be. The reaction forces of the bearings on the shaft act in an opposite direction of the tangential force on the shaft. There is also a torsional stress force acting on the shaft. After calculating for all the unknowns, I took the largest stress force and compared it with the yield strength to determine how large of a factor of safety I had for the shaft's design.

### Output Shaft

The setup and analysis for the output shaft was immensely similar to the input shaft. The process is identical, however the values were slightly different as they diameters were altered in order to compensate for a larger gear.

<img width="3024" height="3155" alt="IMG_3259" src="https://github.com/user-attachments/assets/4d8abc54-213d-4242-acea-5743aad5a7eb" />

While the input shaft was well within a satisfying level of sufficiency, this output shaft had an even safer cushion before any failure would happen.

### Journal Bearings (Pressure, Velocity, and PV)

Now that the shafts were observed, the next course of analysis was on the bearings wrap around the edges of both ends of the shafts. Similar to the shaft, there are two different types of bearing for me to analyze, the input and output bearings. It is important to pick a material for the bearings that satisfies both conditions.

<img width="2785" height="3798" alt="IMG_3260" src="https://github.com/user-attachments/assets/ea90a3dc-cde0-4b72-b547-d5cd88485d60" />

The analyzing process was very much the same. State the knowns and unknowns, research and find the formulas for each missing factor, and solve each criteria given what numerical values I had. While I was only analyzing the bearings, the FBD only analyzed two forces, a main force and a reaction force. All elements of both bearings were well within a sufficient range for design. In order to utilize a material for one or both of the bearings, the calculated values must be less than the provided max values for a specific material. 

<img width="977" height="423" alt="Screenshot 2026-10-29 053910" src="https://github.com/user-attachments/assets/a0065be5-4945-4dce-9220-2308f039830e" />

Given how low a bunch of the criteria is, many materials actually work for the bearings. However, to optimize cost and resources, I believe the best material would be Acetal or Nylon, Polycarbonate.

### Journal Bearings (Thickness)

With continuing my analysis on journal bearings, the next focus was to discover a suitable thickness. The process was the same for the on paper analysis. One thing that was a little different was that the FBD was from an axial perspective rather than a right facing view of a cylinder. Given thickness was the only measurement I was recording, no other forces were acting on the FBD. 

<img width="2847" height="3947" alt="IMG_3261" src="https://github.com/user-attachments/assets/33ff49f3-706a-4cfe-ab50-072084c6cc0b" />

As can be observed the safety factor was almost 10, meaning that sufficiency was once again not a problem. When trying to find a specific thickness that fits the criteria but optimizes cost and efficiency, I could actually work backwards to find the smallest thickness that will prevent my build from failing. However, for the sake of this project, I decided that a thickness of 0.125 inches of one-eight of an inch was more than suitable.

The specific bearing that fits all my specific criteria are the Oil-Embedded SAE 841 Bronze Sleeve Bearing. 
