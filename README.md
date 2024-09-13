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
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

module HALF_ADDSUB(a,b,sum,carry,D,Bo);
input a,b;
output sum,carry,D,Bo; 
wire abar;
not(abar,a);
xor(sum,a,b);
and(carry,a,b);
xor(D,a,b);
and(Bo,abar,b);
endmodule
```
```
Developed by: Easwari M
RegisterNumber: 212223240033*/
```

**RTL realization**
![wave](https://github.com/user-attachments/assets/c7fea907-d0de-4d0d-b634-786e9117aec1)


**Output:**
![wave](https://github.com/user-attachments/assets/ae0fbd59-b227-4108-b97b-f96da118f708)


**RTL**
![rtl](https://github.com/user-attachments/assets/318a69e2-d1ff-4c7c-9236-6a5b47b5a8f3)


**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

