# BOOLEAN_FUNCTION_MINIMIZATION

*AIM:*

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

*Equipment Required:*

Hardware – PCs, Cyclone II , USB flasher

*Software – Quartus prime*

*Theory*
![WhatsApp Image 2025-03-26 at 13 57 23_413f3334](https://github.com/user-attachments/assets/e95b143e-8dca-4431-9f51-7585f5e1c0b0)
*Procedure*

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:

*Program to implement the given logic function and to verify its operations in quartus using Verilog programming*. 

*Developed by: 212224230014 AKBAR.I:*
vhdl
```
module ex2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule
```

vhdl
```
module ex2_2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2= ((~y&z)|(w&z)|(x&y)|(w&y&~z));
endmodule
```

*RTL realization*
# 1-a)
![ex2](https://github.com/user-attachments/assets/649cc145-ba52-4298-9cb6-2fca77af9897)
# 1-b)
![ex2_2](https://github.com/user-attachments/assets/3854152f-2b1d-4a1b-8497-9a9fe5771b17)

*Timing Diagram*
# 2-a)
![Screenshot 2025-03-14 143354](https://github.com/user-attachments/assets/0b3f910e-0f1f-43c2-a9dc-9c663001e820)

# 2-b)
![Screenshot 2025-03-26 142443](https://github.com/user-attachments/assets/7aa0b28d-f3cb-4b51-b518-c08af29634a1)

*Result:*

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
