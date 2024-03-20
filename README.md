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
module BOOLEAN (e, f, a, b, c, d);
output e, f;
input a, b, c, d;
assign e = a || (b && c) || ((!b) && d);
assign f = ((!b) && c)|| (b && (!c) && (!d));
endmodule
```
**RTL realization**
![Screenshot (15)](https://github.com/thejaswinidhanaraj/BOOLEAN_FUNCTION_MINIMIZATION/assets/148514511/2489cefd-8f29-4889-88ae-27dbc70970f0)

**RTL**

![TRUTHTABLE](https://github.com/thejaswinidhanaraj/BOOLEAN_FUNCTION_MINIMIZATION/assets/148514511/693834f3-b1cf-4550-8259-e6708d04fe4a)

**Timing Diagram**
![Screenshot (14)](https://github.com/thejaswinidhanaraj/BOOLEAN_FUNCTION_MINIMIZATION/assets/148514511/eabd710a-3acc-4c7b-b974-5d64c0d1ce7c)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

