## 题目描述
Every morning when they are milked, the Farmer John's cows form a rectangular grid that is $R (1 \leq R \leq 10,000)$ rows by $C (1 \leq C \leq 75)$ columns. As we all know, Farmer John is quite the expert on cow behavior, and is currently writing a book about feeding behavior in cows. He notices that if each cow is labeled with an uppercase letter indicating its breed, the two-dimensional pattern formed by his cows during milking sometimes seems to be made from smaller repeating rectangular patterns.

Help FJ find the rectangular unit of smallest area that can be repetitively tiled to make up the entire milking grid. Note that the dimensions of the small rectangular unit do not necessarily need to divide evenly the dimensions of the entire milking grid, as indicated in the sample input below.

## 输入格式
- Line $1$: Two space-separated integers: $R$ and $C$

- Lines $2\dots R+1$: The grid that the cows form, with an uppercase letter denoting each cow's breed. Each of the $R$ input lines has $C$ characters with no space or other intervening character.

## 输出格式
- Line 1: The area of the smallest unit from which the grid is formed

## 题目大意
**【题目描述】**

每天早上挤奶时，农夫约翰的奶牛们排成一个 $R (1 \leq R \leq 10,000)$ 行乘 $C (1 \leq C \leq 75)$ 列的矩形网格。众所周知，约翰农夫是一个相当擅长牛行为的专家，目前正在撰写一本关于奶牛饲养行为的书。他注意到，如果每头奶牛都标有一个表示其品种的大写字母，那么奶牛在挤奶时形成的二维图案有时似乎是由更小的重复矩形图案组成的。

帮助约翰农夫找到可以重复铺设以组成整个挤奶网格的最小面积的矩形单元。请注意，小矩形单元的尺寸不一定需要完全整除整个挤奶网格的尺寸，如下面的示例输入所示。

**【输入格式】**

- 第一行：两个用空格分隔的整数：$R$ 和 $C$
- 第 $2\dots R+1$ 行：奶牛形成的网格，每个奶牛的品种用大写字母表示。每个 $R$ 输入行有 $C$ 个字符，没有空格或其他间隔字符。

**【输出格式】**

第一行：形成网格的最小单位的面积

**【提示说明】**

整个挤奶网格可以由图案 AB 的重复构建。

翻译来自于：ChatGPT。

```input1
2 5 
ABABA 
ABABA

```

```output1
2
```

## 提示
The entire milking grid can be constructed from repetitions of the pattern `AB`.

