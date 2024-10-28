# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:DURGA V
RegisterNumber:212223230052
*/
```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);

input A,B,C,D,W,X,Y,Z;

wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;

output F1,F2;

assign x1=(~A)&(~B)&(~C)&(~D);

assign x2=(A)&(~C)&(~D);

assign x3=(~B)&(C)&(~D);

assign x4=(~A)&(B)&(C)&(D);

assign x5=(B)&(~C)&(D);

assign x6=(X)&(~Y)&(Z);

assign x7=(~X)&(~Y)&(Z);

assign x8=(~W)&(X)&(Y);

assign x9=(W)&(~X)&(Y);

assign x10=(W)&(X)&(Y);

assign F1=x1|x2|x3|x4|x5;

assign F2=x6|x7|x8|x9|x10;

endmodule
```


**RTL realization**

![image](https://github.com/user-attachments/assets/60a4ab28-928a-4d7f-8035-bf2e796c2add)

## LOGIC SYMBOL & Truthtable:
## TRUTH TABLE FOR F1:
![image](https://github.com/user-attachments/assets/e67ec38e-b2b5-4d3e-ae6f-fb72e68c3deb)

## TRUTH TABLE FOR F2:
![image](https://github.com/user-attachments/assets/8dbb690d-ac5a-42dd-8223-5d2506944d4f)

## Timing Diagram :
![image](https://github.com/user-attachments/assets/50a187d8-1971-487a-b826-3f3d8e2d70db)

## Result:
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

