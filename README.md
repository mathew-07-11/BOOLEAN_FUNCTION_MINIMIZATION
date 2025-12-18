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
module exp2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```
Developed by: TINU MATHEW M
RegisterNumber: 25015787


**RTL realization Output**

<img width="1366" height="768" alt="Screenshot 2025-11-20 142240" src="https://github.com/user-attachments/assets/22da7627-b786-4863-a903-b1afb57de6c6" />

**RTL**
<img width="1366" height="768" alt="Screenshot 2025-11-20 142502" src="https://github.com/user-attachments/assets/4a0d15ff-2e0e-4cf3-8b71-63f27c02573c" />

**Timing Diagram**
![WhatsApp Image 2025-11-20 at 2 28 04 PM](https://github.com/user-attachments/assets/b0add289-0bb3-47b3-8e34-c7bbf143e21d)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

