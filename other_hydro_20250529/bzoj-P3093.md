## 题目描述

Mr. B and Mr. M like to play with balls. They have many balls colored in blue and red. Firstly, Mr. B randomly picks up $n$ balls out of them and put them into a bag. Mr. M knows that there are $n+1$ possible situations in which the number of red balls is ranged from $0$ to $n$, and we assume the possibilities of the $n+1$ situations are the same. But Mr. M does not know which situation occurs. Secondly, Mr. M picks up $p$ balls out of the bag and examines them.

There are $q$ red balls and $p-q$ blue balls. The question is: if he picks up one more ball out of the bag, what is the possibility that this ball is red?

## 输入格式

Each test case contains only one line with three integers $n, p$ and $q$.

## 输出格式

For each test case, display a single line containing the case number and the possibility of the next ball Mr. M picks out is red. The number should be rounded to four decimal places.

```input1
3 0 0
4 2 1
```

```output1
Case 1: 0.5000 
Case 2: 0.5000
``` 

## 数据规模与约定

对于 $100\%$ 的数据，$2\le n\le 10^5$，$0\le p\le n-1$，$0\le q\le p$。

## 提示

[Explanation] 

For example as the sample test one, there are three balls in the bag. The possibilities of the four possible situations are all $0.25$. If there are no red balls in the bag, the possibility of the next ball are red is $0$. If there is one red ball in the bag, the possibility is $\frac{1}{3}$. If there are two red balls, the possibility is $\frac{2}{3}$. Finally if all balls are red, the possibility is $1$. So the answer is $0\times(\frac{1}{4})+(\frac{1}{3})\times(\frac{1}{4})+(\frac{2}{3})\times(\frac{1}{4})+1\times(\frac{1}{4})=0.5$.