# 12-key macropad 

#what is it?
this is a custom 12-key mechanical macropad i designed in kicad from scratch. it runs on a seeed studio xiao rp2040 board instead of a bulky standard dev board, which keeps the whole thing compact and cheap. it has a 4x3 switch matrix with anti-ghosting diodes, a clickable rotary encoder knob, and a 4-pin header on top for a small i2c oled display.

# why make this?
i use a 60% keyboard daily, and while it looks clean and saves desk space, losing dedicated arrow keys, media buttons, and numpad shortcuts is honestly a pain. memorizing three-key layer combos while working or gaming gets frustrating fast. 

i wanted a standalone pad with dedicated hardware buttons for stuff like discord mutes, copy-pasting, app switching, and terminal shortcuts. plus, having a physical rotary dial to control volume or scrub timelines is way more satisfying than pressing function keys.

#how does it work?
- the key matrix:* the 12 switches are wired in a 4-column by 3-row grid connected directly to the xiao gpio pins. the micro-controller quickly scans through the rows and columns to check if a circuit is closed
- diodes* each switch has its own 1n4148 diode wired in series[cite: 3]. this stops back-powering across rows so you can press multiple keys at the same time without triggering phantom ghost clicks.
- rotary encoder:* the ec11 encoder pulses signals across two data pins whenever you turn it, letting the code figure out both direction and speed for scrolling or volume adjustments. the center shaft also clicks straight down, working as a 13th input switch
- oled screen:* hooked up to 5v, ground, sda, and scl pins. it talks over the i2c bus to show what profile or layer you are on, or display real-time stats like click counters.

#hardware & pcb specs
- controller:* seeed studio xiao rp2040
- keys:* 12 push switches arranged with standard 19.05 mm (1u) spacing so normal mechanical keycaps fit properly
- diodes:* 12x 1n4148 through-hole diodes placed next to each switch
- encoder:* ec11 rotary encoder with integrated push switch
- display connector:* 4-pin 2.54mm header for 0.96" i2c oled
- board size:*85.91 mm x 84.00 mm (2-layer pcb)
