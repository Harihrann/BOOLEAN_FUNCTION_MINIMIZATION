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
module halfsubtractor(a, b, dif, bor);
    input a;
    input b;
    output dif;
    output bor;
	        reg dif,bor;
			  reg abar;
	        always@(a or b) begin
	        abar=~a;
	        dif=a^b;
	        bor=b&abar;
	        end
endmodule
```

Developed by: HARIHARAN 
RegisterNumber:24005920


**RTL SCHEMATIC**
![4](https://github.com/user-attachments/assets/e3faf0b0-a9ab-4ad7-8906-18c7a556981f)
![5](https://github.com/user-attachments/assets/1187d2e5-4568-4e57-9202-be2875e23f91)

**Output TIMING WAVEFORM**
![6](https://github.com/user-attachments/assets/accf6e50-1ae3-486d-9682-4f164a7a2939)
![7](https://github.com/user-attachments/assets/e82b3c8a-e97c-4550-beda-c764d06be895)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

