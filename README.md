# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
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
STEP 1: Use module project name(input,output) to start the Verilog programmming.

STEP 2: Assign inputs and outputs using the word input and output respectively.

STEP 3: Use defined keywords like wire,assign and required logic gates to represent the boolean expression.

STEP 4: Use each output to represnt onre for differnce and the other for borrow.

STEP 5: End the verilog program using keyword endmodule.


## Program:
```
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: mathan raj
RegisterNumber:212222230079  
```

## Output:

## HALF SUBTRACTOR
![halfsubl](https://user-images.githubusercontent.com/118680259/233824055-9da2baa9-94bb-4f10-a700-3f2472638b33.png)
## FULL SUBTRACTOR
![fullsub](https://user-images.githubusercontent.com/118680259/233824067-9309b14b-f59b-4069-aac7-5123001498ff.png)
## Truthtable
## HALF SUBTRACTOR
![half truth](https://user-images.githubusercontent.com/118680259/233824091-a74aa6de-3ecd-4eb0-8d70-2f19e2a1792a.png)
## FULL SUBTRACTOR
![full truth](https://user-images.githubusercontent.com/118680259/233824122-edd6588a-05c5-4c32-850c-64b3192f0107.png)




##  RTL realization
## HALF SUBTRACTOR
![rtl half](https://user-images.githubusercontent.com/118680259/233824139-614281fb-7a96-418d-87cf-fa5c5a22ecae.png)
## FULL SUBTRACTOR
![rtl full](https://user-images.githubusercontent.com/118680259/233824142-70b4f112-0786-4353-b888-1c18ba03bc21.png)


## Timing diagram 
## HALF SUBTRACTOR
![time half](https://user-images.githubusercontent.com/118680259/233824151-bd2966f5-ac1f-4296-8a84-b51c8613489a.png)
## FULL SUBTRACTOR
![timing full sub](https://user-images.githubusercontent.com/118680259/233824165-a89cca36-92c0-4ed4-b055-95aca95f5d54.png)

## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
