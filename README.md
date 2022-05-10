# Experiment--04-Implementation-of-combinational-logic-using-universal-gates-
 ## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To implement the given logic function using NAND and NOR gates and to verify its operation in Quartus using Verilog programming.
F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate
F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' using NOR gate


## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory

A universal gate is a logic gate which can implement any Boolean function without the need to use any other type of logic gate. The NOR gate and NAND gate are universal gates. This means that you can create any logical Boolean expression using only NOR gates or only NAND gates. In practice, this is advantageous since NOR and NAND gates are economical and easier to fabricate than other logic gates. Similarly, an OR gate is typically realised as a NOR gate followed by an inverter.
 
 
 
 


## Procedure

1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.



Write the detailed procedure here 


## Program:
/*
Program to design a Implementation of combinational logic using universal gates-  and verify its truth table in quartus using Verilog programming.
Developed by: RAHUL N
RegisterNumber:  212220053010

NAND GATE PROGRAM

module un1(a,b,c,d,f);
input a,b,c,d;
output f;
assign  f=(((~c&b&a))&((d&c&a))&((c&(~b)&a)));
endmodule

NOR GATE PROGRAM

module nor1(a,b,c,d,f);
input a,b,c,d;
output f;
assign  f=((((c&(~b)&a)|(d&(~c)&a)|(c&(~b)&a))));
endmodule
*/

## Output:

## Truthtable

NAND GATE TT
![NAND GATE TT](https://user-images.githubusercontent.com/103518963/167664605-9f8e89cc-55bf-48a6-8d93-b393712d1c3c.jpeg)

NOR GATE TT
![NOR GGATE TT](https://user-images.githubusercontent.com/103518963/167664646-2ec86e84-dd6e-44ee-9e9c-89e148284917.jpeg)


##  RTL realization

NAND GATE 
![nandgate](https://user-images.githubusercontent.com/103518963/167663069-8d8a820b-4fde-4ba3-a253-3fc49a99ac31.png)

NOR GATE 
![norgate](https://user-images.githubusercontent.com/103518963/167663162-6d1fe121-c262-4d43-b2be-05213498d5ae.png)



## Timing diagram 

NAND GATE WF
![nandgate wf](https://user-images.githubusercontent.com/103518963/167664807-c5bdaff2-019b-4976-8a0f-fb4dca5f72a6.png)

NOR GATE WF
![norgate wf](https://user-images.githubusercontent.com/103518963/167664859-1c6c832c-a980-4cf9-9c9c-2c1b827fc54a.png)


## Result:
 
The given logic functions is implemented using NAND and NOR gates and it is verified successfully in quartus using verilog programming
