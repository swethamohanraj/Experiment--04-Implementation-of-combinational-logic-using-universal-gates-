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
![nandtr](https://user-images.githubusercontent.com/94228215/167343748-160ff6b2-64c5-4e7e-be7f-2efd2e736769.png)

### RTL Realisation 
![nandrtl](https://user-images.githubusercontent.com/94228215/167343759-a8002f39-aa05-4336-accf-133fadf7ff79.png)

### Timing diagram
![nandtim](https://user-images.githubusercontent.com/94228215/167343771-b580e858-5b86-4a4d-bdf3-5cacc355dcc0.jpeg)


### NOR GATE
### Truth Table
![nortr](https://user-images.githubusercontent.com/94228215/167343785-fb055c75-f486-4aee-8ece-2712dd57b5d2.png)

### RTL Realisation 
![norlg](https://user-images.githubusercontent.com/94228215/167343797-3b429f21-f5ad-4200-ace4-b3ba3a49113f.png)

### Timing diagram
![nortim](https://user-images.githubusercontent.com/94228215/167343809-29bb1f7b-eca4-475e-a818-5388f7d6f428.png)



## Result:
Thus given logics are implemented using NAND and NOR gates and is verified in Quartus using Verilog programming.
