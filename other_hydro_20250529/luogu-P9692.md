## 题目描述
Twenty years ago, the northern section of Beijing Road Pedestrian Street in Guangzhou unearthed eleven layers of pavement from the Tang Dynasty to the Republic of China, and the southern section excavated the foundation of Gongbei Building with five layers from the Song Dynasty to the Ming and Qing Dynasties. This proves that Beijing Road has a long history as a commercial pedestrian street since the Song Dynasty. At the same time, the first Guangdong Province Collegiate Programming Contest was also held at Sun Yat-sen University in Guangzhou. Today, twenty years later, Beijing Road Pedestrian Street has become one of Guangzhou's most famous tourist attractions and shopping destinations, and the Guangdong Province Collegiate Programming Contest is also celebrating its twentieth birthday.

![](https://cdn.luogu.com.cn/upload/image_hosting/qaieoirq.png)

There are $n$ stores in the pedestrian street which buy and sell the same type of product. The buying and selling price of one such product in the $i$-th store are both $a_i$. To avoid over-trading, the pedestrian street has a regulation, that one can only trade $b_i$ times in the $i$-th store (each buy or each sell both count as a trade) and can only trade one product each time.

You're going to earn money by buying and selling the products in the pedestrian street. If you have infinite amount of money at the beginning (that is to say, you can't be short of money when buying a product), what's the maximum total profit you can make? More precisely, \textit{profit} means the total amount of money earned by selling the products, minus the total amount of money spent for buying the products.

## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($1 \le n \le 10^5$) indicating the number of stores.

For the following $n$ lines, the $i$-th line contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 10^6$) indicating the price and the maximum number of trades in the $i$-th store.

It's guaranteed that the sum of $n$ of all test cases will not exceed $10^6$.

## 输出格式
For each test case output one line containing one integer indicating the maximum total profit.

## 题目大意
**【题目描述】**

二十年前，广州的北京路步行街北段出土了自唐代直到民国时期的十一层路面，南段则发掘出宋代至明清时期共五层的拱北楼建筑基址，佐证了北京路自宋代以来作为商业步行街的悠久历史；同时第一届广东省大学生程序设计竞赛也在位处广州的中山大学举办。二十年后的今天，北京路步行街已成为广州最负盛名的景点和购物胜地之一，而广东省大学生程序设计竞赛也迎来了自己的二十岁生日。

在步行街中，有 $n$ 间商店买卖同一种商品，第 $i$ 间商店一件商品的收购价和出售价均为 $a_i$ 元。为了防止过度交易，步行街有一个规定：您在第 $i$ 间商店最多进行 $b_i$ 次交易（一次买或一次卖均计为一次交易），且每次只能交易一件商品。

您准备通过在步行街中买卖这种商品来赚钱。假如初始时有无限的金钱（也就是说，不会因为钱不够而买不了一件商品），您最多能在步行街中赚到多少总利润？具体来说，``利润``指的是卖出商品获得的金钱总额，减去购买商品花费的金钱总额。

**【输入格式】**

有多组测试数据。第一行输入一个整数 $T$ 表示测试数据组数。对于每组测试数据：

第一行输入一个整数 $n$（$1 \le n \le 10^5$），表示商店的数量。

对于接下来 $n$ 行，第 $i$ 行输入两个整数 $a_i$ 和 $b_i$（$1 \le a_i, b_i \le 10^6$），分别表示第 $i$ 间商店的商品价格，以及该商店可以交易的最大次数。

保证所有数据 $n$ 之和不超过 $10^6$。

**【输出格式】**

每组数据输出一行一个整数，表示在步行街中赚到的最大总利润。

**【样例解释】**

对于第一组样例数据，最优方案是在第 $1$ 间商店买入 $2$ 件商品，在第 $3$ 间商店买入 $4$ 件商品，在第 $2$ 间商店卖出 $5$ 件商品，在第 $4$ 间商店卖出 $1$ 件商品。总利润为 $30 \times 5 + 50 \times 1 - 10 \times 2 - 20 \times 4 = 100$。

对于第二组样例数据，由于所有商店的商品价格都相同，因此无法获得利润。

```input1
2
4
10 2
30 7
20 4
50 1
2
1 100
1 1000
```

```output1
100
0
```

## 提示
For the first sample test case, the optimal strategy is to buy $2$ products from the $1$-st store, buy $4$ products from the $3$-rd store, sell $5$ products to the $2$-nd store and sell $1$ product to the $4$-th store. The total profit is $30 \times 5 + 50 \times 1 - 10 \times 2 - 20 \times 4 = 100$.

For the second sample test case, because all stores have the same price, there is no profit.

