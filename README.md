# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
Boolean function minimization is the process of simplifying Boolean algebraic expressions to reduce the number of logic gates and complexity in a digital circuit leading to more efficient, faster, and less costly hardware

For minimizing Boolean expressions, we can use a set of rules and laws (like distributive, associative, and complement laws) to simplify Boolean expressions. This method focuses on applying algebraic manipulations to reduce the complexity of the expression by eliminating redundant terms.

Identity Law A . 1 = A, A + 0 = A

Null Law A . 0 = 0 ,A + 1 = 1

Idempotent Law A AA, A+A=A

Complement Law A * A' = 0 , A + A' = 1

Distributive Law A (B+C) A-B+A-C

De Morgan's Law (AB)' A' B', (A + B) = A' B'

Absorption Law A (A+B) A, A+ (AB) = A

Associative Law A+ (B+C) = (A+B) + C, A.(B.C) = (A.B).C

Commutative law A B BA,A+B=B+A



**Logic Diagram**

<img width="610" height="342" alt="image" src="https://github.com/user-attachments/assets/e32f37fb-e7a1-4aac-b871-5f58b423f6b5" />
<img width="557" height="514" alt="image" src="https://github.com/user-attachments/assets/9613276b-291e-432b-a924-fe5aa57cb549" />
<img width="845" height="1330" alt="image" src="https://github.com/user-attachments/assets/aab4b36c-bd1b-4a90-b625-6cf6b4484fad" />
<img width="844" height="1353" alt="image" src="https://github.com/user-attachments/assets/4f3acd47-5e8b-4f02-b49e-e5297e0f7a66" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
i)
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

ii)
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule

**RTL realization**

**Output:**
i)
<img width="1920" height="1080" alt="Screenshot (25)" src="https://github.com/user-attachments/assets/9a054cd0-2711-433d-90a0-4b975d21af17" />

ii)
<img width="1920" height="1080" alt="Screenshot (27)" src="https://github.com/user-attachments/assets/af8e7137-4721-47f5-bea9-de98fab60209" />


**RTL**

**Timing Diagram**
i)
<img width="1920" height="1080" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/7212250c-7562-4de9-875c-5e6c421f3893" />

ii)
<img width="1920" height="1080" alt="Screenshot (28)" src="https://github.com/user-attachments/assets/5cbb52c5-c624-434f-b546-bf9d4f861d12" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.


