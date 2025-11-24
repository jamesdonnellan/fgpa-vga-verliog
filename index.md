---
layout: home
title: FPGA VGA Driver Project
tags: fpga vga verilog
categories: demo
---

Welcome to my FPGA VGA Pixel Art project, where Spider-Man's iconic mask comes to life! Using the Basys3 FGPA board, Verilog and digital logic, I adapted my pixel art design to replace the online image with my own recreation in 640x480.

## **Template VGA Design**
### **Project Set-Up**
Summarise the project set-up and design flow. Include a screenshot of your own set-up, for example see the image of my Project Summary window below. Guideline 1 short paragraph.

<img src="https://raw.githubusercontent.com/melgineer/fpga-vga-verilog/main/docs/assets/images/VGAPrjSum.png">
### **Template Code**
Outline the structure and design of the Verilog code templates you were given. What do they do? Include reference to how a VGA interface works. Guideline: 2/3 short paragraphs, consider including screenshot(s).
### **Simulation**
Explain the simulation process. Reference any important details, include a well-selected screenshot of the simulation. Guideline: 1/2 short paragraphs.
### **Synthesis**
Describe the synthesis and implementation processes. Consider including 1/2 useful screenshot(s). Guideline: 1/2 short paragraphs.
### **Demonstration** 
Perhaps add a picture of your demo. Guideline: 1/2 sentences.

## **My VGA Design **
Growing up as a Marvel fan, I wanted my project to be something that I have an interest in. So for my project I chose to create a pixel art of Spider-Man. I felt it would be a manageable design to achieve in the projects timeframe. For design reference, I chose a spiderman pixel art from [PixilArt](https://www.pixilart.com/art/spider-man-pixel-art-sr254518abb76aws3). 

![image10 (1)](https://github.com/user-attachments/assets/e5033b1c-976c-4a61-a163-c70e9d503cf4)

<br>
After the ColourStripes Lab, I began to alter my design. I initially started by setting the background default colour to be fully white. I then began inserting red pixels to get a feel for the sizing and placement that I would need to design my SpiderMan art.
<br>

![image2 (4)](https://github.com/user-attachments/assets/b037eaab-3058-43f7-b47b-897025d81f9a)

<br>
After being 1/4 of the way done, I realised that I had made a mistake on my sizing for the mask. The design was on course to have been far too big.
<br>

![image1 (3)](https://github.com/user-attachments/assets/529c8346-3b0b-4741-bf0c-e73573946273)
![image0 (4)](https://github.com/user-attachments/assets/d598893d-c93c-421e-b9e9-23e6d6e71286)

<br>
After correcting my incorrect sizing, I continued working hard to get the mask done, as you can see here.





### **Code Adaptation**
Briefly show how you changed the template code to display a different image. Demonstrate your understanding. Guideline: 1-2 short paragraphs.

I altered the template codes colour scheme by changing the binary colour code for each row and column. I chose my pixel sizing based off of the row and column it corresponded to in the code.

I changed the multiple striped colours to be a default colour of all white, by changing the RGB binary code to be 1111 (the code for white).

### **Simulation**
Show how you simulated your own design. Are there any things to note? Demonstrate your understanding. Add a screenshot. Guideline: 1-2 short paragraphs.
### **Synthesis**
Describe the synthesis & implementation outputs for your design, are there any differences to that of the original design? Guideline 1-2 short paragraphs.
### **Demonstration**
If you get your own design working on the Basys3 board, take a picture! Guideline: 1-2 sentences.
My Finished Spider-Man Mask! 
![FinishedSoCproject](https://github.com/user-attachments/assets/63ed01cc-51e7-4d87-a93e-1feaec0ba89b)


