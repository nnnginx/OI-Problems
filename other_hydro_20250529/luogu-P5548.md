## 题目背景
韵要怎么押？棋要怎么下？敌要怎么杀？旗要怎么插？

## 题目描述
现在你想要写一首歌词，一共有 $nd$ 个字，你一共设计了 $k$ 种韵脚，每个字恰好要符合一种韵脚。  

并且只有当每种韵脚在歌词中出现的字数恰为 $d$ 的倍数时，这首歌才好听。

试问一共有多少种韵脚的搭配方法，使得歌词好听？

你只需要回答方案数对于 $1049874433$ 取模的结果即可。

## 输入格式
一行三个整数 $n,k,d$，如题意所示。

## 输出格式
一行一个整数，表示答案。

```input1
2 2 2
```

```output1
8
```

```input2
2 3 4
```

```output2
213
```

```input3
2 4 6
```

```output3
5548
```

## 提示
对于 $100\%$ 的数据，保证：  
$0 \le n \le 10^9$  
$1\le k \le 2000$  
$d\in \{ 1,2,3,4,6 \}$

By：EntropyIncreaser

