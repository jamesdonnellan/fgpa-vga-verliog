---
layout: home
title: FPGA VGA Driver Project
tags: fpga vga verilog
categories: demo
---

Welcome to my FPGA VGA Pixel Art project, where Spider-Man's iconic mask comes to life! Using the Basys3 FGPA board, Verilog and digital logic, I adapted my pixel art design to replace the online image with my own recreation in 640x480.

**Basys3 FGPA Board & Reference Photo:** <br>                                        
<img width="318" height="241" alt="SoC Board" src="https://github.com/user-attachments/assets/0c4c5c96-72e9-41f9-8824-b097643990c5" /> 
<img width="318" height="241" alt="UpdatedSpiderManMask" src="https://github.com/user-attachments/assets/3426797c-ce80-43e7-b600-728c357a7821" />
<br> 

## **Spider-Man's Mask VGA Design**
### **Project Set-Up**
I used Vivado and a Basys3 FGPA Board to create my Spider-Man mask. I started by creating a new project, adding my template code files used in previous Labs, and then altered and added to them to create my design. 

<img width="1610" height="596" alt="Project Summary Photo" src="https://github.com/user-attachments/assets/0623e279-75fb-4346-8504-38662d82fad0" />
<br>
(Project Summary Window of my VGA Project Setup)

### **What Did The Template Code Do?**
The template code generates vertical colour bands on a VGA output. It took the column from the VGA timing module and used it to decide what colour each pixel should display. Then, using the RGB combination through 'if else' conditional statements, the colours got selected and displayed into 8 equal stripes.

### **My Simulation Process**
I used Vivado to simulate my VGA project. I then built the template code to ensure that everything was running correctly and that the VGA cable was working to display to correct colours. 

### **Synthesis**
After the simulation process, Vivado translated the VGA pixel-art into a hardware ready circuit, allowing my design to be mapped onto the Baysys3's FGPA. Then, Vivado's synthesis report highlighted how the design was structured internally, showing which parts of the code contributed to logic and other features. 

### **Demonstration** 
After setting up my project properly, here was my first steps to designing my Spider-Man Mask!
<br>
![image10 (1)](https://github.com/user-attachments/assets/e5033b1c-976c-4a61-a163-c70e9d503cf4)

## **My VGA Design - Spider-Man's Mask**
Growing up as a Marvel fan, I wanted my project to be something that I have an interest in. So for my project I chose to create a pixel art of Spider-Man. I felt it would be a manageable design to achieve in the projects timeframe. For design reference, I chose a spiderman pixel art from [PixilArt](https://www.pixilart.com/art/spider-man-pixel-art-sr254518abb76aws3). [1]
<br><br>
<img width="819" height="695" alt="image" src="https://github.com/user-attachments/assets/9d4db5cc-0987-4f7d-add2-fad6d63fa1ec" />
<br>
To prepare my design before coding, I downloaded the image I wanted to use, opened it in Microsoft Paint, and used the photo as a map. I added numbers to make coding easier, to help me quickly see what row/column I was on. I also drew lines through the drawing to map my progress in between college labs.

![ColourStripes](https://github.com/user-attachments/assets/855418de-6d3a-4b3a-a1bc-183ec4a4d18c)
![image10 (1)](https://github.com/user-attachments/assets/e5033b1c-976c-4a61-a163-c70e9d503cf4)

<br>
After the ColourStripes Lab, I began to alter my design. I initially started by setting the background default colour to be fully white. I then began inserting red pixels to get a feel for the sizing and placement that I would need to design my SpiderMan art.
<br><br>
I then initialised a row variable, to work with the column variable from the template code. I added more conditional statements for the RGB colours, I continued this to add small red, black and white pixels to build my Spider-Man mask.
<br><br>

![image2 (4)](https://github.com/user-attachments/assets/b037eaab-3058-43f7-b47b-897025d81f9a)

<br><br>
After being 1/4 of the way done, I realised that I had made a mistake on my sizing for the mask. The design was on course to have been far too big.
<br>

![image1 (3)](https://github.com/user-attachments/assets/529c8346-3b0b-4741-bf0c-e73573946273)
![image0 (4)](https://github.com/user-attachments/assets/d598893d-c93c-421e-b9e9-23e6d6e71286)

<br>
After correcting my incorrect sizing, I continued working hard to get the mask done, as you can see here.

### **Code Adaptation**
I altered the template code by using rows as well as columns to allow more freedom in coding coloured pixels, adding this to my code allowed me to have way more room to work with, allowing me to code vertically and horizontally across the monitor.
<br>
I then changed the template codes colour scheme by changing the binary colour code for each row and column. I chose my pixel sizing based off of the row and column it corresponded to in the code.
<br>
I changed the multiple striped colours to be a default colour of all white, by changing the RGB binary code to be 1111 (the code for white). Once I had my base colour, I began coding in pixels of 16 to create Spider-Man's mask in correlation to my reference photo.
<br>

### **Simulation**
Show how you simulated your own design. Are there any things to note? Demonstrate your understanding. Add a screenshot. Guideline: 1-2 short paragraphs.
### **Synthesis**
Describe the synthesis & implementation outputs for your design, are there any differences to that of the original design? Guideline 1-2 short paragraphs.
### **Demonstration**
After roughly 70 if elses and 530 lines of code... Here is my Finished Spider-Man Mask! 
<br>
![FinishedSoCproject](https://github.com/user-attachments/assets/63ed01cc-51e7-4d87-a93e-1feaec0ba89b)


### References
[1] Pixil Art, Spider-Man, Online, Available: [PixilArt](https://www.pixilart.com/art/spider-man-pixel-art-sr254518abb76aws3). 
