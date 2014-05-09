CE5_Agnolutto
=============
### Task 1
Line 1: addi $s0, $0, 44 #iniitialized register at $s0 and assigned the value 44 to it.

Line 2: addi $s1, $0, -37 #initialized register at $s1 and assigned the value -37 to it.

Line 3: add $s2, $s0, $s1 #add the values from the two registers and store it in $s2.

Line 4: sw $s2, 0(x)54($0) #stores value of $s2 into hexadecimal memory address 0x54.

### Task 2

#### I-Type

Lines 1, 2, and 4 are all I-Type instructions.

All I-Type's follow the format:

|OP|rs|rt|imm|
|:--------:|:------:|:-----:|:-------------:|
|6 bits|5 bits|5 bits| 16 bits


#####Line 1 reads:

| Value   | Field Value   | Machine Code  |
|:--------:|:------------:|:-------------:|
| OP | 8 |001000 |
| rs   | 0 | 00000| 
| rt   | 16 | 10000 |
| imm  | 44  | 0000000000101100 |

Concatenated: 0010 0000 0001 0000 0000 0000 0010 1100

Hexdemical: 0x2010002C

#####Line 2 reads:

| Value   | Field Value   | Machine Code  |
|:--------:|:------------:|:-------------:|
| OP | 8 |001000 |
| rs   | 0 | 00000| 
| rt   | 17 | 10001 |
| imm  | -37  | 1111111111011011 |

Concatenated: 0010 0000 0001 0001 1111 1111 1101 1011

Hexdemical: 0x2011FFDB

#####Line 4 reads:

| Value   | Field Value   | Machine Code  |
|:--------:|:------------:|:-------------:|
| OP | 43 |101011 |
| rs   | 0 | 00000| 
| rt   | 18 | 10010 |
| imm  | 54  | 0000000001010100 |

Concatenated: 1010 1100 0001 0010 0000 0000 0101 0100

Hexdemical: 0xAC120036

#### R-Type

Lines 3 is an R-Type instruction.

All R-Type's follow the format:

|OP|rs|rt|rd|shamt|function|
|:--------:|:------:|:-----:|:----:|:----:|:----:|
|6 bits|5 bits|5 bits| 5 bits|5 bits|5 bits|6 bits|

#####Line 3 reads:

| Value   | Field Value   | Machine Code  |
|:--------:|:------------:|:-------------:|
| OP | 0 |000000 |
| rs   | 16 | 10000| 
| rt   | 17 | 10001 |
| rd  | 18| 10010 |
|shamt| 0| 00000|
|function|32 | 100000|

Concatenated: 0000 0010 0001 0001 1001 0000 0010 0000

Hexdemical: 0x02119020

















