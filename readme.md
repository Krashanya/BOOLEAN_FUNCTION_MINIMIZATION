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
```
module exp_2(A,B,C,D,W,X,Y,Z,F1,F2);
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
```
Developed by: KRASHANYA G
RegisterNumber: 212225230144
```

**Truth table for F1:**

<img width="557" height="851" alt="image" src="https://github.com/user-attachments/assets/f4c3be23-765b-472b-8088-23f680697737" />

**Truth table for F2:**

<img width="560" height="852" alt="image" src="https://github.com/user-attachments/assets/6274372d-3361-4798-844d-24cda18077be" />

**Output:**

<img width="532" height="787" alt="image" src="https://github.com/user-attachments/assets/1239d9a0-11c9-4e7f-a55a-90742c10ebb4" />

**Timing Diagram**

<img width="1600" height="345" alt="image" src="https://github.com/user-attachments/assets/725f3348-c050-4cb0-8da8-ed4735640337" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

