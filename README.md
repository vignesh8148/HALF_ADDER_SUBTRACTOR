# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**HALF Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**HALF Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 FULL Subtractor

**Truthtable HALF ADDER**
<img width="1207" height="908" alt="image" src="https://github.com/user-attachments/assets/d6b8b3c0-8019-45c3-b78d-c7bf53b86ac8" />
FULL SUBTRACTOR
<img width="1197" height="896" alt="image" src="https://github.com/user-attachments/assets/3bc28e3c-bad3-4843-bce6-79f00696101f" />
**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**


Developed by:VIGNESH.K
RegisterNumber:25018207
HALF ADDER
```
 module exp4a(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^c
assign carry=(a&b)|(b&c)|(c&a);
endmodule
```
HALF SUBTRACTOR
```
 module exp4b(a,b,cin,diff,borr);
input a,b,cin;
output diff,borr;
assign diff=(~a)&c|b&c|(~a)&b;
assign borr=a^b^c;
endmodule
```
**RTL Schematic HALF ADDER**
  <img width="1879" height="984" alt="image" src="https://github.com/user-attachments/assets/4804e2a2-b922-4e79-8337-4b7f65032e90" />
  
HALF SUBTRACTOR
 <img width="1649" height="806" alt="image" src="https://github.com/user-attachments/assets/dcc78bfe-36b8-46ed-910f-11f3ddbf2020" />

**Output/TIMING Waveform HALF ADDER**
  <img width="1909" height="317" alt="image" src="https://github.com/user-attachments/assets/dc47851d-2289-4a29-9dab-6ab481d11700" />

HALF SUBTRACTOR
  <img width="1837" height="251" alt="image" src="https://github.com/user-attachments/assets/944b8319-e6d7-4e23-9736-8086f18e8e67" />

**Result:**
Hence to design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming has been verified successfully.
