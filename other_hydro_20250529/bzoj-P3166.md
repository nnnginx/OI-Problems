## 题目描述
Welcome to ALO (Arithmetic and Logistic Online)。这是一个 VR MMORPG，如名字所见，到处充满了数学的谜题。

现在你拥有 $n$ 颗宝石，每颗宝石有一个能量密度，记为 $a_i$，这些宝石的能量 密度两两不同。现在你可以选取连续的一些宝石（必须多于一个）进行融合，设为 $a_i,a_{i+1},\cdots,a_j$，则融合而成的宝石的能量密度为这些宝石中能量密度的次大值与其他任意一颗宝石的能量密度按位异或的值，即，设该段宝石能量密度次大值为 $k$，则生成的宝石的能量密度为 $\max_{p=i}^{j}{k \oplus a_p | a_p \neq k }$。

现在你需要知道你怎么选取需要融合的宝石，才能使生成的宝石能量密度最大。

## 输入格式
第一行，一个整数 $n$，表示宝石个数。

第二行，$n$ 个整数，分别表示 $a_1$ 至 $a_n$，表示每颗宝石的能量密度，保证对于 $i \neq j$ 有 $a_i \neq a_j$。
## 输出格式
输出一行一个整数，表示最大能生成的宝石能量密度。

```input1
5
9 2 1 4 7
```
```output1
14
```

## 样例解释
选择区间 $[1,5]$，最大值为 $7 \oplus 9$

## 数据规模与约定
对于 $100\%$ 的数据有 $1 \le n \le 5\times 10^4, 0 \le ai \le 10^9$

## 题目来源
加强型数据By Hta