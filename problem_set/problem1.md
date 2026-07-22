## Problem No. 1 - Remedial Forecast.

**Input file**: remedial.in **Output file**: Standard Output

The Academic Development Department of the University of Hidalgo pretends to implement a remedial program to reduce the fail index in the Mathematics V course. With this purpose, the Depratment does a future performance forecast of the students with base on historical data. This data record includes the Id number (IN), average (A), number of study hours per week (SH), number of class hours per week (CH), and the result indicator obtained (R); when a student fails R = 0, otherwise R = 1. Students who obtain a failing forecast must take a remedial workshop on extra class hours.

The next table is an example of the historical results of the students who have taken a Mathematics V courses before. The number of historical results is HR.

| Id Number IN | Average of studied subjects A | Number of study hours per week SH | Number of class hours per week CH | Result R |
| --- | --- | --- | --- | --- |
| 735 | 8 | 13 | 25 | 1 |
| 724 | 7 | 10 | 28 | 0 |
| 532 | 9 | 20 | 22 | 1 |
| 677 | 6 | 10 | 22 | 0 |
| 665 | 9 | 23 | 25 | 1 |
| 512 | 8 | 15 | 20 | 0 |

The characteristic vector of any student is represented by: <br>
S<sub>IN</sub> = <A<sub>IN</sub>, SH<sub>IN</sub>, CH<sub>IN</sub>>, for example:

S<sub>735</sub> = <8, 13, 25>, S<sub>677</sub> = <6, 10, 22>

The Manhattan distance is given by: Md<sub>(Si,Sj)</sub> = | A<sub>i</sub> - A<sub>j</sub> | + | SH<sub>i</sub> - SH<sub>j</sub> | + | CH<sub>i</sub> - CH<sub>j</sub> |

Here is an example: Md<sub>S677, S512</sub> = | 6 - 8 | + | 10 - 15 | + | 22 - 20 | = 9

The next procedure is used in forecasts, with base on statistics, and the possibility that a new student in a mathematics V course could fail.


Step 1. Measure the Manhattan distance between the characteristic vector of the student and the characteristic vectors of all the students in the historical table (without considering the result parameter R).

Step 2. Sort the students table based on their distance; in case of tie, take the order as it appears in the original table. Once sorted, take the first k (an even integer number), $1 \leq k \leq HR/2$ to determine the value of the more frequent indicator result and assign it to the student who the forecast is being done to, as seen in the example for NC = 300 student

Step 1.

| | |
| - | - |
| S(735, 300) | Md= \|8-8\| + \|13-20\| + \|25-20\| = 12 |
| S(724, 300) | Md= \|7-8\| + \|10-20\| + \|28-20\| = 19 |
| S(532, 300) | Md= \|9-8\| + \|20-20\| + \|22-20\| = 3 |
| S(677, 300) | Md= \|6-8\| + \|10-20\| + \|22-20\| = 14 |
| S(665, 300) | Md= \|9-8\| + \|23-20\| + \|25-20\| = 9 |
| S(512, 300) | Md= \|8-8\| + \|15-20\| + \|20-20\| = 5 |

Step 2.

| S(532,300) | S(512,300) | S(665,300) | S(735, 300) | S(677, 300) | S(724, 300) |
| - | - | - | - | - | - |
| 3 | 5 | 9 | 12 | 14 | 19 |
| 1 | 0 | 1 | 1 | 0 | 0 |

Like $k=3$, the indicator result forecasted is 1.

### Input
The input to this problem will consist of a (non-empty) series of up to 50 data sets. Each data set will be formatted according to the following description, and there will be a blank space separating data sets.

The first data set contains historical data up to 100 students who have taken this course before. The first number in each line is an integer for the Id Number, followed by three integers corresponding to the characteristic vector of that student.

The following data sets contain an integer in the first line, corresponding to the $k$ value and in the lines to follow a table with the data of new students to whom the forecast has to be done.

### Output
The output consists of a list of pairs of integers that correspond to the students Id Number and the forecasted result, separated by a blank space.

### Sample Input
214 8 13 25 1<br>
315 7 10 28 0<br>
550 9 20 22 1<br>
120 6 10 22 0<br>
335 8 11 20 0<br>
220 10 20 22 1<br>
450 7 15 21 0<br>
180 10 14 20 1<br>
250 7 12 23 0<br>
300 8 16 23 0

3
300 8 20 20<br>
320 7 15 24

5
340 8 15 25<br>
365 10 25 20<br>
440 9 30 20

### Sample Output
300 1<br>
320 0<br>
340 0<br>
365 1<br>
440 1
