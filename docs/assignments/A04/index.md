# A4 – Motor Mount

## Overview
For this assignment, we are taking the example of a Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox motor and creating a mount that is resistant to any excess stress or deflection on it. These are the directions along with a rough visual of how the motor would be affixed to the mount;

<img width="947" height="451" alt="Screenshot 2026-09-16 225955" src="https://github.com/user-attachments/assets/1f26cfdd-c8f9-4a4c-8675-700ac733704b" />

Before we begin the analysis and construction of this mount, it is imperative to break the mount apart into two separate members that I can analyze. This allows for me to better calculate which forces and dimensions are acting on which area of the mount and calculate values much easier. 

## Feature 1 Analysis

For feature 1, which can also be observed as the base of the mount, it is easiest to envision it similar to a cantilever beam with a load and resulting shear force acting in the opposite direction. There is a fixed connection as it is assumed that the mount would be, well mounted, to a wall or other surface. My first course of action was to list all of the knowns and unknowns. The only provided information that was truly known was the force, safety factor, and the deflection limit. The other values such as the length, width and material were all things that I were given the freedom of making up. I chose my material to be PLA as it is what I am most familiar with, and chose the width dimension to be 40 mm and the length to be 60 mm. The next step was figuring out what I needed to solve for. As one of the main objectives with calculating in the first place was determining the minimum needed thickness of the mount, it was imperative we test the required thickness for both the stress and deflection and utilize whichever was larger so both conditions are properly satisfied. After drawing my FBD of the first feature, I then calculated to discover which failing property governs the other and overall which dimension we should use for this feature. My findings can be observed below; 

<img width="3024" height="3038" alt="IMG_2979" src="https://github.com/user-attachments/assets/f90d9f57-a229-4ef5-bcdd-d48d06b59bc8" />

After my calculations, since the deflection required a larger thickness than the stress did, I picked the deflective thickness of 18.34 mm to utilize for feature 1.

## Feature 2 Analysis

When navigating to feature 2, I knew from the beginning it was going to be a very similar process as the first one. I picked a length/height of 50 mm for this one and the width remained the same at 40 mm. All of the before given information remained the same, however there was an inverse moment created by the wall that did not show up in the FBD of feature 1. This makes sense that the moment acts in an opposite direction to the other moment as they have to reach some sort of equilibrium. From here, the process remained the same where I was looking to find which thickness was greater between the minimum required stress and the minimum required deflection. 

<img width="3024" height="2689" alt="IMG_2980" src="https://github.com/user-attachments/assets/381b7779-4083-4d26-836a-08944112ae75" />

After calculating, it was evident that the deflection was once again greater, so I was to use a thickness of 21.34 mm for feature 2 of the mount. 

## Isometric Sketch

The next course of action was creating an isometric sketch of the mount now that I had dimensions to attribute. 

<img width="3024" height="1471" alt="IMG_2981" src="https://github.com/user-attachments/assets/eb4e0a4e-37fd-4738-8402-fac5d204b61b" />

As seen in the sketch, the deflective thickness that I calculated for above were labeled in the sketch. This sketch is a good visual for how I should see my design once I create it in Solid works. 

## CAD Design

The final step of the process is to take that isometric sketch I just completed and transforming it into a CAD software. I knew going into this that this design was well within my capabilities and would not be immensely difficult to complete. 

I started with the base rectangles of the mount and extruding them into a thickened L-shape;

<img width="1502" height="697" alt="Screenshot 2026-09-17 003808" src="https://github.com/user-attachments/assets/5f887617-30fb-4747-a254-2d92d75b3e2e" />

<img width="1007" height="642" alt="Screenshot 2026-09-17 004142" src="https://github.com/user-attachments/assets/6063f8ca-254f-4cb3-9d0e-f4f77cd60831" />

After the base of the mount was complete, it was time to get into the finer details that would ensure the motor would probably affix to the mount. The first step was extruding down a circular port in which the motor can comfortably sit and not dislocate. I utilized the provided dimensions of the specific motor I was basing the mount on in order to make sure the port was the perfect size for it to rest. Then it was time to cut four evenly spaced clearance holes in which bolts can go. These bolts will do the actual mounting and hold it together with a wall or whatever else the motor is to be attached to. 

<img width="801" height="580" alt="Screenshot 2026-09-17 005145" src="https://github.com/user-attachments/assets/1569c41a-2c82-44b4-84a5-aa64b5b05a47" />

<img width="987" height="672" alt="Screenshot 2026-09-17 010032" src="https://github.com/user-attachments/assets/150d9dc0-7a9a-4677-ade3-e3e666a63dea" />

Now that all the necessary components were completed, the next course of action was making sure the mount was secure and has as little stress and deflection as possible. I had the idea of creating ribs in order to ensure the stress levels where the two features intersect were much lower as well as the deflection as the tips of both of the features would be heavily reduced. 

My first attempt at this was to create a plane that went through the mount and sketch  line that connects the vertical wall to the horizontal one. The ribs would be applied on both sides of the created plane. However, when I went to attempt this, it would not let me create the rib between the resting port and the end of feature 1 no matter where I placed it. I gathered there was simply not enough space to put a rib there without overlapping.

<img width="528" height="690" alt="Screenshot 2026-09-17 011345" src="https://github.com/user-attachments/assets/88bcf4e8-6e7f-4c4b-8d80-c303bccd7c4d" />


My next idea was to create my own extrude and have that serve as a rib.  After trying this on both sides and offsetting the extrude 1mm so it was not directly on the edge, I believe it turned out great and definitely would reduce the stress and deflection of the mount. 

<img width="737" height="562" alt="Screenshot 2026-09-17 012250" src="https://github.com/user-attachments/assets/09cad502-8d6a-4070-9f0f-c8668d5e64b4" />

## Lessons 

All in all, this was the motor mount that I calculated for and then designed. It was a very fun project to experiment with and test the importance of having limitations when it comes to deflections and high levels of stress in your design. It has been made imperative that these sort of things can alter products and cause them to fail. 



