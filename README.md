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
<img width="890" height="512" alt="EX 4 LOGIC 1" src="https://github.com/user-attachments/assets/953fb562-d9e5-477f-9cfd-0660d354d14d" />

FULL SUBRACTOR
<img width="891" height="513" alt="EX 4 LOGIC 2" src="https://github.com/user-attachments/assets/35ca3ae2-ca5b-4ff7-a17a-206b9f7a9412" />


**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
FULL ADDER
module fa(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^cin);
assign carry= ( (a & b)| ( cin &(a ^ b )));
endmodule

FULL SUBTRACTOR
module fs(a,b,bin,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference= ( (a ^ b)^bin);
assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b ))));
endmodule


Developed by:Rishikesh S
RegisterNumber:25005617
*/

**RTL Schematic**

FULL ADDER
<img width="890" height="512" alt="EX 4 LOGIC 1" src="https://github.com/user-attachments/assets/1ef63499-e437-4063-a346-bd2c07ac3c86" />


FULL SUBRACTOR
<img width="891" height="513" alt="EX 4 LOGIC 2" src="https://github.com/user-attachments/assets/2c9b12a6-97ee-4500-bd5a-96188898ff34" />


**Output Timing Waveform**

FULL ADDER
<img width="960" height="551" alt="EX 4 WAVE 1" src="https://github.com/user-attachments/assets/7b84afc8-555c-4fc1-a46e-f8055f2809fa" />


FULL SUBRACTOR
<img width="960" height="512" alt="EX 4 WAVE 2" src="https://github.com/user-attachments/assets/e3e10e21-4fcb-444f-bd8b-e3a07e2690ab" />



**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



