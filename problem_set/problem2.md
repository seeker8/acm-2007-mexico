## Problem No. 2 - Counting Squares.

**Input file**: counting.in **Output file**: Standard Output

### Description
Nancy is the best babysitter of the block and today she faces her greater challenge: little John and his anxious box of markers. But Nancy has prepared herself for this eventuality with an activity that it will maintain occupied little John. In a paper sheet with squares John will have to put his blue marker in some corner of a square and at the order of "right" (or left, or up or down) he will have to be draw a segment that unites the present position with the next point to its right (or left, or up, or down); the marker will be placed in that last point hoping the following instruction.

The idea is that John follows the instructions, draws a simple polygon and counts the number of squares that are within the figure. Remember that the boundary of a simple polygon does not cross itself.

### Input
In the first line is a integer number n, that represents the number of tests. In following n lines there will be a statement containing the instructions: U - up, D - down, R - right, L - left.

### Output
For each test it's necessary to indicate the number of squares that the polygon contains.

### Sample Input
2<br>
DLULDDRRRUUULD<br>
UUUULLLLDDDDRRRR

### Sample Output
case 1: 6<br>
case 2: 16
