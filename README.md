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
~~~
module experiment2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~c)|(~a&b&d)|(a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule
~~~
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:Yugabharathi .T RegisterNumber:24900006

**Truth table:**
![392007889-b2e6f509-64de-444c-a5fa-e40898d2b160](https://github.com/user-attachments/assets/830058ab-a0c3-4731-96e2-f6705a60d6c3)
![392007968-0ff0cc8d-a388-4297-ac03-7771303160b7](https://github.com/user-attachments/assets/330bf3e8-b001-4253-962a-f10308e62406)

**RTL realization**
![383127164-67542647-c6fb-4065-9d0f-0ce48d11cae0](https://github.com/user-attachments/assets/22905d4c-1d08-4adf-9d0d-c84dcd997db1)

**Output:**

**RTL**
![387574673-4bfc069b-5f93-4d1a-b89d-8529cbe889b7](https://github.com/user-attachments/assets/eacca589-e4cf-4e39-9cc7-3976648814bf)

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

