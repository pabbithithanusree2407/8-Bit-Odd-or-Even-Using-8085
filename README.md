# 8-Bit-Odd-or-Even-Using-8085

## Aim:
To write an 8085 microprocessor program to check whether a given 8-bit number is odd or even.

## Apparatus Required:
•	Laptop with an internet connection

## Algorithm:
1.	Load the number from a specified memory location into register A.
2.	Perform an AND operation with 01H to check the least significant bit (LSB).
3.	If the result is 0, the number is even; otherwise, it is odd.
4.	Store the result in a specific memory location (odd or even flag).


## Program:

```
LDA 4200H
ANI 01H
JZ L1
MVI A,01H
JMP L2
L1:MVI A,02H
L2:STA 4201H
HLT
```

## Output:

ODD:

<img width="1727" height="478" alt="image" src="https://github.com/user-attachments/assets/77ef03ce-0e29-4cb0-984f-01a532c62bd1" />

EVEN:

<img width="1820" height="585" alt="image" src="https://github.com/user-attachments/assets/a0c3ff80-8b7f-4fae-94a9-f7c3e48b1f47" />



## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

