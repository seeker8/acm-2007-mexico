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

The Manhattan distance is given by: Md<sub>(Si,Sj)</sub> = | A<sub>i</sub> - A<sub>j</sub> | + | 
