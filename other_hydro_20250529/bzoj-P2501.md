## 题目描述

To meet the ever-growing demands of his $N (1 \le N \le 5 \times 10^4)$ cows,Farmer John has bought them a new soda machine. He wants to figure out the perfect place to install the machine.

The field in which the cows graze can be represented as a one-dimensional
number line. Cow i grazes in the range $A_i..B_i$( $1 \le A_i \le B_i,A_i \le B_i \le 1 \times 10^9$ ) (a range that includes its endpoints),
and FJ can place the soda machine at any integer point in the range$1 \times 10^9$ . Since cows are extremely lazy and try to moveas little as possible, each cow would like to have the soda machineinstalled within her grazing range.
Sadly, it is not always possible to satisfy every cow's desires.Thus FJ would like to know the largest number of cows that can besatisfied.
To demonstrate the issue, consider four cows with grazing ranges
$3..5, 4..8, 1..2$ and $5..10$ ; below is a schematic of their grazing
ranges:

```
1   2   3   4   5   6   7   8   9  10  11  12  13
|---|---|---|---|---|---|---|---|---|---|---|---|-...
aaaaaaaaa
bbbbbbbbbbbbbbbbb
ccccc           ddddddddddddddddddddd
```

As can be seen, the first, second and fourth cows share the point $5$ ,but the third cow's grazing range is disjoint. Thus, a maximum of $3$ cows can have the soda machine within their grazing range.

有 $N$ 个人要去膜拜 JZ ，他们不知道 JZ 会出现在哪里，因此每个人有一个活动范围，只要 JZ 出现在这个范围内就能被膜拜，伟大的 JZ 当然希望膜拜他的人越多越好，但是 JZ 不能分身，因此只能选择一个位置出现，他最多可以被多少人膜拜呢？

这个简单的问题 JZ 当然交给你了。

## 输入格式

 
Line $1$ : $A$ single integer: $N$ 。

Lines $2..N+1$ : Line $i+1$ contains two space-separated integers: $A_i$
and $B_i$

## 输出格式

Line $1$ : A single integer representing the largest number of cows
whose grazing intervals can all contain the soda machine.

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

If the soda machine is placed at location $5$ , cows  $1, 2$ , and $4$ can be
satisfied. It is impossible to satisfy all four cows.

## 题目来源

Gold

