## Name:Prideesh M
## Reg no:212223040154
# BOOLEAN_FUNCTION_MINIMIZATION

## AIM:

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


## Program:

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module Boolean_min(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);

and g1(s,ydash,z);
and g2(t,x,y);
and g3(u,w,z);
or g4(f2,s,t,u);
endmodule
```
Developed by:Prideesh M RegisterNumber:212223040154


## RTL realization

![Screenshot 2024-03-23 200335](https://github.com/prideeshm/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870483/f352081d-c087-4f9e-bfbc-1f9953f905cf)



## truth table

![ex02 truth table](https://github.com/prideeshm/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870483/9b8ac838-42f6-4e16-af60-36b3d664d4db)



## Timing Diagram
![Screenshot 2024-04-05 144731](https://github.com/prideeshm/BOOLEAN_FUNCTION_MINIMIZATION/assets/144870483/b09b3c71-f010-4f7b-b776-a0998ac476cd)


## Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

