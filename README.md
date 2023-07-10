# flood-it-boards

This repository contains flood-it boards and their respective smallest number of moves required to solve them.

## File Format

A line starting with # is a comment

The first line that contains no comment specifies the board dimensions an number of colors. In the format
```
m n k
```
where m is the number of rows, n the number of columns and k the number of colors. m, n, k are positive integers.

The second undommented line contains m*n positive integers in the range of 1 to k (including k) separated by a
space that row-wise specify the coloring of the board. The first integer represents the top left cell (pivot element)
of the board.

The third uncommented line contains a positive integer that indicates the number of moves of an optimal solution and can
be 0 if no such solution is known.

### Example
This 3x3 board with 5 colors which can be solved whith 5 moves
```
1 2 3
2 3 4
3 4 5
```
translates to the file:
```
# This file contains a 3x3 flood-it board with 5 colors which can be solved with 5 moves.
3 3 5
1 2 3 2 3 4 3 4 5
5
```



