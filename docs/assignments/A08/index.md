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

### Rough Sketch of Design

Before I begin the difficult part of the project where I actually design the gear box, I was prompted to make a sketch of all the components as well as the housing that holds the gears and makes it a box to begin with. 

<img width="2664" height="1223" alt="IMG_3262" src="https://github.com/user-attachments/assets/646eb15b-3780-493a-89cf-f1ff7a53ca6e" />

While the sketch is hard to comprehend, I believe it was adequate enough to maintain a basic understanding of how to design this. One thing is I noted that to keep the housing elements of the gear box together, I would use a snap fit structure to do so. After some thinking, I decided that I would use bolts for the product in more practical purposes as it may be a little more sturdy than snap fit connections. 

## CAD Designing

Now it was time for me to begin drafting many different parts that I would eventually assemble into one assembly of the gearbox. Since the gears and bearings were linked for me already, I decided to download them into Solid works to get them out of the way. However, I faced a significant problem. My computer would not allow me to download the McMaster files. My only other choices was to design them manually.

<img width="375" height="192" alt="Screenshot 2026-10-29 014306" src="https://github.com/user-attachments/assets/0372e887-f52d-4ac4-b08f-d61a609cdec9" />

### Making the Shafts

Out of all the pieces, I knew that making the shafts would by far be the easiest. These were my parametric modeling dimensions for the input and output shafts respectively.

<img width="777" height="87" alt="Screenshot 2026-10-29 021811" src="https://github.com/user-attachments/assets/7cd0428f-8408-46f5-b2ff-c4cc3df75a39" />

<img width="798" height="90" alt="Screenshot 2026-10-29 022208" src="https://github.com/user-attachments/assets/9f2b32a1-eaec-4ce9-a7ca-f62695bcd720" />

Like I stated, the steps for this part were fairly simple. I created a circular sketch and extruded it into two separate size cylinders, one for the output shaft and one for the input.

<img width="487" height="567" alt="Screenshot 2026-10-29 022007" src="https://github.com/user-attachments/assets/0688e450-406f-4b4a-93dd-7be753ba36bf" />

<img width="1390" height="687" alt="Screenshot 2026-10-29 022351" src="https://github.com/user-attachments/assets/b71cf8f9-d051-4c96-9c61-aebac2f55d08" />

### Making the Housing/Lids

This part was most definitely more sophisticated than creating the shafts. There were a lot more parametric dimensions to account for, however the idea was not too difficult to figure out. It helped that I designed the base of the housing to be very similar and merely identical to the lid of it. 

<img width="773" height="193" alt="Screenshot 2026-10-29 022931" src="https://github.com/user-attachments/assets/b40cb39f-586b-471e-ac0b-9ae5c7d59b49" />

<img width="808" height="540" alt="Screenshot 2026-10-29 023310" src="https://github.com/user-attachments/assets/7f7af0cf-0f04-4a69-9707-d4f71c5c2e19" />

It was important that almost all of the dimensions were exactly the same for the top as with the bottom to ensure that they fit accurately with the bolting geometry. 

<img width="796" height="517" alt="Screenshot 2026-10-29 023729" src="https://github.com/user-attachments/assets/2c6ddd82-4980-4d7f-ad3e-c275a1120eca" />

<img width="1471" height="708" alt="Screenshot 2026-10-29 023945" src="https://github.com/user-attachments/assets/7a6e19fb-2fa3-4c2a-8f7b-3f73d9426d1d" />

<img width="947" height="742" alt="Screenshot 2026-10-29 024912" src="https://github.com/user-attachments/assets/84626a19-ff22-4f4e-8fae-91d2390f32f0" />

I was very pleasantly shocked to find that the housing unit for the gear box turned out pretty good in my opinion. I was shocked that I was able to come up with it, although it could most likely use some enhancements.

<img width="800" height="468" alt="Screenshot 2026-10-29 033431" src="https://github.com/user-attachments/assets/4c8f0a17-a1e2-4917-b2e4-4cad2282d157" />

