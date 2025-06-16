# AT_abc004_3 入れ替え

## 题目描述

这里有 $6$ 张卡，分别写了 $1$ 到 $6$ ，$6$ 个整数。最初，每张牌按从小到大排列。高桥君会给你一个整数 $N$ 。高桥君进行以下的操作： $i＝0，1 , 2，…，N-1$ 。从 $i＝0$ 按顺序进行。 从左到右第 $(i\bmod5)+1$ 张卡与第 $(i\bmod5)+2$ 张卡交换卡片的位置。所谓 $\bmod$ ，意味着“取余”，例如$8\bmod 5=3$，而且 $15\bmod5=0$。这里说明在 $N = 5$ 时进行的操作。
- i＝0的时候： $(0\bmod 5)+1＝1$， $(0\bmod 5)+2=2$，从左到右第1张的卡和第2张卡交换。
![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc004_3/9910e34356f567b079a89cb95447c11e913234c1.png)
- i = 1的时候：  
![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc004_3/e27b53d42b3efae94e288c0b97bc34e8579fc6fa.png)
- i = 2的时候：   
![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc004_3/244c2ec6f9beac0be821d79d7edfd2b166b89e66.png)
- i = 3的时候：  
![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc004_3/fac73fa6d6792eacb6baf5a251dde745c56db6d2.png)
- i = 4的时候：  
![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_abc004_3/4b74bb2dc81c4ba42fb5807fe65b2ad2049f5331.png)

因此，在 $N=5$ 的时候，卡的排列从左到右的编号为`234561`。请你代替高桥君，回答上述的操作全部结束后的从左到右卡的编号。

## 输入格式

一行一个整数 $N$ 代表操作次数。

## 输出格式

一行 $6$ 个整数，代表 $N$ 此操作后卡牌的顺序。

## 说明/提示

样例1 从左到右第 $1$ 张卡和第 $2$ 张卡交换 。  
样例2 是在问题文中所示的例子。  
对于 $30\%$ 的测试点， $1\le N\le50$  
对于 $100\%$ 的测试点， $1\le N\le 10^9$ 。