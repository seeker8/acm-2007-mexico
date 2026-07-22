## Problem No. 5 - Geophysics Prospection

**Input file**: prospection.in **Output file**: Standard Output

The geophysics prospection is a tool that permits to predict the subsoil characteristics, working at variable deeps with multiple targets such as rock differentiation, identification of freatic surfaces and identification of contiaminated areas.

A Geo-explotation company determines the capacity of explotation of the terrain in terms of the analysis of geophysics prospection of a sample of $m$ adjacent longitudinal layers. Each layer is represented by a matrix of $p \times k$ materials. Materials are identified by a code. The set of layers form a three-dimensional matrix that models the characteristics of the subsoil studied. The problem is to identify the grouping patterns of a same exploitable material. A group of material is that wich is contained in adjacent boxes of the layer matrix. Two boxes are adjacent if they share four sides in common.

The material codes and their meaning are described in the following table.

| Code | Meaning |
| ---- | ------- |
| a    | A mix of sand and gravel  |
| b    | Clay                      |
| c    | Mineral                   |
| d    | Gravel                    |
| *    | Material without interest |

### Input
There will be multiple datasets separated by a blank line. Each dataset consists of two parts. The first part is a line with three positive integers to define the matrix dimensions: $p(2 \leq p \leq 50)$, space, $m(2 \leq m \leq 50)$. The second part contains the $m$ layers separated by a blank line. Each layer consists of $p$ lines and each line containes $k$ characters representing material codes.

### Output
The output consists of the grouping pattern of each dataset separated by a blank line. For each dataset, a line with: the string Case, a space, an integer representing the progressive number of dataset (start counting at one), and an ending colon. The next four lines correspond to the materials with explotation interest, with the same order that they appear in the input. Each line consists of a character that represents a material code, followed by a variable number of integers that correspond to the elements of identified groups, in descending order. All data in the line are separated by a space.
