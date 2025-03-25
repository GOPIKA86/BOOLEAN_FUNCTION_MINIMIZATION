NAME: GOPIKA A     

REG NO: 212224100017

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
module
sample2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~a)&(~b)&(~c)&(~d))|(a&
(~c)&(~d))|(~b)&c&(~d)|((~a)&b&c&d)|
(b&(~c)&d);
assign f2=(x&(~y)&z)|((~x)&(~y)&z)|
((~w)&x&y)|(w&x&(~y))|(w&x&y);
endmodule
```

**logic symbol & truth table:**

![Screenshot 2025-03-25 221249](https://github.com/user-attachments/assets/ab200469-dd82-4bc7-aca4-b22f95672ce1)

![Screenshot 2025-03-25 221316](https://github.com/user-attachments/assets/39029445-0322-4e7e-b2fd-9bfb9adfdb2f)




**RTL realization:**

![Screenshot (38)](https://github.com/user-attachments/assets/0edbf395-5787-4a1f-bed5-f79f677276af)



**RTL waveform:**

![Screenshot 2025-03-25 220642](https://github.com/user-attachments/assets/a7cf39e5-6c42-4871-87bd-c0155c69937a)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

