# BOOLEAN_FUNCTION_MINIMIZATION

## AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

## Equipment Required:
Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

## Theory:
Theory A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.

## Procedure:

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:
```
 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: SUDHARSANA KUMAR S R
RegisterNumber: 212223240162
module combinationalcircuit(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```

## RTL realization:
![image](https://github.com/sudharsanakumar18/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849110/14048d72-126a-43a7-aacd-7aa153d9752e)

## RTL realization:
![image](https://github.com/sudharsanakumar18/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849110/9a677ac8-42c9-4ddb-b484-fc75b252cdb3)

## RTL:
![image](https://github.com/sudharsanakumar18/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849110/0db17570-e390-47bf-8aef-9c4c6556442a)

## Timing Diagram:
![image](https://github.com/sudharsanakumar18/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849110/91a487ba-d0ec-4696-b80f-8c31ae4e597d)

## Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

