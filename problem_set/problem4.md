## Problem No. 4 - Decode Messages

**Input file**: decode.in **Output file**: Standard Output

Being in charge of the computer department of the Agency of International Espionage, you are asked to write a program that will allow a spy to decode their messages.

You can assume a spy's message is at most 400 characters long, and it includes all the uppercase letters of the English alphabet plus the space, any digit, and any of the following characters: _! , . : ; ? -_

The algorithm that the department will use to encode all their messages will be following:

They first encode the message with a simple code key. This simple code key is a one for one character substitution based upon a single arithmetic manipulation of the printable portion of the ASCII character set (0-126). This single arithmetic manipulation is the same for each character of the message.

After, they agree secretly on two numbers that will be used as the number of rows (R) and columns (C) in a matrix.

For example, if the message is:

**CDC IS THE TRADEMARK OF THE CONTROL DATA CORPORATION**

and there $R=9$ and $C=6$, the department would write down.

### Message encode

**4JKJ'PZ'[OL'[YHKLTHYR'VM'[OL'JVU[YVS'KH[H'JVYWVYH[PVU5**

The matrix would be filled in as follows:

<!-- add image -->
<img width="376" height="440" alt="image" src="https://github.com/user-attachments/assets/63fd0aca-6335-496e-b488-00809e8eea1b" />


### Input
There will be multiple datasets. Each dataset consist of two lines. The first line contains $R (2 <= R <= 20)$, a space, $C (2<=C<=20)$. The next line is a string of characters that represent the contents of the matrix $(R x C characters)$. The characters are in row major order. The last input set is followed by a line containing two zeros $(0,0)$. This line should not be processed.

### Output
For each dataset, you should have one line of output, giving the decoded message.

### Sample Input
9 6<br>
4JKJ'P[OL'JZ'VYWV'MJ5VU[V'UY[O'HVHYLR[P[V'YHK'S[HTLKHY<br>
0 0

### Sample Output
-CDC IS THE TRADEMARK OF THE CONTROL DATA CORPORATION.
