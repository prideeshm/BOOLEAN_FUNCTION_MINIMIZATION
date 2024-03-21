## Name:Prideesh M
## Reg no:212223040154
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
module ex02(A,B,C,D,F1);
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
Developed by:Prideesh M RegisterNumber:212223040154


**RTL realization**
**RTL**
![Screenshot 2024-03-21 102113](https://github.com/prideeshm/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870483/26927343-2d06-47e8-ab86-e1a3df97ccf8)

**truth table**
![ex02 truth table](https://github.com/prideeshm/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870483/945b8acc-3e73-46f0-bf91-bc90ce3c3ddc)

**Timing Diagram**
![Screenshot 2024-03-21 080417](https://github.com/prideeshm/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870483/ae0c3ab8-aa65-4683-9d29-0e2c9da8267a)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

