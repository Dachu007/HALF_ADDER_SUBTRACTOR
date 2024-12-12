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

Half Adder

![25c155be-73d9-4d6c-8513-2f0ed1d3935c](https://github.com/user-attachments/assets/05d8c4eb-9f81-434f-9f6e-957ca53697ea)

Half Subtractor

![3a838616-3605-4898-afee-b203c673a243](https://github.com/user-attachments/assets/5db1a266-fa51-4ba5-a4cf-6f1f960eb42b)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Half Adder

```
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule
```
Half Subtractor

```
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule
```

Developed by: Dharshini S RegisterNumber: 24900257

**RTL Schematic**
Half Adder

![8d39f18d-7f7d-4166-aa85-a18534eb977a](https://github.com/user-attachments/assets/5aa9a67d-08bc-4ce0-8433-3ca61ba5e3fd)
Half Subtractor

![Screenshot (17)](https://github.com/user-attachments/assets/e9751c26-6865-4ef5-8e74-4b1d6ac08bf0)


**Output/TIMING Waveform**
Half Adder

![Screenshot (16)](https://github.com/user-attachments/assets/e5239735-8ac9-4ce2-9c02-b1ec61d49b32)
Half Subtractor

![Screenshot (18)](https://github.com/user-attachments/assets/bd882689-6d20-4c11-be0b-2aaede33031d)

**Result:**

Thus the truth table of a half adder and half subtractor circuit and in Quartus using Verilog programming is verified.

