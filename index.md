---
layout: home
title: FPGA VGA Driver Project
tags: fpga vga verilog
categories: demo
---
  
Welcome to my FPGA VGA Pixel Art project, where Spider-Man's iconic mask comes to life! Using the Basys3 FGPA board, Verilog and digital logic, I adapted my pixel art design to replace the online image with my own recreation on a 640x480 VGA display.

**Basys3 FGPA Board & Reference Photo:** <br>                                        
<img width="318" height="241" alt="SoC Board" src="https://github.com/user-attachments/assets/0c4c5c96-72e9-41f9-8824-b097643990c5" /> 
<img width="318" height="241" alt="UpdatedSpiderManMask" src="https://github.com/user-attachments/assets/3426797c-ce80-43e7-b600-728c357a7821" />
<br> 

## **Spider-Man's Mask VGA Design**
### **Project Set-Up**
I used Vivado and a Basys3 FGPA Board to create my Spider-Man mask. I started by creating a new project, adding my template code files used in previous Labs [1], and then altered and added to them to create my design. 
The previous labs guided me through the set up process using Vivado and the Basys3 board. I follow the set up protocal of build, synthesise, implement and then progamming the board.

<img width="2250" height="900" alt="Project Summary Photo" src="https://github.com/user-attachments/assets/0623e279-75fb-4346-8504-38662d82fad0" />
<br>
(Project Summary Window of my VGA Project Setup)

### **What Did The Template Code Do?**
The template code generates vertical colour bands on a VGA output. It took the column from the VGA timing module and used it to decide what colour each pixel should display. Then, using the RGB combination through 'if else' conditional statements, the colours got selected and displayed into 8 equal stripes.

### **Simulation Process**
To start off my project, I simulated the template code using Vivado to ensure that everything was working, and that no code was broken. Once I ensured that the VGA timing module checked correct behavior, I began coding my own design based off of the template code. This step was essential in my project as before making any first steps, I needed to ensure that timing was perfect, to avoid any breakages in the VGA output.

### **Synthesis**
After I completed my initial simulation, Vivado performed Synthesis to map the design onto the Basys3 FGPA board. Then, it produced reports detailing resource usage, timing information and a hardware diagram on how the design would fit onto the chip. The original design didn't have much comparison logic, so the hardware design was more simple than my final design.

### **Demonstration** 
After setting up my project properly, here was my first steps to designing my Spider-Man Mask!
<br>
![image10 (1)](https://github.com/user-attachments/assets/e5033b1c-976c-4a61-a163-c70e9d503cf4)

## **My VGA Design - Spider-Man's Mask**
Growing up as a Marvel fan, I wanted my project to be something that I have an interest in. So for my project I chose to create a pixel art of Spider-Man. I felt it would be a manageable design to achieve in the projects timeframe. For design reference, I chose a spiderman pixel art from [PixilArt](https://www.pixilart.com/art/spider-man-pixel-art-sr254518abb76aws3). [2]
<br><br>
<img width="318" height="241" alt="image" src="https://github.com/user-attachments/assets/9d4db5cc-0987-4f7d-add2-fad6d63fa1ec" />
<br>
To prepare my design before coding, I downloaded the image I wanted to use, opened it in Microsoft Paint, and used the photo as a map. I added numbers to make coding easier, to help me quickly see what row/column I was on. I also drew lines through the drawing to map my progress in between college labs.


### **Code Adaptation**
I altered the template code by using rows as well as columns to allow more freedom in coding coloured pixels, adding this to my code allowed me to have way more room to work with, allowing me to code vertically and horizontally across the monitor.
<br>
I then changed the template codes colour scheme by changing the binary colour code for each row and column. I chose my pixel sizing based off of the row and column it corresponded to in the code.
<br>
<br>
After the ColourStripes Lab, I began to alter my design. I initially started by setting the background default colour to be fully white, by changing the RGB binary code to be 1111 (the code for white). I then began inserting red pixels, to get a feel for the sizing and placement that I would need to design my SpiderMan art.
<br><br>
I then initialised a row variable, to work with the column variable from the template code. I added more conditional statements for the RGB colours, I continued this to add small red, black and white pixels to build my Spider-Man mask.
<br>
![ColourStripes](https://github.com/user-attachments/assets/855418de-6d3a-4b3a-a1bc-183ec4a4d18c)
![image10 (1)](https://github.com/user-attachments/assets/e5033b1c-976c-4a61-a163-c70e9d503cf4)
<br>

<br>
After being 1/4 of the way done, I realised that I had made a mistake on my sizing for the mask. The design was on course to have been far too big.
I then calculated the correct pixel sizing that I would need to ensure my design fit on the screen. After correcting my incorrect sizing, I continued working hard to get the mask done, as you can see here.
<br><br>

![image2 (4)](https://github.com/user-attachments/assets/b037eaab-3058-43f7-b47b-897025d81f9a)
![image1 (3)](https://github.com/user-attachments/assets/529c8346-3b0b-4741-bf0c-e73573946273)
![image0 (4)](https://github.com/user-attachments/assets/d598893d-c93c-421e-b9e9-23e6d6e71286)
<br>


### **My Simulation & Synthesis Process**
Before programming the Basys3 board, the VGA system is checked through Vivado simulation by using the testbench. I was able to watch how signals such as hsync, vsync, pixel position counters such as row and col, and the RGB values change over time in waveforms. This simulation allowed me to ensure that the VGA timing pattern was correct.
<br>

<img width="1500" height="750" alt="image" src="https://github.com/user-attachments/assets/642dff3a-2295-46a4-8f5b-c3f8557147ee" />
<img width="1500" height="750" alt="image" src="https://github.com/user-attachments/assets/5fc6de25-3dcd-4b2d-a681-fc64b65dc0af" />
<img width="1500" height="750" alt="image" src="https://github.com/user-attachments/assets/7d382617-b611-4d9d-8918-ffb51e59b0b3" />

After the simulation process, Vivado carried out the synthesis, which converted my VGA pixel-art design from code into a hardware circuit that I used to run on the Basys3 FGPA. During this step, Vivado determined how the modules in my project, such as the VGA timing module and pixel colour logic are implemented using actual FGPA resources like flip-flops, LUTs and I/O buffers. [3]
<br>
The photo of my circuit above shows how different parts of my code are mapped to physical hardware components that drive the VGA output and display the pixel art on the monitor.
<br>
### **Demonstration**
After roughly 70 if elses and 530 lines of code... Here is my Finished Spider-Man Mask! 
<br>
![FinishedSoCproject](https://github.com/user-attachments/assets/63ed01cc-51e7-4d87-a93e-1feaec0ba89b)


### References
[1] M.Lynch, "System On Chip", Lecture/Lab, ATU, Galway, 2025
<br>
[2] Pixil Art, "Spider-Man", [Online], Available: [PixilArt](https://www.pixilart.com/art/spider-man-pixel-art-sr254518abb76aws3). 
<br>
[3] ChatGPT, For a deeper understanding on Simulation and Synthesis, [Online], Available: [ChatGPT](https://chatgpt.com)



