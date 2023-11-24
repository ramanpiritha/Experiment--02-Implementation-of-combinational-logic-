# Experiment--02-Implementation-of-combinational-logic
Name: Piritharaman R
Ref no: 23013537
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
module exp_2(A,B,C,D,F1);
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
## RTL realization:
![image](https://github.com/ramanpiritha/Experiment--02-Implementation-of-combinational-logic-/assets/147084116/cfdce6e1-9b10-4bf0-840b-69a8589ec30b)
##Truth Table:
![image](https://github.com/ramanpiritha/Experiment--02-Implementation-of-combinational-logic-/assets/147084116/2adbc69c-7b8f-43d6-a0d2-bf6932f0bf5b)


## Output:
## RTL
## Timing Diagram
## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
