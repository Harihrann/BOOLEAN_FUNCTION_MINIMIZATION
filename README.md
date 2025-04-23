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
module booleanfn(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```

```
module booleanfnb(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|(w & y)|(x & y));
endmodule
```


Developed by: HARIHARAN 
RegisterNumber:24005920


**RTL SCHEMATIC**
![12](https://github.com/user-attachments/assets/b26b3dec-a70e-407f-9306-1ae6221eb7cb)
![13](https://github.com/user-attachments/assets/283d72bf-f594-4bbb-b7a1-432f28d75649)


**Output TIMING WAVEFORM**
![14](https://github.com/user-attachments/assets/74ab46bb-e664-4f83-a952-a59ee553b697)
![15](https://github.com/user-attachments/assets/74b3bed9-18ad-40b3-8676-a06048336abb)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

