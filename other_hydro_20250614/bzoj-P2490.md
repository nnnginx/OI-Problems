## 题目描述

Some brave warriors come to a lost village．They are very lucky and find a lot of treasures and a big treasure chest，but with angry zombies．  
The warriors are so brave that they decide to defeat the zombies and then bring all the treasures back．A brutal long-drawn-out battle lasts from morning to night and the warriors find the zombies are undead and invincible．  
Of course，the treasures should not be left here．Unfortunately，the warriors cannot carry all the treasures by  the treasure chest due to the limitation of the capacity of the chest．Indeed，there are only two types of treasures：emerald and sapphire．All of the emeralds are equal in size and value，and with infinite quantities．So are sapphires．  
Being the priest of the warriors with the magic artifact：computer，and given the size of the chest，the value and size of each types of gem，you should compute the maximum value of treasures our warriors could bring back．

## 输入格式

There are multiple test cases．The number of test cases $T$ is given in the first line of the input file．For each test case，there is  only one line containing five integers $N,S_1,V_1,S_2,V_2$，denoting the size of the treasure chest is $N$ and the size and value of an emerald is $S_1$ and $V_1$，size and value of a sapphire is $S_2,V_2$．All integers are positive and fit in 32-bit signed integers．

有两种宝石和一个箱子，宝石有体积 $S$ 和价值 $V$，箱子有容量 $N$，求怎样使箱子中的宝石价值最大（所有数据是正数且范围在32位有符号正数范围内）。

## 输出格式

For each test case，output a single line containing the case number and the maximum total value of all items that the warriors can carry with the chest．

```input1
2
100 1 1 2 2
100 34 34 5 3
```

```output1
Case #1: 100
Case #2: 86
```

## 数据规模与约定

$100\%$ 的数据满足：$T \le 200$。

## 题目来源

Acm 2011 上海


