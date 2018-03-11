						SG3114: 2BIT UNIVERSAL & EXCLUSIVE GATE WITH INOUT BUFFER

This project was implemented on LTSpice by using modules such as SRAM, 2 to 4 Decoder, NAND, NOR, XOR, XNOR, 4 input OR gate and so on. The final schematic has all these modules combined togeter to test all possible cases with 2 select lines(s1, s2) and 2 inputs(ip1, ip2). This can be observed in the final waveform generation. SRAM module was designed with read and write stability requirements by making pull up transistor(PMOS) weak, Driver transistor(NMOS) strong and access transistor(NMOS) moderately strong with the help of Layout and Simulation of a 6T SRAM Cell by Mat Binggeli found at https://www.researchgate.net/file.PostFileLoader.html?id=58513794615e27ef35444935&assetKey=AS%3A439169819385856%401481717652133.

Select lines and the respective gates that are active

00 -> NAND, 01 -> NOR, 10 -> XOR, 11 -> XNOR

Installation and Usage
The .rar file contails all the needed schematics and their schematics needed to execute the above said project on LTSpice.
LTSpice can be found on http://www.linear.com/designtools/software/  ,Use this link to download the latest version of LTSpice and install it.

Steps to use the project
1. Extract sandesh_guru.rar into a folder of your choice, make sure to open LTSpice in Admistrator mode if files are in C Drive.
2. Goto File -> Open, Navigate to the folder where you extracted the project to and open microcontroller.sch
3. Click on Simulate -> RUN, to run with the given values run as is else change values of s1, s2, ip1, ip2 in schematic.
   To change simulation time, use 'Change simulation Cmd' found under Simulate and enter the desired simulation time.
4. IN the simulation window right click and select add plot pane to add an empty plot plane.
5. Right click on the desired plot plane and right click to select 'add trace' to add the desired waveform.
6. Observe if the waveforms match the said output give above.  

A Symbol for the same is created called SG3114 for implementation in different projects.
