# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**


FULL ADDER
<img width="368" height="339" alt="EX 4 TABLE 1" src="https://github.com/user-attachments/assets/fb45ece1-0555-4662-9691-62070f2e4f5d" />


FULL SUBRACTOR
<img width="357" height="337" alt="EX 4 TABLE 2" src="https://github.com/user-attachments/assets/b8fbd33a-30bf-4065-87e3-19d985e1d1c7" />


**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

**RTL Schematic**

FULL ADDER
<img width="890" height="512" alt="EX 4 LOGIC 1" src="https://github.com/user-attachments/assets/cba600f5-a05f-4f9f-a399-99914dad6638" />


FULL SUBRACTOR
<img width="891" height="513" alt="EX 4 LOGIC 2" src="https://github.com/user-attachments/assets/9d0d9a7f-945c-43cc-8b6c-b6110dc2bced" />



**Output Timing Waveform**

FULL ADDER
<img width="960" height="551" alt="EX 4 WAVE 1" src="https://github.com/user-attachments/assets/bb2e9cfd-6f8a-46f1-92a6-c74373747257" />


FULL SUBRACTOR
<img width="960" height="512" alt="EX 4 WAVE 2" src="https://github.com/user-attachments/assets/1c5f8f19-953c-4707-90de-27a00eb57b42" />


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



