## Problem No. 7 - Friend Numbers

**Input file**: friend.in **Output file**: Standard Output<br>
**Time Limit**: 20 sec

Friend number are those who are composed of the same digits, for example $3123$ and $11233233$ are friend numbers, but $1233432$ and $123331$ are not friend numbers because in the second number the 4 is missing.

Your task is this: given an integer closed range $[A, B]$, an integer number $N$ and an integer $K$, you must  find the $Kth$ friend number of $N$ in that range.

### Input]
Input will consist of several test cases each of them in a separate line. For each test case you will receive four (with no leading zeros) integers $A, B, N$ and $K(0 < A \leq B < 10^{100}, 0 \leq N \leq 10^{100}, 0 < K \leq 10^{17})$.

### Output
For each test case you must print a line containing a number representing the $Kth$ friend number in the given range, or "-1" if it is not possible to obtain the $Kth$ friend number.

### Sample Input
1 191010100333 1003 20000<br>
1 200 1 3<br>
1 200 1 4<br>
1 200 211 1<br>
1 200 211 2<br>
1 200 211 3

### Sample Output
1010110131<br>
111<br>
-1<br>
12<br>
21<br>
112
