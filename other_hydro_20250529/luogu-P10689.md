## 题目描述
Your friend, Jackson is invited to a TV show called SuperMemo in which the participant is told to play a memorizing game. At first, the host tells the participant a sequence of numbers, $A_1, A_2, \ldots A_n$. Then the host performs a series of operations and queries on the sequence which consists:

  * `ADD x y D`: Add $D$ to each number in sub-sequence $A_x \ldots A_y$. For example, performing "ADD 2 4 1" on $1, 2, 3, 4, 5$ results in $1, 3, 4, 5, 5$
  * `REVERSE x y`: reverse the sub-sequence ${A_x \ldots A_y}$. For example, performing "REVERSE 2 4" on $1, 2, 3, 4, 5$ results in $1, 4, 3, 2, 5$
  * `REVOLVE x y T`: rotate sub-sequence ${A_x \ldots A_y}$ $T$ times. For example, performing "REVOLVE 2 4 2" on $1, 2, 3, 4, 5$ results in $1, 3, 4, 2, 5$
  * `INSERT x P`: insert $P$ after $A_x$. For example, performing "INSERT 2 4" on $1, 2, 3, 4, 5$ results in $1, 2, 4, 3, 4, 5$
  * `DELETE x`: delete $A_x$. For example, performing "DELETE 2" on $1, 2, 3, 4, 5$ results in $1, 3, 4, 5$
  * `MIN x y`: query the participant what is the minimum number in sub-sequence $A_x \ldots A_y$. For example, the correct answer to "MIN 2 4" on $1, 2, 3, 4, 5$ is $2$

To make the show more interesting, the participant is granted a chance to turn to someone else that means when Jackson feels difficult in answering a query he may call you for help. You task is to watch the TV show and write a program giving the correct answer to each query in order to assist Jackson whenever he calls.

## 输入格式
The first line contains $n$ ($n \leq 100000$).

The following $n$ lines describe the sequence.

Then follows $M$ ($M \leq 100000$), the numbers of operations and queries.

The following $M$ lines describe the operations and queries. 

## 输出格式
For each "MIN" query, output the correct answer.

```input1
5
1
2
3
4
5
2
ADD 2 4 1
MIN 4 5
```

```output1
5
```

