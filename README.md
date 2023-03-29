# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:Preethi.A.A 
RegisterNumber:212222110035

HALF ADDER:

module halfadder(A,B,C,S);
input A,B;
output S,C;
xor(S,A,B);
and(C,A,B);
endmodule

FULL ADDER:

module fulladd(A,B,Ci,S,Co);
input A,B,Ci;
output S,Co;
wire D,E,F;
xor(D,A,B);
xor(S,D,Ci);
and(E,Ci,D);
and(F,A,B);
or(Co,E,F);
endmodule

```
*/
###LOGIC GATES:
Logic symbol of Half adder:

![Screenshot 2023-03-29 220702](https://user-images.githubusercontent.com/120115840/228607940-1802d49e-5d56-4a07-9dec-8db8baa4e43a.png)

Logic symbol of Full adder:

![Screenshot 2023-03-29 220543](https://user-images.githubusercontent.com/120115840/228607774-18f8878c-6cf2-4a80-b380-ad349fe59821.png)

###TRUTH TABLE:
Truth table of Half adder:

![Screenshot 2023-03-29 221152](https://user-images.githubusercontent.com/120115840/228609054-f763847f-8df3-4bf7-86ae-057093053e2d.png)

Truth table of Full adder:

![Screenshot 2023-03-29 221046](https://user-images.githubusercontent.com/120115840/228608793-884ca3b5-2b0b-45dd-b94d-c2be95953a80.png)

###RTL:
RTL realization of Half adder:

![half adder gate](https://user-images.githubusercontent.com/120115840/228608422-e3c3486a-c1a5-46cb-acc1-bed4b8a3fa52.png)

RTL realization of Full adder:

![fulladder gate](https://user-images.githubusercontent.com/120115840/228608287-9413bebb-37d8-4ff6-aeb0-bac46f3bc208.png)

### Waveform:
Half adder:

![half adder table](https://user-images.githubusercontent.com/120115840/228610175-466fea28-01f2-4029-a23c-ed9591613c84.png)

Full adder:

![fulladder waveform](https://user-images.githubusercontent.com/120115840/228610287-35ed925e-f211-4388-855a-ca65fd714dc6.png)

### Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
