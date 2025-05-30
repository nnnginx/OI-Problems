## 题目描述
To meet the ever-growing demands of his N (1 &amp;lt;= N &amp;lt;= 50,000) cows, Farmer John has bought them a new soda machine. He wants to figure out the perfect place to install the machine.

The field in which the cows graze can be represented as a one-dimensional number line. Cow i grazes in the range A\_i..B\_i (1 &amp;lt;= A\_i &amp;lt;= B\_i; A\_i &amp;lt;= B\_i &amp;lt;= 1,000,000,000) (a range that includes its endpoints), and FJ can place the soda machine at any integer point in the range 1..1,000,000,000.  Since cows are extremely lazy and try to move as little as possible, each cow would like to have the soda machine installed within her grazing range.

Sadly, it is not always possible to satisfy every cow's desires. Thus FJ would like to know the largest number of cows that can be satisfied.

To demonstrate the issue, consider four cows with grazing ranges 3..5, 4..8, 1..2, and 5..10; below is a schematic of their grazing ranges:

```cpp

         1   2   3   4   5   6   7   8   9  10  11  12  13
         |---|---|---|---|---|---|---|---|---|---|---|---|-...
                 aaaaaaaaa
                     bbbbbbbbbbbbbbbbb
         ccccc           ddddddddddddddddddddd
```
As can be seen, the first, second and fourth cows share the point 5, but the third cow's grazing range is disjoint.  Thus, a maximum of 3 cows can have the soda machine within their grazing range.


有N个人要去膜拜JZ，他们不知道JZ会出现在哪里，因此每个人有一个活动范围，只要JZ出现在这个范围内就能被膜拜，

伟大的JZ当然希望膜拜他的人越多越好，但是JZ不能分身，因此只能选择一个位置出现，他最多可以被多少人膜拜呢，

这个简单的问题JZ当然交给你了


## 输入格式
\* Line 1: A single integer: N

\* Lines 2..N+1: Line i+1 contains two space-separated integers: A\_i and B\_i


## 输出格式
\* Line 1: A single integer representing the largest number of cows whose grazing intervals can all contain the soda machine.


## 题目大意
**为了满足fj所有的N(1<=n<=50000)头奶牛的需求，fj新买了一台汽水机。他想找到一个最完美的位置来安放它。**

**奶牛的牧场可以被表示为一个一维数轴，第i个奶牛被放牧的区间是[Ai...Bi]（包含端点），fj可以把汽水机放在[1..1,000,000,000]。**

**因为奶牛们都懒得要死，她们想尽可能的少移动。她们希望汽水机被放在自己的放牧区间内。**

**遗憾的是，fj并不总能满足所有奶牛的要求，所以他想请你帮忙算出他能满足的奶牛数目**

```input1
4 
3 5 
4 8 
1 2 
5 10 

```

```output1
3 

```

## 提示
If the soda machine is placed at location 5, cows 1, 2, and 4 can be satisfied. It is impossible to satisfy all four cows.


