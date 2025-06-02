# NAME : ADITHYA M
# REG. NO : 212224230008
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
module NITHISH(a,b,c,d,w,x,y,z,f1,f2);
  input a,b,c,d,w,x,y,z;
  output f1,f2;
  wire x1,x2,x3,x4,x5,y1,y2,y3,y4,y5;
  assign x1=((~a)&(~b)&(~c)&(~d));
  assign x2=(a&(~c)&(~d));
  assign x3=((~b)&(c)&(~d));
  assign x4=((~a)&(b)&(c)&(d));
  assign x5=(b&(~c)&(d));
  assign f1=x1|x2|x3|x4|x5;
  
  assign y1=(x&(~y)&(z));
  assign y2=((~x)&(~y)&z);
  assign y3=((~w)&x&y);
  assign y4=(w&(~x)&(y));
  assign y5=(w&x&y);
  assign f2=y1|y2|y3|y4|y5;
  endmodule
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by : ADITHYA M
RegisterNumber: 212224230008


**TRUTH TABLE**

![Screenshot 2025-05-26 193622](https://github.com/user-attachments/assets/b29ca862-0bf0-4514-a608-b4bd403421f4)
![Screenshot 2025-05-26 193633](https://github.com/user-attachments/assets/c2d87e70-2655-488b-a031-5c130edb151d)


**RTL**

![Screenshot 2025-05-26 193747](https://github.com/user-attachments/assets/5641ddd4-efe0-44ee-8d5c-67288c0a9df4)


**WAVEFORM**

![Screenshot 2025-05-26 193826](https://github.com/user-attachments/assets/60e672c5-84f7-42cd-b1b9-1e626de1efeb)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

