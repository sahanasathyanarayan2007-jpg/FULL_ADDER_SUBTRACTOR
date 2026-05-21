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
full adder
<img width="526" height="625" alt="image" src="https://github.com/user-attachments/assets/3bc8288d-d943-40e3-b444-56ba5dfc2b95" />


**Procedure**
```
Open the Verilog HDL software and create a new module for Full Adder and Full Subtractor.
Declare the inputs a, b, cin and outputs sum, carry, DIFF, BO.
Write the dataflow equations using assign statements for adder and subtractor outputs.
Compile the Verilog code and remove any syntax errors if present.
Simulate the program using a testbench and verify the outputs with the truth table.
```

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by:Sahana.s RegisterNumber:212225240130
*/
full adder
```
   module exp3de(a,b,cin,sum,carry);
   input a,b,cin;
   output sum,carry;
   assign sum=( (a ^ b)^cin);
   assign carry= ((a&b)| (cin&(a^b)));
   endmodule
   ```

**RTL Schematic**
full adder
<img width="917" height="437" alt="Screenshot 2026-05-21 111814" src="https://github.com/user-attachments/assets/013b444b-2349-4a55-82ec-e4ea30e718a1" />


**Output Timing Waveform**
Full adder
<img width="1907" height="917" alt="image" src="https://github.com/user-attachments/assets/16a9bcb6-88bc-4e25-aa3f-6a059a7b36b2" />


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