<img width="863" height="505" alt="Screenshot 2026-10-29 033523" src="https://github.com/user-attachments/assets/2327d3d6-79e3-4ef4-8b1b-c48cb61e0a2b" />

### Making the Bearings

Since I was unable to download that file, I was forced to make these from scratch as well. On a brighter note though, this process took almost no extra time to complete.

<img width="781" height="140" alt="Screenshot 2026-10-29 033759" src="https://github.com/user-attachments/assets/a5b06e74-fbf1-478e-82e6-6d379c2300fe" />

<img width="1292" height="647" alt="Screenshot 2026-10-29 033918" src="https://github.com/user-attachments/assets/b08aa33a-7281-4d54-9d2e-897e7ff19bc4" />

### Making the Gears

After the files failed to download, I was nervous about if I was going to be able to incorporate the gears into the mechanism. Luckily, I researched a feature in which I can imprint gears and other common tools directly into SolidWorks. I found it quite fascinating and it helped a lot. One of the only issues I faced was that the lowest number of teeth they have was ten, yet the project require nine. I was left with no other choice, so I chose to go with the ten teeth pinion in hopes it would not change much.

<img width="632" height="597" alt="Screenshot 2026-10-29 021132" src="https://github.com/user-attachments/assets/e5a28010-5612-4485-b8f1-d70e53329de9" />

<img width="660" height="371" alt="Screenshot 2026-10-29 040152" src="https://github.com/user-attachments/assets/c0162b2e-acf4-49b1-9571-397a085e50f5" />

## Assembling all of the Pieces Together

Now that I had created several separate parts, it wads time to assemble them into one singular gearbox. I started out by just adding all of the components in and mating them one at a time in order to look similar to the image I had in my head. 

<img width="850" height="726" alt="Screenshot 2026-10-29 041207" src="https://github.com/user-attachments/assets/628af43b-d330-4689-b4a4-1e94be6528e7" />

<img width="787" height="686" alt="Screenshot 2026-10-29 042520" src="https://github.com/user-attachments/assets/2b2e3fa9-caaa-43f7-9c0b-78a7334a8019" />

<img width="797" height="665" alt="Screenshot 2026-10-29 042634" src="https://github.com/user-attachments/assets/1dec5296-9455-4926-968b-9716edd3febd" />

<img width="702" height="583" alt="Screenshot 2026-10-29 042724" src="https://github.com/user-attachments/assets/b2c8d645-01ac-4241-b070-7bfb84193b09" />

Overall, there were definitely some dimensional errors I made with the gears. If I had more time, I would change a lot of features on the geometric side of things in order to ensure that the gears can fit inside of the box and not be hindered by an obstacles or interferences. 

## MEGR 2157 - Drawing

Given that I had the gearbox all assembled, the final step was to make an engineering drawing given the prototype of what I did. I wanted to incorporate as many views as possible that give insight of what is going on within the mechanism that may not be noticeable when within the housing box. 

<img width="898" height="693" alt="Screenshot 2026-10-29 050254" src="https://github.com/user-attachments/assets/1ceafc52-993d-43d4-9a4f-a7091c93c8a2" />

## Lessons Learned

I learned so many things over the coarse of this project. For one I learned how even with access to parts setting up and analyzing a design is a long and meticulous process and should not be taken for granted. While none of my observations during my pre-design analysis showed any signs of failure, it is still so important in advanced projects such as this one to ensure that all elements are satisfied and will not yield under special circumstances. I learned that when there is technology issues there is always another way around things. While it took me a lot of time to do so, I am satisfied with knowing that I did my very best with the time provided to improve my design. 

[GearBox_AssemDrawing.pdf](https://github.com/user-attachments/files/34127545/GearBox_AssemDrawing.pdf)

[GearBox_AssemDrawing2.PDF](https://github.com/user-attachments/files/34127551/GearBox_AssemDrawing2.PDF)
