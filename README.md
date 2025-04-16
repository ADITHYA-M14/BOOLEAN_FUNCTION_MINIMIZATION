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
```
module func(a,b,c,d,f1); 
input a,b,c,d; 
output f1; 
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c)); 
endmodule

module func1(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(w&y)|(x&y));
endmodule
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by : ADITHYA M
RegisterNumber: 212224230008


**RTL realization**

**Output:**

**RTL**
![Screenshot 2025-04-16 131949](https://github.com/user-attachments/assets/e85fcf0e-96d5-491f-bcbf-f09efae568d9)

![Screenshot 2025-04-16 132006](https://github.com/user-attachments/assets/fe22daf9-5b53-4f2a-89bc-d178df5d55b1)


**Timing Diagram**
![Screenshot 2025-04-16 132019](https://github.com/user-attachments/assets/9f9a1d83-a8f6-4ca5-8485-73d929bb3d32)

![Screenshot 2025-04-16 132032](https://github.com/user-attachments/assets/e5b6da23-879e-458b-ae00-ebf2cf9912b0)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

