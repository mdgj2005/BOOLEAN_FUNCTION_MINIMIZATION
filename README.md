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

Developed by:GOKUL ANAND M  RegisterNumber:212223040049*/
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

**RTL realization**

**Output:**
![Screenshot 2024-10-24 105436](https://github.com/user-attachments/assets/89cf43ff-eef1-4cbb-9ee8-1169b72a8a81)
![Screenshot 2024-10-24 105416](https://github.com/user-attachments/assets/d15a1429-be32-4091-9d46-2f041aec497d)

**RTL**
![Screenshot 2024-10-24 105446](https://github.com/user-attachments/assets/a425cddc-89d3-46da-b811-c44aee8d1fa0)
![Screenshot 2024-10-24 105455](https://github.com/user-attachments/assets/df44f6c7-19b5-44e5-9f41-2253581d1270)

**Timing Diagram**
![Screenshot 2024-10-24 105501](https://github.com/user-attachments/assets/ab8c4aaa-3d76-458a-abe1-e620526c8202)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

