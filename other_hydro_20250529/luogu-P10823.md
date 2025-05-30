## 题目描述
Prof. Pang has only $1$ Au in his pocket. (Yes, Prof. Pang is from Austan and he uses the currency Au there.)

He will make use of a balloon store and a candy store to make money: In the balloon store, Prof. Pang can buy $k_{ab}$ balloons for the price of $1$ Au or buy $k_{cb}$ balloons for the price of $1$ candy. In the candy store, Prof. Pang can buy $k_{ac}$ candies for the price of $1$ Au or buy $k_{bc}$ candies for the price of $1$ balloon. Prof. Pang can also sell one balloon and get $k_{ba}$ Aus. He can sell one candy and get $k_{ca}$ Aus. The only constraint to him is that there are only $n_b$ balloons in the balloon store and only $n_c$ candies in the candy store. He can buy balloons and candies only when supplies last. Even if he sells some of his balloons or candies, the number of balloons and candies in the stores will not increase.

Each of the six transactions can be performed in any order for any times ($0$ or more) but they are not separable (for example, Prof. Pang can not buy $k_{ab}/2$ balloons for the price of $1/2$ Au).

Please find out how many Aus he can make at most.

## 输入格式
The first line contains a single integer $T$ ($1\le T\le 1000$) denoting the number of test cases.

Each of the next $T$ lines contains eight integers $n_b$, $n_c$, $k_{ab}$, $k_{ba}$, $k_{ac}$, $k_{ca}$, $k_{bc}$, $k_{cb}$ ($1\le n_b, n_c\le 10^9$, $1\le k_{ab}, k_{ba}, k_{ac}, k_{ca}, k_{bc}, k_{cb}\le 100$) separated by single spaces.

## 输出格式
For each test case, print one line containing the answer.

```input1
6
2 2 2 2 2 2 2 2
78 74 5 3 10 2 4 7
31 75 3 6 6 1 8 4
91 86 4 2 9 5 8 5
48 89 3 9 2 3 5 7
13 25 5 7 6 1 2 4
```

```output1
7
355
239
571
637
109
```

## 提示
In the first example, Prof. Pang buys $2$ balloons with $1$ Au and then sells $2$ balloons and gets $4$ Aus. Then he buys $2$ candies with $1$ Au, sells $2$ candies and gets $4$ Aus.


