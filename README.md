# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.


## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure
```
1. Use module projname(input,output) to start the Verilog programmming.

2. Assign inputs and outputs using the word input and output respectively.

3. Use defined keywords like wire,assign and required logic gates to represent the boolean expression.

4. Use each output to represnt onre for differnce and the other for borrow.

5. End the verilog program using keyword endmodule
```

## Program:
```
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: R.LOGA MITHRA
RegisterNumber: 212223100027
```

## Output:
## Truthtable
HALF SUBTRACTOR

![image](https://github.com/mithra916/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149986612/438d2d7b-0b47-4ed0-8788-d6f36ea47183)

FULL SUBTRACTOR

![image](https://github.com/mithra916/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149986612/761cc9cb-db92-4808-8197-c063b9d15f5b)

##  RTL realization
HALF SUBTRACTOR

![image](https://github.com/mithra916/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149986612/84589f2f-0af5-4165-a4be-f433d6f8f41c)


FULL SUBTRACTOR

![image](https://github.com/mithra916/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149986612/5a151710-5be4-43a3-86d5-7589f5669f74)

## Timing diagram 
HALF SUBTRACTOR

![half_subtractor EX NO4(1)](https://github.com/mithra916/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149986612/cc5f07df-b471-4f3c-bfff-4266c5589398)

FULL SUBTRACTOR

![full_subtractor EX NO 4(2)](https://github.com/mithra916/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/149986612/7480c2ac-7815-444d-a4b2-64bbf49fb898)

## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
