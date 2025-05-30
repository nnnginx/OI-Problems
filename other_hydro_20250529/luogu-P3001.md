## 题目描述
Bessie is studying her favorite subject, Macroeconomics, in cowllege. For her final project, she will be presenting research on exchange rates between countries around the world.


In order to make her presentation more lively, she would like to show the relative prices of Big Macs around the world, despite their rather unsavory contents. To illustrate, suppose that Bessie would like to find smallest value of a Big Mac in a country given its value in some initial country and exchange rates from which other country's values can be calculated (as illustrated below):




```cpp
* A Big Mac is worth 60 dollars in the United States 
* The exchange rate from US dollars to Canadian dollars is 0.2 Canadian dollars per US dollar 
* The exchange rate from US dollars to British Pounds is 5.00 British Pounds per US Dollar 
* The exchange rate from British Pounds to Canadian dollars is 0.5 Canadian dollars per British Pound 
* The exchange rate between Canadian dollars to US dollars is 5.00 US dollars per Canadian dollar and Bessie would like to find the smallest possible value of a Big Mac in Canada that can be obtained by exchanging currencies. There are two ways: 
* Going from US dollars directly to Canada dollars would yield a burger worth 60.00 US dollars * 0.2 Canadian dollars / US dollar = 12.00 Canadian dollars 
* Going from US dollars to British Pounds to Canadian dollars would yield a burger worth 60.00 US$ * 5.00 GBP / 1 US$ * 0.5 C$ / 1 GBP = 150.00 C$ (Canadian dollars). 
```
Bessie would choose the former option, since she would much rather pay 12.00 Canadian dollars instead of 150.00 Canadian dollars for a Big Mac in Canada. 

Bessie has N (1 <= N <= 2,000) countries conveniently labeled 1 to N that she would like to consider along with a list of M (1 <= M <= 25,000) exchange rates e_ij (0.1 < e_ij <= 10), each between countries i and j (1 <= i <= N; 1 <= j <= N). 

Given the value V (1 <= V <= 1,000,000,000,000), which is not necessarily an integer, of the Big Mac in her starting country A (1 <= A <= N), help her find the smallest possible value of a Big Mac in country B (1 <= B <= N; B != A) after a series of currency conversions. If there is no minimum, output 0. 

It is guaranteed that the answer is, if not 0, between 1 and 10^15.

It is also guaranteed that, for any country's currency, it is possible to get to any other country's currency.





## 输入格式
Line 1: Five space-separated numbers: N, M, V, A, B

Lines 2..M+1: Three space-separated numbers: i, j, e\_ij


## 输出格式
Line 1: A single positive number, the price of the Big Mac, with absolute or relative error at most 10^-6. If there is no minimum, output 0.

## 题目大意
### 题目描述

Bessie 正在学习她最喜欢的科目宏观经济学，作为她最后一门学科，她将对世界各种货币的汇率进行研究。

为了让她的演讲更加生动，她会展示一个叫做 BM 的商品在全世界的相对价格。举个例子，Bessie 会通过其他国家的汇率去找到一件 BM 在一个国家的最小价值。

- 一件 BM 在美国值 $60$ 美元；
- 美元与加拿大元的汇率为 $1$ 美元换 $0.2$ 加拿大元（$1:0.2$）。
- 美元与英镑的汇率为 $1$ 美元换 $5$ 英镑（$1:5$）。
- 英镑与加拿大元的汇率为 $1$ 英镑换 $0.5$ 加拿大元（$1:0.5$）。
- 加拿大元与美元的汇率是 $5$ 美元换一加拿大元（$5:1$），Bessie 有两种方法通过货币兑换在加拿大这个国家找到一件 BM 的最低价值：

1. 拿着美元直接去加拿大，通过汇率得出一件 BM 只要 $12$ 加拿大元；
2. 拿着美元去英国，兑换为英镑后再去加拿大，得出一件 BM 要 $150$ 加拿大元。

Bessie 会选择前一种方案因为她更乐意为在加拿大买一件 BM 支付 $12$ 加元而不是 $150$ 加元。

Bessie 有 $N(1\leq N\leq 2000)$ 个国家的信息和 $M(1\leq M\leq25000)$ 种汇率，在 $i,j$ 国间的汇率表示为 $e_{ij}(0.1\leq e_{ij}\leq 10)$。

给你一个值 $V(1\leq V\leq 10^{12})$，$V$ 不一定是一个整数。$V$ 是 BM 在起始国家 A 的价格，帮助 Bessie 寻找到在 B 国 BM 最低的价格，如果不存在，则输出 $0$。

据保证答案小于 $10^{15}$，也保证所有国家都可以通过汇率将钱币转为别的国家的。

### 输入格式

第 $1$ 行：五个数：$N,M,V,A,B$，分别一个空格隔开。

第 $2$ 到 $M+1$ 行：三个数 $i,j,e_{ij}$，分别一个空格隔开。

### 输出格式

一行：BM 在 B 国的最低价格，精确到 $10^{-6}$。如果没有最小值，输出 $0$。

**注意，本题的汇率是单向的**。

感谢 @JJYZ\_cbh 的耐心翻译


```input1
3 4 60 1 2 
1 2 0.2 
1 3 5 
3 2 0.5 
2 1 5 

```

```output1
12.00 

```

