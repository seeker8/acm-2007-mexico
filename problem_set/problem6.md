## Problem No. 6 - Domino Art

**Input file**: domino.in **Output file**: Standard Output

Lawliet is a very intelligent person, he is often seen solving puzzles or painting beautiful landscapes, in his new challenge he is trying to make some art with dominoes, he will draw figure on a rectangular grid consisting of $1\times1$ squares by marking some of these squares, after that he will try to cover the marked squares with dominoes. As you probably know dominoes consist of pieces of size $2 \times 1$, for simplicity we assume that the dominoes can only be put horizontally or vertically and that you have an unlimited amount of dominoes available. The cover has to be perfect, meaning that the dominoes must cover only the marked positions and the dominoes must cover all of them, also all the dominoes must lie strictly inside the rectangular grid. Bellow are shown two examples of possible figures, which correspond to the two first inputs in the sample input, the first is possible to cover with dominoes, while the second is not:

Exmaple 1 (Possible)

<!-- inset images -->

Example 2 (Impossible)

<!-- insert image -->

Now your taks is this: given a figure of marked squares on a rectangular grid, you must help Lawliet to determine if it is possible to exactly cover the figure with dominoes.

### Input
The input consists of several test cases separated by blank lines. First line of each test case contains two positive integers $R$ and $C(1 \leq R, C \leq60)$ the number of rows and columns of the rectangular grid of dots '.' and sharps '#'. Each character represents a square of the rectangular grid. A dot '.' represents a square which is unmarked and a sharp '#' represents a square marked to be part of the desired figure. A case when $R=C=0$ denotes the end of the input, this case should not be processed.

### Output
For each test case output a line containing the number of the case (starting at 1) and only one of the following two messages: If it is impossible to cover the marked squares with dominoes configuration output a single word "Impossible". If it is possible print the single word "Possible". See examploes below for more details.

### Sample Input
4 4<br>
. . # #<br>
. # # .<br>
. # # #<br>
. # # #

4 4<br>
\# \# \# \#<br>
\# \# . \#<br>
\# \# \# .<br>
. \# . \#

4 16<br>
\#  \# \#  . \# \# \# . \# \# \# . \# \# \# .<br>
 .  \#  .  . \#  .  . . \#  . \# . \#  .  . .<br>
 .  \#  .  . \#  .  . . \# \# \# . \#  .  . .<br>
\#  \# \#  . \# \# \# . \#  .  . . \# \# \# .<br>

0 0

### Sample Output
Case 1: Possible<br>
Case 2: Impossible<br>
Case 3: Impossible
