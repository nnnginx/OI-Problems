## 题目描述
Farmer John realizes that the income he receives from milk production is insufficient to fund the growth of his farm, so to earn some extra money, he launches a cow-rental service, which he calls "USACOW" (pronounced "Use-a-cow").

Farmer John has $N$ cows ($1 \leq N \leq 100,000$), each capable of producing some amount of milk every day. The $M$ stores near FJ's farm ($1 \leq M \leq 100,000$) each offer to buy a certain amount of milk at a certain price. Moreover, Farmer John's $R$ ($1 \leq R \leq 100,000$) neighboring farmers are each interested in renting a cow at a certain price.


Farmer John has to choose whether each cow should be milked or rented to a nearby farmer. Help him find the maximum amount of money he can make per day.


## 输入格式
The first line in the input contains $N$, $M$, and $R$. The next $N$ lines each contain an integer $c_i$ ($1 \leq c_i \leq 1,000,000$), indicating that Farmer John's $i$th cow can produce $c_i$ gallons of milk every day. The next $M$ lines each contain two integers $q_i$ and $p_i$ ($1 \leq q_i, p_i \leq 1,000,000$), indicating that the $i$th store is willing to buy up to $q_i$ gallons of milk for $p_i$ cents per gallon. Keep in mind that Farmer John can sell any amount of milk between zero and $q_i$ gallons to a given store. The next $R$ lines each contain an integer $r_i$ ($1 \leq r_i \leq 1,000,000$), indicating that one of Farmer John's neighbors wants to rent a cow for $r_i$ cents per day.


## 输出格式
The output should consist of one line containing the maximum profit Farmer John can make per day by milking or renting out each of his cows. Note that the output might be too large to fit into a standard 32-bit integer, so you may need to use a larger integer type like a "long long" in C/C++.


## 题目大意
### 题目描述

Farmer John 意识到牛奶生产的收入不足以支持农场的扩展，因此为了赚取额外收入，他推出了一项奶牛租赁服务，称为“USACOW”（发音为“Use-a-cow”）。

Farmer John 有 $N$ 头奶牛（$1 \leq N \leq 100,000$），每头奶牛每天可以生产一定量的牛奶。附近的 $M$ 家商店（$1 \leq M \leq 100,000$）每家都愿意以一定价格购买一定量的牛奶。此外，Farmer John 的 $R$ 个邻居（$1 \leq R \leq 100,000$）每家都愿意以一定价格租赁一头奶牛。

Farmer John 需要决定每头奶牛是用于产奶还是租给附近的农民。请帮助他计算每天可以赚取的最大金额。

### 输入格式

输入的第一行包含 $N$、$M$ 和 $R$。接下来的 $N$ 行每行包含一个整数 $c_i$（$1 \leq c_i \leq 1,000,000$），表示 Farmer John 的第 $i$ 头奶牛每天可以生产 $c_i$ 加仑牛奶。接下来的 $M$ 行每行包含两个整数 $q_i$ 和 $p_i$（$1 \leq q_i, p_i \leq 1,000,000$），表示第 $i$ 家商店愿意以每加仑 $p_i$ 美分的价格购买最多 $q_i$ 加仑牛奶。请注意，Farmer John 可以向每家商店出售任意数量的牛奶，范围从 $0$ 到 $q_i$ 加仑。接下来的 $R$ 行每行包含一个整数 $r_i$（$1 \leq r_i \leq 1,000,000$），表示 Farmer John 的一个邻居愿意以每天 $r_i$ 美分的价格租赁一头奶牛。

### 输出格式

输出应包含一行，表示 Farmer John 通过产奶或租赁奶牛每天可以获得的最大利润。请注意，输出可能超过标准 32 位整数的范围，因此可能需要使用更大的整数类型，例如 C/C++ 中的 `long long`。

### 提示

Farmer John 应该让奶牛 #1 和 #4 产奶，每天生产 $13$ 加仑牛奶。他应该完全满足 $10$ 加仑的订单，赚取 $250$ 美分，并以每加仑 $15$ 美分的价格出售剩余的 $3$ 加仑，总共赚取 $295$ 美分的牛奶利润。

然后，他应该将其他三头奶牛分别以 $250$、$80$ 和 $100$ 美分的价格租出，赚取额外的 $430$ 美分。（他应该忽略 $40$ 美分的租赁请求。）这样，他每天的总利润为 $725$ 美分。

```input1
5 3 4
6
2
4
7
1
10 25
2 10
15 15
250
80
100
40
```

```output1
725

```

## 提示
Farmer John should milk cows #1 and #4, to produce 13 gallons of milk. He should completely fill the order for 10 gallons, earning 250 cents, and sell the remaining three gallons at 15 cents each, for a total of 295 cents of milk profits.


Then, he should rent out the other three cows for 250, 80, and 100 cents, to earn 430 more cents. (He should leave the request for a 40-cent rental unfilled.) This is a total of 725 cents of daily profit.


