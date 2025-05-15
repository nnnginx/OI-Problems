# Description

Suppose that the fourth generation mobile phone base stations in the Tampere area operate as follows. The area is divided into squares. The squares form an  *S* ×*S*matrix with the rows and columns numbered from 0 to  *S* - 1. Each square contains a base station. The number of active mobile phones inside a square can change because a phone is moved from a square to another or a phone is switched on or off. At times, each base station reports the change in the number of active phones to the main base station along with the row and the column of the matrix.

Write a program, which receives these reports and answers queries about the current total number of active mobile phones in any rectangle-shaped area.

# Format

## Input and Output

The input is read from standard input as integers and the answers to the queries are written to standard output as integers. The input is encoded as follows. Each input comes on a separate line, and consists of one instruction integer and a number of parameter integers according to the following table.

| Instruction | Parameters | Meaning                                                                                                                                  |
| ------------- | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| 0           | S          | Initialize the matrix size to *S* ´*S*containing all zeros. This instruction is given only once and it will be the firstinstruction.  |
| 1           | *X Y A*   | Add*A*to the number of active phones in table square ( *X* , *Y* ).*A*may be positive or negative.                                   |
| 2           | *L B R T* | Query the current sum of numbers of active mobile phonesin squares ( *X* , *Y* ), where $L \leq  X \leq  R $, $B \leq  Y \leq T $|
| 3           |            | Terminate program. This instruction is given only once andit will be the last instruction.                                               |

The values will always be in range, so there is no need to check them. In particular, if *A *is negative, it can be assumed that it will not reduce the square value below zero. The indexing starts at 0,

e.g. for a table of size 4´4, we have $0 \leq  X \leq  3  $ and $ 0 \leq  Y \leq  3$.

Your program should not answer anything to lines with an instruction other than 2. If the instruction is 2, then your program is expected to answer the query by writing the answer as a single line containing a single integer to standard output.

## 

One integer, the sum of x and y.

# Samples

```input1
123 500
```

```output1
623
```

# Limitation

### **Programming instructions**

In the examples below, the integer last is the last one to be read from a line, and answer is the integer variable containing your answer.

If you program in C++ and use iostreams, you should use the following implementation for reading standard input and writing to standard output:

cin>>last; cout<<answer<<endl<<flush;

If you program in C or C++ and use scanf and printf, you should use the following implementation for reading standard input and writing to standard output:

scanf ("%d", &last); printf("%d\n",answer); fflush (stdout);

If you program in Pascal, you should use the following implementation of reading standard input and writing to standard output:

Read(last); ... Readln; Writeln(answer);

### **Example**

stdin	stdout	explanation

| 0 | 4 |   |     |   | Initialize table size to 4´4.               |
| --- | --- | --- | ----- | --- | ---------------------------------------------- |
| 1 | 1 | 2 | 3   |   | Update table at (1,2) with +3.               |
| 2 | 0 | 0 | 2 2 |   | Query sum of rectangle$ 0\leq X\leq 2, 0\leq Y\leq 2$. |
|   |   |   |     | 3 | Answer the query.                            |
| 1 | 1 | 1 | 2   |   | Update table at (1,1) with +2.               |
| 1 | 1 | 2 | -1  |   | Update table at (1,2) with -1.               |
| 2 | 1 | 1 | 2 3 |   | Query sum of rectangle $1\leq X\leq 2, 1\leq Y\leq 3$. |
|   |   |   |     | 4 | Answer the query.                            |
| 3 |   |   |     |   | Terminate program.                           |

### **Constraints**

| Table size                                 | S × S | 1×1$\leq  S × S \leq 1024×1024$        |
| -------------------------------------------- | -------------- | ------------------------------------------- |
| Cell value*V*at any time                  | V            | $0 \leq  V  \leq 2^{15}$ –1 (= 32767)         |
| Update amount                              | A            | $-2^{15} \leq  A \leq 2 ^{15}$ –1 (= 32767) |
| No of instructions in input                | U            | 3£  *U* £ 60002                        |
| Maximum number ofphones in the whole table | M            |  *M* = $2^{30}$                            |

Out of the 20 inputs, 16 are such that the table size is at most 512´512. NOTE: The web test facility feeds your input file to your program ’s standard input .

### **Description of the example solution**

The solution is easiest to up with by considering the 1-dimensional case i.e., a one-dimensional table (size N) with incremental updates and queries on sums of values on an interval. If the values on the table are stored as such, computing the sum of an interval requires O(N) operations. A query of the sum of values stored on a certain interval [X, Y] can also be answered by computing the cumulative sums S= [1, X-1] and M = [1, Y] and then the answer A = M - S. The sums S and M can be stored in the table, in which case the query can be answered in O(1). Maintaining the sums then causes the update to require O(N) operations.
![image](./4366/file/WNaQNIHMdJmb_38N2uvqd.png)


The binary indexed tree data structure (Figure 3) presented in [1] can support cumulative sum computation and update in O(log N) and only takes the same space as the raw table. In the tree the indices run from 1… N and each cell at index I contains the sum of an interval [$I-2 ^K +1, I$] where K is the number of trailing zeroes in the binary representation of the index of the cell. Thus the sum of an interval can be computed with 2 O(log N) queries. The next cell in an update can be computed by adding to the current index value its lowest 1 bit. Similarly in a query the next cell index can be obtained by subtracting the lowest 1-bit. An update requires updating all the cells that contain the sum of an interval containing the cell, this can also be done in O(log N) operations. The computation of sums can be made a little faster for small intervals by noting that the cumulative sum queries will eventually hit the same cells and stop at the first common cell (the query ends up adding and subtracting the same cell).

The solution to the 1-dimensional case can be generalized to any number of dimensions (in the case of the IOI competition 2D, i.e., a NxN table). The trees are placed using the same logic as in the 1 dimensional case forming a tree of trees. In this case in the tree-like structure the cell at coordinate

(X, Y) contains the sum of an area which is determined by the number of zeroes in the binary representation of X in the X-direction and respectively the number of zeroes in the binary representation of Y in the Y-direction. The structure can then support queries of a sum of values in the rectangle [1, X]´[1, Y] in time $O((log N) ^2 )$ (for an P-dimensional case $O((log n) ^P ))$. The query for a rectangular shape can be expressed in terms of these basic queries (e.g. 4 queries in the 2 dimensional case: sum([L, R]´[B, T]) = sum([1, R]´[1, T]) - sum([1, L-1]´[1, T]) - sum([1, R]´[1, B-1]) +

sum([1, L-1]´[1, B-1])). (See Figure 4 for examples.) The example solution also optimizes this for small queries using the same method as the 1-dimensional case. The task also requires indexing to start at 0 and the binary indexed tree data structure requires indexing that starts at 1.
![image](./4366/file/jjNrgOicm9nv1977B6kj3.png)
![image](./4366/file/mWLGBKgN3_JvdqlHrMGFy.png)

### **Reference**

[1] P. M. Fenwick, A new data structure for cumulative frequency tables, *Software - Practice and Experience*24, 3 (1994), 327-336, 1994.

