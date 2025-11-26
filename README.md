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
module funct1(a,b,c,d,f1); 
input a,b,c,d; 
output f1; 
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c)); 
endmodule
```
```
module funct2(w,x,y,z,f2); 
input w,x,y,z; 
output f2; 
assign f2=((~y & z)|( w & y )|(x & y)); 
endmodule
```

Developed by: RegisterNumber:25018006


**RTL realization**
<img width="1920" height="1080" alt="exp2 logic diagram" src="https://github.com/user-attachments/assets/3f7e9f39-edad-468e-982b-0b86bde28e0e" />
<img width="1920" height="1080" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/5fa38b36-3b39-4e22-a1f7-d381296e43a5" />



**Output:**
<img width="1920" height="1080" alt="exp2 waveform" src="https://github.com/user-attachments/assets/6dfe201c-4aa8-43cc-9040-de657af613c9" />
<img width="1920" height="1080" alt="Screenshot (19) (1)" src="https://github.com/user-attachments/assets/7dd27408-aa66-40b5-996c-30f8c4d55192" />





**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

