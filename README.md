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
module combinationalcircuit(A,B,C,D,F1);
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
![WhatsApp Image 2023-12-22 at 14 05 23_7aead406](https://github.com/Kamal-Raj-A/Experiment--02-Implementation-of-combinational-logic-/assets/145742556/f3211b49-bd3c-4302-b3a9-f71f4ba58fe1)
**Output:**
![WhatsApp Image 2023-12-22 at 14 07 03_020500d0](https://github.com/Kamal-Raj-A/Experiment--02-Implementation-of-combinational-logic-/assets/145742556/5e57d2a5-c8e3-4ba8-988e-042ebba5119b)
**RTL**

**Timing Diagram**
![IMG_20231223_100210](https://github.com/Kamal-Raj-A/Experiment--02-Implementation-of-combinational-logic-/assets/145742556/61447713-d289-43b1-a284-df6ea5067c3c)
**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

