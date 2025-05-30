## 题目描述
Farmer John's N (1 <= N <= 1000) cows each reside in one of B (1 <= B <= 20) barns which, of course, have limited capacity. Some cows really like their current barn, and some are not so happy.

FJ would like to rearrange the cows such that the cows are as equally happy as possible, even if that means all the cows hate their assigned barn.


Each cow gives FJ the order in which she prefers the barns.  A cow's happiness with a particular assignment is her ranking of her barn. Your job is to find an assignment of cows to barns such that no barn's capacity is exceeded and the size of the range (i.e., one more than the positive difference between the the highest-ranked barn chosen and that lowest-ranked barn chosen) of barn rankings the cows give their assigned barns is as small as possible.


## 输入格式
Line 1: Two space-separated integers, N and B


Lines 2..N+1: Each line contains B space-separated integers which are exactly 1..B sorted into some order. The first integer on line i+1 is the number of the cow i's top-choice barn, the second integer on that line is the number of the i'th cow's second-choice barn, and so on.


Line N+2: B space-separated integers, respectively the capacity of the first barn, then the capacity of the second, and so on. The sum of these numbers is guaranteed to be at least N.


## 输出格式
Line 1: One integer, the size of the minumum range of barn rankings the cows give their assigned barns, including the endpoints.


## 题目大意
有 $N$ 头牛，$B$ 个牛棚。告诉你每头牛心里牛棚的座次，即哪个牛棚他最喜欢，哪个第 $2$ 喜欢，哪个第 $3$ 喜欢，等等。但牛棚容量一定，所以每头牛分配到的牛棚在该牛心中的座次有高有低。现在求一种最公平的方法分配牛到牛棚，使所有牛中，所居牛棚的座次最高与最低的跨度最小。

```input1
6 4
1 2 3 4
2 3 1 4
4 2 3 1
3 1 2 4
1 3 4 2
1 4 2 3
2 1 3 2
```

```output1
2
```

## 提示
Explanation of the sample:




Each cow can be assigned to her first or second choice: barn 1 gets cows 1 and 5, barn 2 gets cow 2, barn 3 gets cow 4, and barn 4 gets cows 3 and 6.


