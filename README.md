# Experiment--04-Implementation-of-combinational-logic-using-universal-gates-
 ## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To implement the given logic function using NAND and NOR gates and to verify its operation in Quartus using Verilog programming.
F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate
F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' using NOR gate


## EQUIPMENTS REQUIRED:
### 1.Hardware – PCs, Cyclone II , USB flasher
### 2.Software – Quartus prime
### 3.Theory

## PROCEDURE
### 1.Use module projname(input,output) to start the Verilog programmming.
### 2.Assign inputs and outputs using the word input and output respectively.
### 3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.
### 4.Represent the output according to the given boolean expression(Using either NAND or NOR gate)
### 5.End the verilog program using keyword endmodule.

## PROGRAM:

Program to design a Implementation of combinational logic using universal gates-  and verify its truth table in quartus using Verilog programming.
```
Developed by: K.M.SWETHA
RegisterNumber: 212221240055
```
### IMPLEMENT THE LOGIC USING NAND GATE:
```
module combination(A,B,C,D,F);
input A,B,C,D;
output F;
wire P,Q,R;
assign P = C&(~B)&(~A);
assign Q = D&(~c)&(~A);
assign R = (~C)&B&(~A);
assign F = (~p&~Q&~R);
end module
```
### IMPLEMENT THE LOGIC USING NOR GATE
```
module ex4(A,B,C,D,F);
input A,B,C,D;
output F;
wire P,Q,R,S;
assign P=(C&~B&A);
assign R=(C&~B&A);
assign Q=(D&~C&A);
assign S=~(P|Q|R);
not(F,S);
endmodule
```


## OUTPUT:
### NAND GATE
### Truth Table
### RTL Realisation 
### Timing diagram

### NOR GATE
### Truth Table
### RTL Realisation 
### Timing diagram


## Result:
Thus given logics are implemented using NAND and NOR gates and is verified in Quartus using Verilog programming.
