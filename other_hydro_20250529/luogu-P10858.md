## 题目描述
In Minecraft, there are three dimensions in the simple world, one of which is known as “The End”. In this dimension, the Ender Dragon is usually symbolized as the final boss of Minecraft.

![](https://cdn.luogu.com.cn/upload/image_hosting/hsvxefjr.png)

Now we, you, and Steve want to beat the dragon. However, we find that the dragon is telling a puzzle. We must solve it before fighting against the dragon. Please stand by our side to fight against the dragon. The puzzle goes as follows.

Given two positive integers $x$ and $y$, please find two integers $a$ and $b$, such that

$$\sqrt{\dfrac{\operatorname{lcm}(x,y)}{\gcd(x,y)}}=a\sqrt{b}$$

and to maximize $a \cdot b$.

Here, $\gcd(a, b)$ represents the greatest common divisor of $a, b$, while $\operatorname{lcm}(a, b)$ represents the least common multiple of $a, b$.

## 输入格式
The first line contains an integer $T (1 \leq T \leq 10^4)$ indicating the number of test cases.

Of the following $T$ lines, each contains two integers $x$ and $y (1 \leq x, y \leq 10^9)$, representing the puzzle.

## 输出格式
Output $T$ lines. Each contains two integers $a$ and $b$, indicating the answer to each test case.

## 题目大意
### 题目描述
在 Minecraft 中，简单世界中有三个维度，其中一个被称为“The End”。在这个维度中，末影龙通常被象征为 Minecraft 的最终 Boss。

现在，我们、你和Steve想要打败这条龙。然而，我们发现这条龙出了一道谜题来困扰我们。在与龙战斗之前，我们必须先解开这个谜题。请站在我们这边，与龙一同战斗。谜题如下：

给定两个正整数 $x$ 和 $y$，请找到两个整数 $a$ 和 $b$，使得

$$\sqrt{\dfrac{\operatorname{lcm}(x,y)}{\gcd(x,y)}}=a\sqrt{b}$$

并使 $a \cdot b$ 最大化。

其中，$\gcd(a, b)$ 表示 $a$ 和 $b$ 的最大公约数，而 $\operatorname{lcm}(a, b)$ 表示 $a$ 和 $b$ 的最小公倍数。

### 输入格式

第一行包含一个整数 $T \ (1 \leq T \leq 10^4)$，表示测试用例的数量。

接下来的 $T$ 行中，每行包含两个整数 $x$ 和 $y \ (1 \leq x, y \leq 10^9)$，表示这个谜题。

### 输出格式

输出 $T$ 行，每行包含两个整数 $a$ 和 $b$，表示每个测试用例的答案。

### 说明/提示
亲爱的所有参赛者：

这个问题可能是故事的开篇，但绝不是故事的结尾。请一直相信自己，愿我的歌声伴随你们，“致我们曾一起翻越的高山，与你并肩战斗巨龙的时光，我度过了生命中最美好的时光”。

翻译者：[Immunoglobules](https://www.luogu.com.cn/user/1066251)

```input1
2
1 1
4 4
```

```output1
1 1
1 1
```

## 提示
Dear all participants:

This problem may be the very first page, but not where the story line ends. Please believe in yourself all the time, wishing you with my singing, “Long live all the mountains we moved, I had the time of my life fighting dragons with you”.

