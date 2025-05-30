## 题目描述
Farmer John wants to save some blocks of his cows' delicious Wisconsin cheese varieties in his cellar for the coming winter. He has room for one tower of cheese in his cellar, and that tower's height can be at most T (1 <= T <= 1,000). The cows have provided him with a virtually unlimited number of blocks of each kind of N (1 <= N <= 100) different types of cheese (conveniently numbered 1..N). He'd like to store (subject to the constraints of height) the most

valuable set of blocks he possibly can. The cows will sell the rest to support the orphan calves association.

Each block of the i-th type of cheese has some value V\_i (1 <= V\_i <= 1,000,000) and some height H\_i (5 <= H\_i <= T), which is always a multiple of 5.

Cheese compresses. A block of cheese that has height greater than or equal to K (1 <= K <= T) is considered 'large' and will crush any and all of the cheese blocks (even other large ones) located below it in the tower. A crushed block of cheese doesn't lose any value, but its height reduces to just 4/5 of its old height. Because the height of a block of cheese is always a multiple of 5, the height of a crushed block of cheese will always be an integer. A block of cheese is either crushed or not crushed; having multiple large blocks above it does not crush it more. Only tall blocks of cheese crush other blocks; aggregate height of a tower does not affect whether a block is crushed or not.

What is the total value of the best cheese tower FJ can construct?

Consider, for example, a cheese tower whose maximum height can be 53 to be build from three types of cheese blocks. Large blocks are those that are greater than or equal to 25. Below is a chart of the values and heights of the various cheese blocks he stacks:

Type    Value      Height 

1      100         25

2       20          5

3       40         10

FJ constructs the following tower: 

Type Height Value 

top -> [1]   25    100

```cpp
[2]    4     20   <- crushed by [1] above 
[3]    8     40   <- crushed by [1] above 
[3]    8     40   <- crushed by [1] above 
bottom -> [3]    8     40   <- crushed by [1] above 
```
The topmost cheese block is so large that the blocks below it are crushed. The total height is:
```cpp
25 + 4 + 8 + 8 + 8 = 53 
The total height does not exceed 53 and thus is 'legal'. The total value is: 
100 + 20 + 40 + 40 + 40 = 240. 
This is the best tower for this particular set of cheese blocks. 
要建一个奶酪塔，高度最大为T。他有N块奶酪。第i块高度为Hi（一定是5的倍数），价值为Vi。一块高度>=K的奶酪被称为大奶酪，一个奶酪如果在它上方有大奶酪（多块只算一次），它的高度就会变成原来的4/5.。 很显然John想让他的奶酪他价值和最大。求这个最大值。
```

## 输入格式
\* Line 1: Three space-separated integers: N, T, and K

\* Lines 2..N+1: Line i+1 contains two space separated integers: V\_i and H\_i


## 输出格式
\* Line 1: The value of the best tower FJ can build


## 题目大意
**【题目描述】**

FJ 要建一个奶酪塔，高度最大为 $T\ (1 \le T \le 10^3)$ 。他有 $N\ (1 \le N \le 10^2)$ 种奶酪。第 $i$ 种奶酪的高度为 $H_i\ (5\le H_i \le T\text{ 且 }5 \mid H_i)$ ，价值为 $V_i\ (1 \le V_i \le 10^6)$ 。一块高度 $H_i\ge K\ (1 \le K \le T)$ 的奶酪被称为大奶酪，如果一个奶酪上方有大奶酪（如果有多块就只算一次），这个奶酪的高度 $H_i$ 就会变成原来的 $\frac{4}{5}$。FJ 想让他的奶酪塔价值和最大。请你求出这个最大值。

例如，考虑一种奶酪塔，其最大高度可以是 $53$，可以用三种类型的奶酪块建造。大块是大于或等于 $25$ 的块。下面是他堆叠的各种奶酪块的值和高度的图表：

|类型|价值|高度|
| :----------: | :----------: | :----------: |
|1|100|25|
|2|20|5|
|3|40|10|

FJ建造了以下奶酪塔：

|类型|价值|高度|
| :----------: | :----------: | :----------: |
|1|100|25|
|2|20|4|
|3|40|8|
|3|40|8|
|3|40|8|

总高度是 $25 + 4 + 8 + 8 + 8 = 53$，除塔顶奶酪外，其余高度均被压低。总价值是 $100 + 20 + 40 + 40 + 40 = 240$。

**【输入格式】**

第1行为三个用空格隔开的整数 $N,T,K$。

第2至 $N+1$ 行中第 $i+1$ 行包含两个用空格隔开的整数 $V_i,H_i$。

**【输出格式】**

一行一个整数为奶酪塔的最大价值。

```input1
3 53 25 
100 25 
20 5 
40 10 

```

```output1
240 

```

