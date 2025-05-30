## 题目描述


Little Lidia likes playing with numbers. Today she has a positive integer $n$ , and she wants to decompose it to the product of positive integers.

Because Lidia is little, she likes to play with numbers with little difference. So, all numbers in decomposition should differ by at most one. And of course, the product of all numbers in the decomposition must be equal to $n$ . She considers two decompositions the same if and only if they have the same number of integers and there is a permutation that transforms the first one to the second one.

Write a program that finds all decompositions, which little Lidia can play with today.



## 输入格式


The only line of the input contains a single integer $n (1 \le n \le 10^{18}).$



## 输出格式


In first line output the number of decompositions of $n$ , or $−1$ if this number is infinite. If number of decompositions is finite, print all of them one per line. In each line first print number $k_{i}$ of elements in decomposition. Then print $k_{i}$ integers in this decomposition in any order. Don't forget that decompositions which are different only in order of elements are considered the same.



## 题目大意
小刘烨喜欢玩数字，她有一个正整数$n$，她想把它分解成正整数的乘积，她喜欢玩没有什么区别的数字。因此，分解中的所有数字应该最多相差1，
而且，分解中所有数字的乘积必须等于$n$，她认为两个分解是相同的，当且仅当它们有相同数量的整数，并且有一个排列将第一个转化为第二个，写一个程序，找出小刘烨今天可以玩的所有的分解。

```input1
12

```

```output1
3
1 12
3 2 3 2
2 4 3

```

```input2
1

```

```output2
-1

```

## 提示
Time limit: 3 s, Memory limit: 512 MB. 

spj provider:@[shenyouran](/user/137367).

