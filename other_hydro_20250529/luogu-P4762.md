## 题目描述
Viruses are usually bad for your health. How about fighting them with... other viruses? In this problem, you need to find out how to synthesize such good viruses.

We have prepared for you a set of strings of the letters $A, G, T$ and $C$. They correspond to the DNA nucleotide sequences of viruses that we want to synthesize, using the following operations:

   - Adding a nucleotide either to the beginning or the end of the existing sequence.
   - Replicating the sequence, reversing the copied piece, and gluing it either to the beginning or to the end of the original (so that e.g., $AGTC$ can become $AGTCCTGA$ or $CTGAAGTC$).

We’re concerned about efficiency, since we have very many such sequences, some of them very long. Find a way to synthesize them in a minimum number of operations.


## 输入格式
The first line of input contains the number of test cases $T$. The descriptions of the test cases follow:

Each test case consists of a single line containing a non-empty string. The string uses only the capital letters $A, C, G$ and $T$ and is not longer than $100 000$ characters.


## 输出格式
For each test case, output a single line containing the minimum total number of operations necessary to construct the given sequence.


## 题目大意
初始有一个空串，利用下面的操作构造给定串 $S$ 。   

1、串开头或末尾加一个字符   

2、串开头或末尾加一个该串的逆串   

求最小化操作数， $|S| \leq 10^5$，字符集为 $\{A,T,C,G\}$。  

Translated by  @wasa855 

```input1
4
AAAA
AGCTTGCA
AAGGGGAAGGGGAA
AAACAGTCCTGACAAAAAAAAAAAAC
```

```output1
3
8
6
18
```

