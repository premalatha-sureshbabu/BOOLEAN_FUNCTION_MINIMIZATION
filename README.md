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
module boolean_fun(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u,v,w1,w2,x1,x2,y1,y2,z1,z2;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);

and(w1,a,b,c);
and(w2,~a,~b,~c);
or(f2,w1,w2);
endmodule
```

**RTL realization**

![image](https://github.com/premalatha-sureshbabu/BOOLEAN_FUNCTION_MINIMIZATION/assets/120620842/d9caeef3-7cf1-4829-9a43-ef11c0b114b4)


![image](https://github.com/premalatha-sureshbabu/BOOLEAN_FUNCTION_MINIMIZATION/assets/120620842/ad77cb23-80b4-4d53-9d96-63e9fcd280d9)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

