Journal #1 : Making the Case!
by@aryansalvehub

Total Time Spent : 2Hrs 32min

By@aryansalvehub

Starting the project, the plan was to make the case! For this hackpad, I am designing the case in two part, 1st part is to make upper body of the case and the other was to make the bottom of the case, the bottom case was a box with hollow space for the PCB and the space for USB connection of hackpad to the device. 
<img width="1290" height="594" alt="image" src="https://github.com/user-attachments/assets/58642bb3-4ad7-4294-8ebd-4b64fd7c530f" />


For the 2nd Part I made a simple plate with gap for the keys the OLED panel and for the rotating dial too. The design was too added in the 2nd part and Extended to part 1 an idea to add some more hand holding design with more than a box like some thing different from just box.
![Uploading image.png…]()



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

