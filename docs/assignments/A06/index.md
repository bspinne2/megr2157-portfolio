# A6 – Bracket Drawing

<img width="861" height="512" alt="Screenshot 2026-10-01 001509" src="https://github.com/user-attachments/assets/e975b019-0164-44eb-8b00-c462a67c806f" />

This assignment is an extension of the A5 assignment, where I analyzed the dimensions that are satisfied by stress and stiffness calculations. When I get prepared to design the bracket, it is imperative to utilize the dimension that are satisfied by the minimum allowable stress and stiffness analysis for each feature of the bracket. Surprisingly, the governing failure mode for all 5 features I analyzed was stress. This means that I will utilize the stress dimensions when I begin drawing and designing within this assignment. 

As a refresher, here are my calculated stress values:

<img width="3024" height="4032" alt="IMG_3015" src="https://github.com/user-attachments/assets/f2a4f147-eab8-486a-98b3-f5d85019decc" />

<img width="3024" height="4032" alt="IMG_3017" src="https://github.com/user-attachments/assets/ef84e8db-23d4-4bce-bc2a-b75d0e85af84" />

<img width="3024" height="4032" alt="IMG_3019" src="https://github.com/user-attachments/assets/8f6bc610-8f06-4ac7-ad3a-0687431175e6" />

<img width="3024" height="4032" alt="IMG_3021" src="https://github.com/user-attachments/assets/b6679dcf-4c46-4ba6-abdd-b28649abde56" />

<img width="3024" height="4032" alt="IMG_3023" src="https://github.com/user-attachments/assets/033cdc68-74be-45fe-8f9c-7e4c4d2b408b" />

## Parametric Design

Despite the fact that I already calculated for specific restraining values, the assignment requires for parametric modeling to be utilized. This means that for each unknown dimension I need to implement the equation using known variables to determine specific values. Parametric modeling is very beneficial to ensure that mistakes can be fixed much easier when specific values are applied. Below are the applied variables I assigned in Solidworks;

<img width="765" height="112" alt="Screenshot 2026-10-01 004435" src="https://github.com/user-attachments/assets/6f68b02f-99c5-4db7-b8d2-261a26a839f4" />

<img width="712" height="213" alt="Screenshot 2026-10-01 004454" src="https://github.com/user-attachments/assets/0cfcf52b-e4a9-47d0-b176-d166ef029dd4" />

## Design Process

Part of the parametric modeling process is now assigning those specific variables to each of the dimensions of the bracket. This was a lot more challenging of a process than I had thought it would be as the under constrained line segments were moving around as I was trying to assign the values to them. After a lot of fidgeting around with it, I finally managed to get a rough geometry right.

<img width="816" height="598" alt="Screenshot 2026-10-01 013805" src="https://github.com/user-attachments/assets/360da86d-6f25-4d28-9aa6-aeb7b27a0ca6" />

<img width="1427" height="620" alt="Screenshot 2026-10-01 014340" src="https://github.com/user-attachments/assets/a7fa47f5-d3c6-41be-ac19-545f557d5591" />

<img width="1197" height="672" alt="Screenshot 2026-10-01 014353" src="https://github.com/user-attachments/assets/16b820cd-bba3-4c81-93fe-60eb98210550" />

### Adding "C" to Bracket
I began with modeling the "C" or top of the bracket attachment first as this was the largest piece of geometry. Something interesting that can be observed is that my design given the values I calculated for are very funny-looking and would most definitely fail in the real world. However, given the instructions, it is an accurate display of the calculated values. The long, skinny wall thickness dimension is due to the wall being in pure axial tension. Since the material is metal and can typically survive forces in pure tension it is strong enough to withstand the stress and stiffness acting on it. The instructions also allow me to ignore shear stress which lets this application work, where it never usually would in real life applciations.

### Adding the Arm

The next step was adding the arm to the bracket. Similarly, the design came out to be much difference than the model provided in the assignment page. However, the arm mathematically works. 

<img width="660" height="637" alt="Screenshot 2026-10-01 014816" src="https://github.com/user-attachments/assets/3588d4fa-483f-4b54-9e89-ce32a9511fc8" />

<img width="583" height="572" alt="Screenshot 2026-10-01 014925" src="https://github.com/user-attachments/assets/bc3b3f0d-f86d-407a-b4ba-9b4e96f6297d" />

### Adding the Pin

The final feature to add to the CAD design is the pin. This step was fairly simple and had the same logic as the prior feature components with how it turned out visually. 

<img width="392" height="465" alt="Screenshot 2026-10-01 015201" src="https://github.com/user-attachments/assets/c5984065-f82e-4d97-87a7-ef4668e0cd61" />

<img width="532" height="545" alt="Screenshot 2026-10-01 015247" src="https://github.com/user-attachments/assets/79024740-8d48-4cc3-b325-ad75d01b390d" />

Overall, my full Parametric modelling section for the bracket assignment can be observed below:

<img width="1517" height="617" alt="Screenshot 2026-10-01 015347" src="https://github.com/user-attachments/assets/87d837e2-3c01-425e-97a9-1b8032f634e2" />

<img width="1430" height="540" alt="Screenshot 2026-10-01 015357" src="https://github.com/user-attachments/assets/d4acc7a7-0940-40f0-baeb-8a3ed6e64e6a" />
