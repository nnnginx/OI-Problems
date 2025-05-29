## 题目描述

Farmer John made a profit last year! He would like to invest it well but wonders how much money he will make.

He knows the interest rate $R$ that is compounded annually at his bank. He has an integer amount of money $M$. He knows how many years $Y$ he intends to invest the money in the bank. Help him learn how much money he will have in the future by compounding the interest for each year he saves.

Print an integer answer without rounding. Answers for the test data are guaranteed to fit into a signed $32$ bit integer.

## 输入格式

* Line $1$: Three space-separated integers: $R$, $M$, and $Y$.

## 输出格式

* Line $1$: A single integer that is the number of dollars FJ will have after $Y$ years.

```input1
5 5000 4
```

```output1
6077
```

## 样例说明 

$5\%$ annual interest, $5000$ money, $4$ years.  
Year $1$: $1.05 \times 5000 = 5250$.  
Year $2$: $1.05 \times 5250 = 5512.5$.  
Year $3$: $1.05 \times 5512.50 = 5788.125$.  
Year $4$: $1.05 \times 5788.125 = 6077.53125$.  
The integer part of $6077.53125$ is $6077$.

## 数据规模与约定 

对于 $100\%$ 的数据：$0\leq R\leq 20$，$100\leq M\leq 10^6$，$0\leq Y\leq 400$。

## 题目来源

Usaco2005 qua