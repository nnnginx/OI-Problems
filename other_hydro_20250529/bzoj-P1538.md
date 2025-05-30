## 题目描述

King Byteasar has decided to throw two great parties and wants to invite to them every single Byteotian inhabitant. Of course he wants to invite each of them to exactly one of the parties. The king knows from his own vast experience that a person is having a good time when there is an even number of her/his friends at the party. Thus he has asked you to divide the country's inhabitants between two parties in a way that as many people as possible have an even number of friends at their party. A trivial division, i.e. one that leaves one party with no guests invited, is allowed. The acquaintanceship is a symmetric relation, i.e. whenever a person $A$ knows the person $B$, the person $B$ also knows the person $A$.

拜占庭国王要举办两个大派对，并且希望邀请更多的居民，国王从他的丰富经验里知道，如果一个居民在派对上能遇到偶数个的朋友，那他会非常高兴。因此，他要求你邀请国家的居民去两个派对（注：就是说把居民分到两个派对上），而使尽可能多的人在他们的聚会上有偶数个的朋友，允许一小部分人没有参加派对。认识是一种对称关系，如 $A$ 认识 $B$，那么 $B$ 也认识 $A$。

TaskWrite a programme that:

reads from the standard input the number of Byteotia's inhabitants and the description of their acquaintances,splits the inhabitants into two parties in such way that the number of people who have an even number of friends at their party is as large as possible,writes to the standard output a list of people who should be invited to the first party.

你的任务是编写一个程序：

从标准输入流中读取居民的数量和各个居民的朋友，把居民划分入两个派对，并且尽量使一个居民在派对上的朋友数更多

## 输入格式

In the first line of the standard input there is one integer $N$ ($1\le N\le 200$) - it is the number of inhabitants of Byteotia. The inhabitants are numbered from $1$ to $N$. In the following $N$ lines there are the descriptions of subsequent persons' acquaintances. At the beginning of the $(i+1)$'th line there is an integer $l_i$ ($0\le l_i\le N-1$) - the number of friends of the ith inhabitant. It is followed by $l_i$ pairwise distinct numbers of the $i$'th inhabitant's friends. We assume that no inhabitant is her/his own friend. It follows that each acquaintance is written twice: if $A$ and $B$ know each other, then $B$ appears on $A$'s list of friends and $A$ appears on $B$'s.

输入共 $N+1$ 行在第一行读入一个整数 $N$ - 表示居民的数量，接下来 $N$ 行，第 $i+1$ 行是一个整数 $l_i$，表示第 $i$ 个居民的朋友数量，接着是 $l_i$ 个数，为第 $i$ 个居民的朋友编号。我们假设没有人是自己的朋友。如果 $B$ 出现在了 $A$ 的朋友列表中，那么 $A$ 也会出现在 $B$ 的培养列表中。

## 输出格式

In the first line of the standard output your programme should write one integer $M$ - the number of people who are to come to the first party. In the second line the $M$ numbers of these people should be written. The rest shall come to the second party.

There are many correct divisions in this task - your programme should write any one of them.

第一行是一个整数 $M$，是前往第一个排队的人数。第二行 $M$ 个整数，是去第一个派对的居民编号，其余的居民前往第二个派对。

有很多种答案，你只需要输出一个。

## 输入样例
```plain
5
3 2 3 4
2 1 3
4 2 1 4 5
2 1 3
1 3
```

## 输出样例
```plain
3
1 2 3
```

## 数据规模及约定

对于  $100 \%$ 的数据 ：$1\le N\le 200$。
