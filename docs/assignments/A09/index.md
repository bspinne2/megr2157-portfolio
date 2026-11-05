# A9 – Pulley System Design

## Instructions/Objective

<img width="1053" height="881" alt="Screenshot 2026-11-04 192814" src="https://github.com/user-attachments/assets/80313ecb-f9a5-48fa-baec-d225e59887df" />

<img width="1040" height="760" alt="Screenshot 2026-11-04 192830" src="https://github.com/user-attachments/assets/f72b4d8c-baf4-4a10-88e2-7e0862210949" />

<img width="1011" height="941" alt="Screenshot 2026-11-04 192845" src="https://github.com/user-attachments/assets/5b6a337b-32b7-49f5-a12a-66bb7c2aebc6" />

For this assignment, I am to analyze a pulley system and each of the components of it. I am given a certain list of restraints listed above with a small range in which I can choose specific values. Unlike other assignments, this one does not require me to design in a CAD software such as SolidWorks, but rather prompted me to perform on-paper analysis and planning for each element of the suggested pulley system.

## Belt Analysis

The first area I investigated was the belt system of the pulley. The belt was listed to be made from polyurethane rubber, giving it a yield strength of 3.25 MPa (471 psi) at 20% strain. Below is my written experimentation with this belt system;

<img width="3024" height="4032" alt="IMG_3306" src="https://github.com/user-attachments/assets/6611e51c-77be-49ba-b78f-8db20fde3193" />

The first step I took was to list out all the knowns and unknowns given the provided information. For all criteria giving flexibility with a range of values to choose from, I opted to pick the middle value of the range for simplicity. These values included the center distance, rotational speed, and static belt tension. The unknowns are everything I symbolically solved for and utilized to find the cross sectional area and diameter of the belt which is the main criteria I was to figure out.

The FBD I drew was very similar to Figure #1 shown in the instructions, featuring two pulleys connected by a loop. During power transition, there is a tight side and a loose side labeled by the FBD which accounts for a proper pulley flow. Slippage is considered to be neglible in this analysis.

Setting up the equations for the unknown variables were pretty self-explanatory. Given the belt friction and torque relationship equation, the centrifugal force is ignored to maintain a simple analysis and theta is equivalent to pi for flat/round pulleys. Given the above analysis, the outer length of the belt was found to be 19.42 inches, the cross-sectional area of the belt was found to be 0.0459 squared inches, and the belt diameter is about 0.242 inches.

Given these recorded dimensions, I was to assign a belt that adequately satisfies all required conditions. I searched McMaster-Carr for around a 1/4 inch diameter polyurethane round belt with a length of approximately 19.4 inches long.

<img width="1062" height="286" alt="Screenshot 2026-11-04 210142" src="https://github.com/user-attachments/assets/44d1604a-de06-4ca0-a09e-cf9a200daa92" />

The best fit given the dimensions would be the second option from the top, with length between the 12 and 24 inch outer circumference.

## Shaft Analysis

The next thing I analyzed was the support shafts subjected to pure torsion from the pulley and radial reaction forces. These shafts act as carriers for the power throughout the pulley system. The shaft was chosen to be 1060 hardened steel which holds a yield strength of 65 ksi.

<img width="3024" height="4032" alt="IMG_3307" src="https://github.com/user-attachments/assets/e6cd5e83-d1d6-4985-9ebf-72cc1626f0db" />

Just like with the belt, I began by listing all of the relevant knowns and unknowns specifically to the shaft. For optimum sufficiency, a safety factor of 3 was assumed. The only unknown in this analysis was the shaft diameter.

The FBD demonstrates the cylindrical shaft being subjected to an applied torsional moment "T" at the pulley mounting location.

When calculating the transmitted torque variable, I utilized the Force dimensions calculated for during the belt analysis. I then used this value to calculate the maximum shear stress for pure torsion which is what the shaft is in. All of these values resulted in a shaft diameter of 0.146 inches. However, for an even better guarantee of safety, I should utilize a much large diameter value for practical applications to maximize efficiency. 

## Journal Bearing Analysis

The next area of focus was on the journal which acts as the critical mechanical interface between the rotating shaft and the stationary support frame. This component ensures the highest level of structural integrity of the system as it reduces high amounts of friction and excessive heat. The bearings are assumed to be some sort of porous metal material.

<img width="3024" height="4032" alt="IMG_3308" src="https://github.com/user-attachments/assets/19d6283c-6b56-4fc3-95b8-b00261ebf9b6" />

Given the important function of the bearings within the system itself, it contains many variables that need to be calculated for, such as the bearing area, pressure, linear velocity and the PV factor. All of these variables allow me to determine the material suitability of the bearing to prevent failure.

The FBD shows radial reaction forces represented by the variable of "W" acting on the sleeve/journal bearing supporting the rotating shaft. 

Assuming the length of the bearing is 0.5 inches to match the shaft diameter which is standard for plain sleeve bearings, I began to solve for the pressure and velocity values. After calculating, I found that pressure is 40 psi, the velocity is about 196.35 ft/min, and the PV factor is about 7,854 psi * ft/min. 

Given this data, I investigated the Machinery's Handbook and found that oil-impregnated porous bronze (sintered metal) is a very suitable choice as it has a maximum PV limit of between 20,000 and 50,000 psi * ft/min. My calculated value was well within this range so it holds sufficient.

## Frame Design

The final area of focus was to design a frame that holds the two shafts at the required center distance while supporting the belt tension loads without failing. The frame rough design was given by Appendix A for visual aid. 

<img width="3024" height="4032" alt="IMG_3309" src="https://github.com/user-attachments/assets/5c5748c1-77fc-42ff-ae01-d9f3a08e0f5f" />

The beneficial part about designing the frame was that most of the work and dimensioning was already done in prior steps. Most variables like the space between the shaft holes and pre-tensile load were already solved for in prior analysis. In this aspect, the pre-tensile load acts as a tensile/bending force attempting to pull the two bearing hubs together.

In terms of the material I chose, I decided to go with a simple Aluminum 6061-T6 with a yield stress of 35 ksi. The width, thickness, and hole diameter dimensions were choices to increase the optimization of the bracket. 

I then calculated for the max stresses that can be analyzed given my dimensions to discern if it is subject to failure or not. Given my calculated safety factor was 202.5, which is much larger than the suggested safety factor of 3, I would consider design to be satisfactory. 

## Lessons Learned

Overall, breaking up the several components of this pulley system was not super challenging to complete. Given that a lot of the equations and variables began to repeatedly come u made it easy to solve for new values. Furthermore, I learned how integrating mechanical constraints across components—such as sizing the belt cross-section for maximum allowable normal stress, scaling the shaft diameter against torsional shear limits, and verifying that journal bearing PV parameters remain within safe thresholds are crucial to designing a sustainable system that does not fail once manufactured. These calculations can potentially save a lot of time and resources from the effects of making a mistake, especially in expensive manufacturing. 
