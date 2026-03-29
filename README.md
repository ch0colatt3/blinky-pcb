# blinky-pcb
![pcb heel 3d view](images/kicad_3Dview.png)
## Components

- x16+ Red LEDs
- x1 555 Timer IC
- x1 10 μF Capacitor
- x1 100k Variable Resistor
- x1 10k Resistor
- x1 330 ohm resistor
- x1 1 Push Button
- x1 9V Battery Holder Clip

## Description
This project is a hardware design of a 555 led chaser/blinky board. I made this double-layered pcb project following stasis’ & Athena’s Sleepover starter project. The software I used in the process is KiCad.


Process:
1. Use Kicad schematic editor to insert components /* idk if I used the right 55 timer IC */
2. Assign footprints to each component
3. Wire diagram 
4. Run electrical rules check(ERC) to fix any errors 
5. Export schematic to pcb editor
6. Import a dxf file of the image I want as my edge cut onto edge.cut layer(heel) /* this step took me hours, I downloaded Inkscape for this & tried to create a shape myself when the problem was that I forgot to put in on the correct layer, -I also had to adjust the shape of the heel to make sure if fitted the schematic(measurements, ratio) after I ran DRC :((  */
7. Arranged components inside heel shape
8. Route everything following highlighted blue lines on F.Cu or B.Cu(backside-if not enough space)
9. Run design rule check(DRC) to fix any errors (for me: unconnected wires, SILKSCREEN ISSUES) 
10. Use the text function and add design to board (I typed symbols & words) /*this step took me a few hours -rotating, making sure the text didn’t cause any errors or warnings */
11. Run DRC again 
12. Yippee! 

