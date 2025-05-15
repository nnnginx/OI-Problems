# Description

Consider a binary string (b1...bN) with N binary digits. Given such a string, the matrix of Figure 1 is

formed from the rotated versions of the string.

b1 b2 ... bN-1 bN

b2 b3 ... bN b1

...

bN-1 bN ... bN-3 bN-2

bN b1 ... bN-2 bN-1

Figure 1. The rotated matrix

Then the rows of the matrix are sorted in alphabetical order, where ¡®0¡¯ is before ¡®1¡¯. You are to write a

program which, given the last column of the sorted matrix, finds the first row of the sorted matrix.

As an example, consider the string (00110). The sorted matrix is

0 0 0 1 1

0 0 1 1 0

0 1 1 0 0

1 0 0 0 1

1 1 0 0 0

and the corresponding last column is (1 0 0 1 0). Given this last column your program should

determine the first row, which is (0 0 0 1 1).

# Format

## Input

The input file name is bincode.in. The first line contains one integer N, the number of binary digits

in the binary string. The second line contains N integers, the binary digits in the last column from top

to bottom.

## Output

The output file name is bincode.out. The first line contains N integers: the binary digits in the first

row from left to right.

# Samples

```input1
5 
1 0 0 1 0
```

```output1
0 0 0 1 1
```

# Limitation

Constraints

For the length of the binary code we have $1 < N \leq  1000$.

Solution

The following algorithm can be used to solve the problem.

Algorithm LinearBincode

1. Count the number of 0's and the number of 1's in the last column, and form the first

column from them.

2. Create an array Next which contains row numbers so that the row with the ith 0 in the first

column points to the row with the ith 0 in the last column, and similarly with 1's.

3. Starting from the first row, go through the rows following the row indexing in Next, that

is, from row k go to row Next[k], and form missing items of the first row from the last

column values in the order in which the rows are traversed.

Lemma 1. LinearBincode solves the Bincode problem.

Proof. We say that the successor of a string is its left rotation. To prove the correctness of the

algorithm, we show that the array Next represents this successor relationship of the rotated strings.

Then, it is fairly obvious that Step 3 correctly recovers the first row of the sorted matrix.

Consider the rows beginning with a ¡®0¡¯ in the sorted matrix. Because they are in alphabetical

order with matching first bits, their left rotations (with the ¡®0¡¯ in last column) must also be inalphabetical order among themselves. This means that the successors of the rows starting with a ¡®0¡¯

appear in order as the rows ending with a ¡®0¡¯ in the sorted matrix. The same holds for the rows starting

with a ¡®1¡¯ and their successors.

Lemma 2. LinearBincode runs in linear time and space.

Proof. Linear time complexity is evident, since the algorithm only traverses the input column to

count the 0's and 1's, initializes Next, and then traverses Next. Linear space complexity is also evident

as only some index variables are needed in addition to the necessary additional array Next.

In addition to LinearBincode, which obviously is an asymptotically optimal solution, we also consider

three other attempts to solve the problem. These are referred to in evaluation data generation section.

Algorithm IterativeBincode

1. Initialize a working matrix with N rows and initially 0 columns.
2. Prepend the input column to the left of the matrix and sort the rows.
3. If the matrix has less than N columns, go to 2.
4. Output the first row.

Lemma 3. IterativeBincode solves the Bincode problem.

Proof. We show by induction that the algorithm builds the sorted matrix column by column

starting from the first column. The initial step with 0 columns is trivial. Suppose then that the matrix

has I < N columns, which are the I first columns of the sorted matrix. Prepending the last column of

the sorted matrix yields the I + 1 first columns of a right rotation of the sorted matrix. By sorting the

resulting matrix, we obtain the I + 1 first columns of the sorted matrix, because a rotation of the sorted

matrix still has the same set of rows and the order given by the first k + 1 columns can only differ from

the correct order for rows that have the same I + 1 initial columns.

A trivial implementation of IterativeBincode requires at least cubic time because there are N

iterations and each iteration must sort a matrix of quadratic size. By noting that each sort opeartions

yields the same permutation with the rows beginning with a ¡®0¡¯ moved to front, the analysis of this

algorithm quickly leads to the successor realtionship of the above LinearBincode algorithm.

The algorithm ExhaustiveBincode works as follows.

Algorithm ExhaustiveBincode

1. Generate a binary string with N binary numbers, all 0's.2. Generate the matrix and sort it.
2. If the last column is the input column, a solution has been found, stop.
3. Generate the next binary string with N binary numbers in the alphabetical order and go to
4. 

Clearly, ExhaustiveBincode is not optimal, but since it tests all possible solutions, if needed, it is

guaranteed to solve the problem.

The last attempt is based on guessing the bincode. Since the first row is first in the sort order, it is

more likely that 0's are at the left end of the row.

Algorithm GuessBincode

1. Count the number of 0's I in the input column.
2. Generate the row with first I zeros and then N - I ones.

Test data

The test data contains 20 test cases, each generated by sorting the rotations of an input string as

described in the problem setting. The input strings are all random, except for the following four cases

of length 100

- all 1's
- all 0's
- 01...01
- 0...01...1,

which are included for the purpose of detecting defects in handling of special cases. Also three small

inputs of lengths 5, 10, and 20 are included so that inefficient but correct solutions can score some

points. The lengths of the remaining 13 inputs range from 300 to 1000.

Each test case is worth 5 points and the distribution of input lengths is chosen so that the example

implementations of LinearBincode, IterativeBincode, ExhaustiveBincode, and GuessBincode

algorithms score 100, 40, 10, and 15 points, respectively.

Background

This problem is a special case of the reversible transform used in the Burrows-Wheeler block sorting

compressor [1]. The original version used a general alphabet. The idea of using only a binary alphabet

is that the task is then simpler but at the same time the solution is less obvious as the substring given bythe last and the first characters of a row seems rather useless now as it can appear in quite many

positions of the input string.

Reference

[1]

M. Burrows and D. J. Wheeler, A block-sorting lossless data compression algorithm, Digital

System Research Center, Research Report 124,

