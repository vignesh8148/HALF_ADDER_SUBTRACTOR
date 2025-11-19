# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable HALF ADDER**
<img width="1207" height="908" alt="image" src="https://github.com/user-attachments/assets/d6b8b3c0-8019-45c3-b78d-c7bf53b86ac8" />
HALF SUBTRACTOR
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
module addsub(a,b,s,c);
input a,b;
output s,c;
xor g1(s,a,b);
and g2(c,a,b);
endmodule
```
HALF SUBTRACTOR
```
module sub(a,b,diff,borr);
input a,b;
output diff,borr;
assign diff=a^b;
assign borr=(~a)&b;
endmodule
```
**RTL Schematic HALF ADDER**
<img width="1915" height="1079" alt="Screenshot 2025-11-19 100621" src="https://github.com/user-attachments/assets/ed053324-1315-4b97-9de8-c7172c4edf62" />
HALF SUBTRACTOR
<img width="1910" height="1053" alt="Screenshot 2025-11-19 102617" src="https://github.com/user-attachments/assets/477e8d4c-9dd6-4c28-90e2-0b345fd9a597" />
**Output/TIMING Waveform HALF ADDER**
<img width="1917" height="1077" alt="Screenshot 2025-11-19 100912" src="https://github.com/user-attachments/assets/415acabe-bb8f-4d59-bd5e-f0cdbcfe6476" />
HALF SUBTRACTOR
<img width="1919" height="1079" alt="Screenshot 2025-11-19 103217" src="https://github.com/user-attachments/assets/bb6415dc-13ec-4ea2-8cf0-e40395685d4f" />

**Result:**
Hence to design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming has been verified successfully.
