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

**Truthtable**





![WhatsApp Image 2025-03-26 at 3 06 00 PM](https://github.com/user-attachments/assets/ab93c04a-8ceb-4b3e-8f9a-9c10abd46cee)







![WhatsApp Image 2025-03-26 at 3 06 13 PM](https://github.com/user-attachments/assets/a1d04bdd-dad1-4110-9238-916ac8350b5d)








**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
HALF ADDER
``` 
module ha(a,b,sum,carry);
 input a,b;
 output sum,carry;
 assign sum=(a^b);
 assign carry=(a&b);
 endmodule
```
```
HALF SUBTRACTOR
  module hs(a,b,difference,borrow);
 input a,b;
 output difference,borrow;
 assign difference=(a^b);
 assign borrow=(~a&b);
 endmodule
```




Developed by: somalarajurohini RegisterNumber:*/24000337

**RTL Schematic**

![Screenshot 2025-03-26 151601](https://github.com/user-attachments/assets/f92b1ec4-4b4f-47d7-ba4f-2f022d1da1dc)










![Screenshot 2025-03-26 151605](https://github.com/user-attachments/assets/8874f195-428d-4ac2-a77d-71391e04597a)






**Output/TIMING Waveform**





![Screenshot 2025-03-26 151714](https://github.com/user-attachments/assets/defe2688-4fc8-4e5c-b8b7-2436f5b8ffa5)





![Screenshot 2025-03-26 151728](https://github.com/user-attachments/assets/f5c69aa7-bb40-447e-90f0-46f9a35cc5ea)





**Result:**
Thus the half adder and half subtractor are studied and the truth table table,logic gates are verified in Quartus II using Verilog programming
