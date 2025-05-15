# Description

Santa Claus has found a nice new sleigh from the sleigh shop. Santa's old sleigh and the new sleigh

have equal amount of room for the magic boxes Santa Claus uses to carry Christmas presents. For

comparing sleighs, Santa's elves have carried a set of boxes to the shop. Each box has an integer

volume. Santa Claus wants to compare the flying properties with sleighs packed so that the sums of the

box volumes in the sleighs are as close as possible to a desired value.

Suppose that the desired sum of box volumes for both sleighs is D, and that a sleigh is packed so

that the sum of the volumes in the sleigh is S. If S £D, then the filling of that sleigh is S, and

otherwise the filling is max(0, 2D - S). Given volumes of the available boxes and the required filling of

the sleighs, you are to find such a placement of boxes for the two sleighs that the sum of the fillings of

the two sleighs is as large as possible.

# Format

## Input

The input file names are boxes.inI, where I is one of characters 1, 2, 3, 4, or 5. The first line of the

input file contains one integer, the number of boxes N, $1 \leq N \leq 17$. The second line contains the

desired sum of box volumes D, which is the same for both sleighs. For D it holds that $1 \leq D \leq 100 000$

0. The third line contains N integers $W_1$, $W_2$,...,$W_N$, the volumes of the N boxes. For each $W_i$ we have

$1 \leq W_i \leq 50 000 000$ ($1\leq i\leq n$).


## Output

The first line of the output file contains the string

#FILE boxes I

where I is the number of the input file respective to this output file. The second line contains one

integer F, the sum of the fillings of the two sleighs. Then follow N lines, which describe the placement

of the boxes as follows. On each of these lines there are two integers, W and K, where W is the size of

one of the boxes (each box must appear in output), and K is the sleigh number of the sleigh for that

box. Use sleigh numbers 1 and 2 for the sleighs and 0 if the box should not be placed in either of the

sleighs.

# Samples

```input1
5
11
5 6 7 8 9
```

```output1
#FILE boxes 0
20
7 0
9 2
8 0
5 1
6 1
```

# Limitation

The problem is NP-complete and hence enumerative solution can be used only for small inputs.

Number of boxes is bound by 17, and there are only two sleighs. Hence, this can be considered as a

small case, and by trying every solution we'll find the right answer.

There are at most 317 = 129140163 different solutions. We have to use three, because it is not

required that every box is assigned into a sleigh.

Idea of the enumerative solution is the following. Let the number of boxes is b. We use a vector

of length b to describe the assignment of each box into sleigh (1 or 2) or to tell that the item is not

assigned at all (value 0). Now we can interpret the solution vector as a 3-base number having n-digits.

Short pseudo-code of the enumerative solution:

1. Initialize variables
2. j = n - 1 (n is the number of the magic boxes)
3. while (j > -1)
4. Count the result for this solution. Record, if new best found.
5. Increase number by one.
6. if all slots 0 to n - 1 in the solution contain 2, set j = -1.

