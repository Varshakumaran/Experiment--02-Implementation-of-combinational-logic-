NAME: varsha.k

referrence: 23005952

# Experiment 02 Implementation of combinational logic

 
# AIM:
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
```
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
```
## RTL realization
![image](https://github.com/Varshakumaran/Experiment--02-Implementation-of-combinational-logic-/assets/144979367/7953200f-85a6-4f48-bf98-a1ae34421676)
# TRUTH TABLE:
![image](https://github.com/Varshakumaran/Experiment--02-Implementation-of-combinational-logic-/assets/144979367/c05fb4a4-31cf-461c-8ae4-0d663f693278)

# Timing Diagram:
![image](https://github.com/Varshakumaran/Experiment--02-Implementation-of-combinational-logic-/assets/144979367/dbf26781-bf2e-4b68-82a1-903f2e7c9797)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
