## 题目描述

The well-known Fibonacci sequence is defined as following：  
Here we regard $n$ as the index of the Fibonacci number $F(n)$．  
This sequence has been studied since the publication of Fibonacci's book Liber Abaci．So far，many properties of this sequence have been introduced．  
You had been interested in this sequence，while after reading lots of papers about it．You think there’s no need to research in it anymore because of the lack of its unrevealed properties．Yesterday，you decided to study some other sequences like Lucas sequence instead．  
Fibonacci came into your dream last night．＂Stupid human beings．Lots of important properties of Fibonacci sequence have not been studied by anyone，for example，from the Fibonacci number $347746739\dots$＂．  
You woke up and couldn’t remember the whole number except the first few digits Fibonacci told you．You decided to write a program to find this number out in order to continue your research on Fibonacci sequence．

输入一串数字，判断为第几个fib数的前缀，如有多个输出最前面的，不存在或者大于等于 $1 \times 10^5$ 输出 `-1`。

## 输入格式

There are multiple test cases．The first line of input contains a single integer $T$ denoting the number of test cases．  
For each test case，there is a single line containing one non-empty string made up of at most $40$ digits．And there won’t be any unnecessary leading zeroes．

## 输出格式

For each test case，output the smallest index of the smallest Fibonacci number whose decimal notation begins with the given digits．If no Fibonacci number with index smaller than $1 \times 10^5$ satisfy that condition，output `-1` instead – you think what Fibonacci wants to told you beyonds your ability．

```input1
15
1
12
123
1234
12345
9
98
987
9876
98765
89
32
51075176167176176176
347746739
5610
```

```output1
Case #1: 0
Case #2: 25
Case #3: 226
Case #4: 1628
Case #5: 49516
Case #6: 15
Case #7: 15
Case #8: 15
Case #9: 43764
Case #10: 49750
Case #11: 10
Case #12: 51
Case #13: -1
Case #14: 1233
Case #15: 22374
```

## 数据规模与约定

$100\%$ 的数据满足：$T \le 5 \times 10^4$。

## 题目来源

Acm 2011 上海
