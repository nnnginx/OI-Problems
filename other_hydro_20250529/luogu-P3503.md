## 题目描述
    Bytie has got a set of wooden blocks for his birthday.

The blocks are indistinguishable from one another, as they are all cubes of the same size.

    Bytie forms piles by putting one block atop another.

Soon he had a whole rank of such piles, one next to another in a straight line.

Of course, the piles can have different heights.

Bytie's father, Byteasar, gave his son a puzzle.

He gave him a number ![](http://main.edu.pl/images/OI17/klo-en-tex.1.png) and asked to rearrange the blocks in such a way that    the number of successive piles of height at least ![](http://main.edu.pl/images/OI17/klo-en-tex.2.png) is maximised.

However, Bytie is only ever allowed to pick the top block from a pile strictly    higher than ![](http://main.edu.pl/images/OI17/klo-en-tex.3.png) and place it atop one of the piles next to it.

Further, Bytie is not allowed to form new piles, he can only move blocks    between those already existing.



## 输入格式
In the first line of the standard input there are two integers separated by a single space:

![](http://main.edu.pl/images/OI17/klo-en-tex.4.png) (![](http://main.edu.pl/images/OI17/klo-en-tex.5.png)), denoting the number of piles, and ![](http://main.edu.pl/images/OI17/klo-en-tex.6.png) (![](http://main.edu.pl/images/OI17/klo-en-tex.7.png)),      denoting the number of Byteasar's requests.

The piles are numbered from ![](http://main.edu.pl/images/OI17/klo-en-tex.8.png) to ![](http://main.edu.pl/images/OI17/klo-en-tex.9.png).

In the second line there are ![](http://main.edu.pl/images/OI17/klo-en-tex.10.png) integers ![](http://main.edu.pl/images/OI17/klo-en-tex.11.png)      separated by single spaces (![](http://main.edu.pl/images/OI17/klo-en-tex.12.png)).

The number ![](http://main.edu.pl/images/OI17/klo-en-tex.13.png) denotes the height of the ![](http://main.edu.pl/images/OI17/klo-en-tex.14.png)-th pile.

The third line holds ![](http://main.edu.pl…


## 输出格式
Your program should print out ![](http://main.edu.pl/images/OI17/klo-en-tex.21.png) integers, separated by single spaces,      to the standard output - the ![](http://main.edu.pl/images/OI17/klo-en-tex.22.png)-th of which should be the answer to the puzzle      for the given initial piles set-up and the parameter ![](http://main.edu.pl/images/OI17/klo-en-tex.23.png).


## 题目大意
给出 $n$ 个正整数 $a_1,a_2,\cdots,a_n$，再给出一个正整数 $k$，现在可以进行如下操作：

- 每次选择一个大于 $k$ 的正整数 $a_i$，将 $a_i$ 减去 $1$ ，选择 $a_{i-1}$ 或 $a_{i+1}$ 中的一个加上 $1$。

经过一定次数的操作后，问最大能够选出多长的一个连续子序列，使得这个子序列的每个数都不小于 $k$。$m$ 组询问。

```input1
5 6
1 2 1 1 5
1 2 3 4 5 6
```

```output1
5 5 2 1 1 0
```

## 提示
$1\le n\le 10^6$，$1\le m\le 50$，$1\le a_i,k\le 10^9$


