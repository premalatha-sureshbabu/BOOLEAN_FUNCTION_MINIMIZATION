# EX NO:2 BOOLEAN_FUNCTION_MINIMIZATION

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

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: S.Prema Latha
RegisterNumber:212222230112
```
module exp22(A,B,C,D,F1);
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

**RTL realization**

![image](https://github.com/premalatha-sureshbabu/BOOLEAN_FUNCTION_MINIMIZATION/assets/120620842/18e26de1-dd14-4e34-b53b-182044799816)

**Truth Table**

![image](https://github.com/premalatha-sureshbabu/BOOLEAN_FUNCTION_MINIMIZATION/assets/120620842/a903ec9e-14cc-4fef-8203-65a27c73363a)

**Timing Diagram**

![image](https://github.com/premalatha-sureshbabu/BOOLEAN_FUNCTION_MINIMIZATION/assets/120620842/d164c2e5-0745-4078-8d18-8ea7feb94647)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

