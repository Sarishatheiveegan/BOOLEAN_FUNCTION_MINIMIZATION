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
Developed by:Marino Sarisha T   RegisterNumber:212223240084*/


**RTL realization**
![Screenshot 2024-03-15 111111](https://github.com/Sarishatheiveegan/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979465/8852166c-c1aa-45e4-8c05-6fdcdac0b49f)

**Output:**
**TruthTable:**
![Screenshot 2024-03-15 111622](https://github.com/Sarishatheiveegan/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979465/45f181b0-15a9-4315-94be-d4d22d916a01)


**Timing Diagram**
![Screenshot 2024-03-15 111309](https://github.com/Sarishatheiveegan/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979465/aff35fce-8517-4fff-84b7-69c9bc4304f6)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

