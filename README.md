********************************************************************************************************************************************************************************************
						SG3114: 2BIT UNIVERSAL & EXCLUSIVE GATE WITH INOUT BUFFER
********************************************************************************************************************************************************************************************

This project was implemented on LTSpice as a part of Digital Integrated Circuit design course taken up for Spring 2018 Term under the guidance of Dr. Gayatri Mehta. 
The project implementationwas performed by using modules such as SRAM, 2 to 4 Decoder, NAND, NOR, XOR, XNOR, 4 input OR gate and so on. The final schematic has all
these modules combined togeter to test all possible cases with 2 select lines(s1, s2) and 2 inputs(ip1, ip2). This can be observed in the final waveform generation.
SRAM module was designed with read and write stability requirements by making pull up transistor(PMOS) weak, Driver transistor(NMOS) strong and access 
transistor(NMOS) moderately strong with the help of Layout and Simulation of a 6T SRAM Cell by Mat Binggeli found at 
https://www.researchgate.net/file.PostFileLoader.html?id=58513794615e27ef35444935&assetKey=AS%3A439169819385856%401481717652133.


Select lines, input and the respective gates and their outputs are as shown below
-------------------------------------------------------
s1	s2	GATE ACTIVE	IP1	IP2	OUTPUT
-------------------------------------------------------
0	0	NAND		0	0	1
				0	1	1
				1	0	1	
				1	1	0	

0	1	NOR		0	0	1
				0	1	0
				1	0	0
				1	1	0	

1	0	XOR		0	0	0
				0	1	1
				1	0	1	
				1	1	0

1	1	XNOR		0	0	1
				0	1	0
				1	0	0
				1	1	1


Installation and Usage
The .rar file contails all the needed schematics and their schematics needed to execute the above said project on LTSpice.
LTSpice can be found on http://www.linear.com/designtools/software/  ,Use this link to download the latest version of LTSpice and install it.

Steps use the project
1. Extract sandesh_guru.rar into a folder of your choice, make sure to open LTSpice in Admistrator mode if files are in C Drive.
2. Goto File -> Open, Navigate to the folder where you extracted the project to and open microcontroller.sch
3. Click on Simulate -> RUN, to run with the given values run as is else change values of s1, s2, ip1, ip2 in schematic.
   To change simulation time, use 'Change simulation Cmd' found under Simulate and enter the desired simulation time.
4. IN the simulation window right click and select add plot pane to add an empty plot plane.
5. Right click on the desired plot plane and right click to select 'add trace' to add the desired waveform.
6. Observe if the waveforms match the said output give above.  

A Symbol for the same is created called SG3114 for implementation in different projects. 

Contribution
The project was done by a team of 2 students and their contribution is as given below
---------------------------------------------------------------------------------
NAME						CONTRIBUTION 
---------------------------------------------------------------------------------
SANDESH HULIKAL SOMASHEKHAR			SRAM module
						NAND gate
						XNOR gate
						Combining individual modules
								
GURU PRASANNA SRINIVASAN			2 to 4 Decoder
						NOR gate
						XOR gate
						4 input OR gate
