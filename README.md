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



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```HALF ADDER
Sum = A’B+AB’ =A ⊕ B Carry = AB
module ha(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum= (a ^ b);
assign carry= ( a & b);
endmodule

HALF SUBTRACTOR
Diff = A’B+AB’ =A ⊕ BBorrow = A’B
module hs(a,b,difference,borrow);
input a,b;
output difference,borrow;
assign difference= (a ^ b);
assign borrow= ( ~a & b);
endmodule```

Developed by: A.DIVIYADHARSHINI
RegisterNumber:24008491

Truth Table
Half Adder
Sum = A’B+AB’ =A ⊕ B Carry = AB
![image](https://github.com/user-attachments/assets/d9908a47-1546-42a6-96f0-02a8872570c1)


Half Subracter
Diff = A’B+AB’ =A ⊕ BBorrow = A’B
![image](https://github.com/user-attachments/assets/a4cfb7be-a80b-4dee-810a-f68687be31fd)


**RTL**
Half Adder
Sum = A’B+AB’ =A ⊕ B Carry = AB
![Screenshot (6)](https://github.com/user-attachments/assets/b61ef194-0e8b-4006-89ef-81d6f674f54e)
Half Subractor
Diff = A’B+AB’ =A ⊕ BBorrow = A’B
![Screenshot (9)](https://github.com/user-attachments/assets/12122b8e-7eb2-4526-bacc-31df28c7703f)




**Output**
Half Adder
Sum = A’B+AB’ =A ⊕ B Carry = AB
![Screenshot (8)](https://github.com/user-attachments/assets/4828595c-a0c0-4b82-ab25-e240a8cd20aa)
Half Subractor
Diff = A’B+AB’ =A ⊕ BBorrow = A’B
![Screenshot (10)](https://github.com/user-attachments/assets/78a3c890-374d-4186-8b38-20345e6e2645)



**Result:**
The Half adder and half subractor circuit was verified.
