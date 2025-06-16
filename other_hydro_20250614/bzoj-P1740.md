## 题目描述
The cows have purchased a yogurt factory that makes world-famous Yucky Yogurt. Over the next $n \ (1 \le n \le 10^4)$ weeks, the price of milk and labor will fluctuate weekly such that it will cost the company $c_i \ (1 \le c_i \le 5\times 10^3)$ cents to produce one unit of yogurt in week $i$. Yucky's factory, being well-designed, can produce arbitrarily many units of yogurt each week. Yucky Yogurt owns a warehouse that can store unused yogurt at a constant fee of $s \ (1 \le s \le 100)$ cents per unit of yogurt per week. Fortuitously, yogurt does not spoil. Yucky Yogurt's warehouse is enormous, so it can hold arbitrarily many units of yogurt. Yucky wants to find a way to make weekly deliveries of $y_i \ (0 \le y_i \le 10^4)$ units of yogurt to its clientele ($y_i$ is the delivery quantity in week $i$). Help Yucky minimize its costs over the entire Nweek period. Yogurt produced in week $i$, as well as any yogurt already in storage, can be used to meet Yucky's demand for that week.

牛们收购了一个奶酪工厂，接下来的 $n$ 个星期里，牛奶价格和劳力价格不断起伏。第 $i$ 周，生产一个单位奶酪需要 $c_i$ 便士。工厂有一个货栈，保存一单位奶酪，每周需要 $s$ 便士，这个费用不会变化。货栈十分强大，可以存无限量的奶酪，而且保证它们不变质。工厂接到订单，在第 $i$ 周需要交付 $y_i$ 单位的奶酪给委托人。第 $i$ 周刚生产的奶酪，以及之前的存货，都可以作为产品交付。请帮牛们计算这段时间里完成任务的最小代价。
## 输入格式
* Line $1$: Two space-separated integers, $n$ and $s$.
* Lines $2\dots n+1$: Line $i+1$ contains two space-separated integers: $c_i$ and $y_i$.
* 第一行输入两个整数 $n$ 和 $s$。
* 接下来 $n$ 行输入 $c_i$ 和 $y_i$。
## 输出格式
* Line $1$: Line $1$ contains a single integer: the minimum total cost to satisfy the yogurt schedule. Note that the total might be too large for a 32-bit integer.
* 输出最少的代价。注意，可能超过 32 位长整型。
```input1
4 5
88 200
89 400
97 300
91 500
```
```output1
126900
```
## 样例说明
第 $1$ 周生产 $200$ 单位奶酪并全部交付；第 $2$ 周生产 $700$ 单位，交付 $400$ 单位，有 $300$ 单位；第 $3$ 周交付 $300$ 单位存货；第 $4$ 周生产并交付 $500$ 单位。
## 数据规模与约定
对于 $100\%$ 的数据，$1\le n\le 10^4$，$1 \leq c_i \leq 5\times 10^3$，$1 \leq s \leq 100$，$0 \leq y_i \leq 10^4$。
## 题目来源
Gold