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

<img width="368" height="339" alt="EX 4 TABLE 1" src="https://github.com/user-attachments/assets/9837caab-e425-435c-b965-08386fb4c7c8" />


FULL SUBRACTOR

<img width="357" height="337" alt="EX 4 TABLE 2" src="https://github.com/user-attachments/assets/4d279501-80b3-4b8b-b084-2a8194e216cc" />


**Procedure**

FULL ADDER: 1.Open Quartus II and create a new project.

2.Use schematic design entry to draw the full adder circuit.

3.The circuit consists of XOR, AND, and OR gates.

4.Compile the design, verify its functionality through simulation.

5.Implement the design on the target device and program it.

FULL SUBRACTOR:

1.Follow the same steps as for the full adder.

2.Draw the full subtractor circuit using schematic design.

3.The circuit includes XOR, AND, OR gates to perform subtraction.

4.Compile, simulate, implement, and program the design similarly to the full adder


**Program:**

FULL ADDER
```
module fa(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=( (a ^ b)^cin);
assign carry= ( (a & b)| ( cin &(a ^ b )));
endmodule
```

FULL SUBTRACTOR
```
module fs(a,b,bin,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference= ( (a ^ b)^bin);
assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b ))));
endmodule
```

Developed by: Rishikesh S 

RegisterNumber: 25005617

**RTL Schematic**

FULL ADDER

<img width="890" height="512" alt="EX 4 LOGIC 1" src="https://github.com/user-attachments/assets/94c398d5-b18e-42f6-a4b3-2b62310465f9" />


FULL SUBRACTOR

<img width="891" height="513" alt="EX 4 LOGIC 2" src="https://github.com/user-attachments/assets/07e02671-0b60-47af-96d9-037eaf77e9e5" />


**Output Timing Waveform**

FULL ADDER

<img width="960" height="551" alt="EX 4 WAVE 1" src="https://github.com/user-attachments/assets/68512036-bbb4-49f5-8681-c5eac475e6d8" />


FULL SUBRACTOR

<img width="960" height="512" alt="EX 4 WAVE 2" src="https://github.com/user-attachments/assets/8c68ee90-84d5-40d1-b738-13baeb91f99e" />


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



