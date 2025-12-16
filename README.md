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

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

**Half Adder**
// Half Adder in Verilog module half_adder ( input wire a, b, // Inputs output wire sum, // Sum output output wire carry // Carry output );
```
// Logic equations
assign sum   = a ^ b;   // XOR for sum
assign carry = a & b;   // AND for carry
```
end module

**Half Subtractor**

// Half Subtractor in Verilog module half_subtractor (input  wire a, b, // Inputsoutput wire diff, borrow  // Outputs);

    // Logic equations
    assign diff   = a ^ b;     // XOR for difference
    assign borrow = ~a & b;    // Borrow when a < b

endmodule

Developed by:Yuvasri V
RegisterNumber:25008890

**RTL Schematic**
half adder:

<img width="927" height="521" alt="digi" src="https://github.com/user-attachments/assets/c04d8a13-9d9f-4583-8a40-792a0155f415" />

half subtractor:

<img width="990" height="619" alt="digi1" src="https://github.com/user-attachments/assets/bab51d8e-23a1-4977-a879-60ede1f08e8c" />

**Output/TIMING Waveform**
half adder:
<img width="1298" height="334" alt="digi2" src="https://github.com/user-attachments/assets/008bde8a-b697-46ae-a7ea-b46aa1654a68" />

half subtractor:
<img width="1308" height="367" alt="digi3" src="https://github.com/user-attachments/assets/fd662ec2-a95b-4476-b296-34c6be333664" />

**Result:**
Thus, the program to design a half adder and full adder circuit is executed and verified in Quartus using Verilog programming successfully.
