Journal #1 : Making the Case!
by@aryansalvehub

Total Time Spent : 2Hrs 32min

By@aryansalvehub

Starting the project, the plan was to make the case! For this hackpad, I am designing the case in two part, 1st part is to make upper body of the case and the other was to make the bottom of the case, the bottom case was a box with hollow space for the PCB and the space for USB connection of hackpad to the device. 
<img width="1290" height="594" alt="image" src="https://github.com/user-attachments/assets/58642bb3-4ad7-4294-8ebd-4b64fd7c530f" />


For the 2nd Part I made a simple plate with gap for the keys the OLED panel and for the rotating dial too. The design was too added in the 2nd part and Extended to part 1 an idea to add some more hand holding design with more than a box like some thing different from just box.
<img width="1174" height="592" alt="image" src="https://github.com/user-attachments/assets/1989d649-e28f-4f58-baab-478af3f5f822" />




Journal #2 by @Mwezi2000
Total time - 1 hr 10 min 

I started by placing the Seeeduino XIAO (U1) on the right side of the sheet. I put the 12 switches (SW1–SW12) in a 3×4 grid on the left, each with its own 1N4148 diode (D1–D12).
I wired the keys as a matrix instead of giving every key its own pin. A matrix uses far fewer GPIOs, and the XIAO doesn't have many. The wiring works like this:
* Each of the 4 columns is a vertical wire connecting the left side of the 3 switches in that column. Those wires go to XIAO pins D0–D3.
* Each of the 3 rows is a horizontal wire connecting the diode cathodes across that row, and it goes to its own pin on the XIAO.
* Every switch has a diode in series, so pressing several keys at once doesn't cause ghosting.
Next I added the rotary encoder (SW13). Its A and B pins go to two GPIO pins, the common pin C goes to GND, and I labelled the GND connection with a power symbol.
Last I added J1, a 4-pin header with GND, +5V, and two signal lines going to the XIAO's SDA and SCL pins. This lets me plug in an I2C device such as an OLED display. I also connected the XIAO's 5V and GND pins to the +5V and GND power symbols.
￼<img width="1462" height="856" alt="image" src="https://github.com/user-attachments/assets/55bdd728-6507-4746-ae08-a1942253cbd9" />

  Final schematics -  	•	U1 — MOUDLE-SEEEDUINO-XIAO (14-pin module)
* 12x SW_Push (SW1-SW12) in a 3-row x 4-column matrix, each with a 1N4148 diode
* SW13 — RotaryEncoder_Switch (SCROLL1), wired to A/B/GND/S1/S2
* J1 — Conn_01x04_Pin, breaking out GND / +5V / OLED_SDA / OLED_SCL for the OLED panel
* Row1-3 and Col1-4 nets routed across the matrix; SDA/SCL shared between the OLED connector and controller

Journal #3 by @aryansalve041
Total Time - 2hrs 32 min(case modification) + 3 hrs (art design)

I felt something off at the case deign and some structural errors so i gave some of my time to fix the structurals errors and the other thing was make it more live,
so i added some wavy feels rather than keepig it like simple box and i too added some of boundary for rotatory switch so that themiddle part which was first visibble to viewwer now could hide so that it would feel kind of stylish rather keeping it like a mechanical feels. I too removed unneccasary part space taking to fit the PCB more precisely. i also added the boundary to the OLED  Screen so that the side part is less visible and the screens feels more wide.
<img width="1174" height="592" alt="image" src="https://github.com/user-attachments/assets/c77f3925-659d-46da-afb2-e7d19eceeef5" />


Now moving toward some styling part of case and PCB sso that it would feel more real and could see it as a mark.
This was my first time using Krita, so I spent some time getting familiar with the different tools and the interface. I started by trying out the brush, eraser, colours, layers and basic shapes. I then started making the artwork for my on-board design. Since I was using a mouse, making smooth lines and small details was a bit difficult, and I had to use undo and eraser quite often. I also experimented with different brush sizes and layers to make the design look better.
In the last part, I cleaned up the unwanted lines, adjusted some details and made a few changes to the colours and overall look. Overall, it took me around 2.5–3 hours, and I got more comfortable with Krita while making the artwork.
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/512d293c-c53e-48d2-80c4-99e33588ea38" />
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/fe3aad66-a881-4a6f-8e81-9c824acb4c9d" />



journal #4
By @Mwezi2000

Total time - 1hr 46 mins (pcb editor part 1) + 51 mins (art) + 3hrs 41 mins ( art again ) = 6hrs 18 mins  so after completing my schematics for pcb I wen off to the kicad pcb editor
It was my first time using it, which was really fun! (I got stuck at making that grid for keys and did it manually at last-) I also did some changes on the pcb scheme, checked all the footprints then imported on pcb editor
Then it was just arranging these components on their places which looked very congested at first
But at last I was sure it would turn out really beautiful ! I was bored of pcb editor so I started making some art for my pcb 

<img width="1176" height="725" alt="image" src="https://github.com/user-attachments/assets/c2b95bba-e370-4150-9db0-568ef8163615" />
￼
 Again this was my first time using krita (didnt expect it would go so well) I started making all the things I could think of also I tried to keep it related to our theme Harvest!

 <img width="1182" height="713" alt="image" src="https://github.com/user-attachments/assets/9248f9ed-4e19-461e-96f7-3e0b21d02680" />

￼
 So the first one was trial but I decided to keep it, the next two turned out to be good 
I went for a break then but came back to draw some of my coolest stickersssss (still can’t believe, krita was so fun!)


 <img width="1183" height="749" alt="image" src="https://github.com/user-attachments/assets/962de613-c2e6-45b2-922f-2b6f23969db5" />

￼
 This took me a whole bunch of time but turned out real beauty
I loved it so much that I just forgot about the pcb, and went on drawing! Every cool thing I could think of, I seriously couldn’t stop myself 
I thought to write out team logo and then I also made our friendly neighbour spidermans logo! 
￼

<img width="1179" height="743" alt="image" src="https://github.com/user-attachments/assets/bb920af7-0b94-4bd6-887e-ec7741180a43" />


Finally back to completing the pcb! 


