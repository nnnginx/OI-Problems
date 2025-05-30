## 题目描述
The cows, who always have an inferiority complex about their intelligence, have a new guessing game to sharpen their brains.

A designated 'Hay Cow' hides behind the barn and creates N (1 ≤ N ≤ 1,000,000) uniquely-sized stacks (conveniently numbered 1..N) of hay bales, each with 1..1,000,000,000 bales of hay.

The other cows then ask the Hay Cow a series of Q (1 ≤ Q ≤ 25,000) questions about the the stacks, all having the same form:

What is the smallest number of bales of any stack in the range of stack numbers Ql..Qh (1 ≤ Ql ≤ N; Ql ≤ Qh ≤ N)?The Hay Cow answers each of these queries with a single integer A whose truthfulness is not guaranteed.

Help the other cows determine if the answers given by the Hay Cow are self-consistent or if certain answers contradict others.



## 输入格式
\* Line 1: Two space-separated integers: N and Q

\* Lines 2..Q+1: Each line contains three space-separated integers that represent a single query and its reply: Ql, Qh, and A


## 输出格式
\* Line 1: Print the single integer 0 if there are no inconsistencies among the replies (i.e., if there exists a valid realization of the hay stacks that agrees with all Q queries). Otherwise, print the index from 1..Q of the earliest query whose answer is inconsistent with the answers to the queries before it.


## 题目大意
给一个长度为 $n$ 的数组 $q$ 个条件，数组中的数字互不相同，每个条件格式形如  $l_i,r_i,x_i$ 表示这个数组的区间 $[l_i,r_i]$ 内的最小值为  $x_i$，输出最早与前面的条件有矛盾的条件的编号，如果所有条件都不发生矛盾，输出 $0$。

### 输入格式

第一行两个整数，分别是  $n$ 和  $q$。

第二行至第 $q+1$ 行，每行三个整 $l_i,r_i,x_i$ 描述一个条件。

### 输出格式

仅一个整数，表示最早发生矛盾的条件的编号。如果所有条件都没有发生矛盾，输出 $0$。

```input1
20 4
1 10 7
5 19 7
3 12 8
11 15 12

```

```output1
3

```

