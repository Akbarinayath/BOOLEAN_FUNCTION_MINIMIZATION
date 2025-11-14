# BOOLEAN_FUNCTION_MINIMIZATION

**DATE:** 14.11.2025

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

**Program to implement the given logic function and to verify its operations in quartus using Verilog programming.** 

 **Developed by:ROHIT G**
 
 **RegisterNumber:212222240083**

```

module exp2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)| (~a&b&d)| (a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule 
```

**RTL realization**

<img width="512" height="410" alt="502658188-027a0976-886a-4274-ba9a-3fa0cafb0ea8" src="https://github.com/user-attachments/assets/b905452b-b995-4d0f-af60-7cbdea39cd69" />



**RTL**

<img width="1005" height="586" alt="502658989-b1ed9be3-6475-40ed-bb82-890855579dbd" src="https://github.com/user-attachments/assets/84019e50-81fe-4e4e-b6ed-88fc8445806f" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


