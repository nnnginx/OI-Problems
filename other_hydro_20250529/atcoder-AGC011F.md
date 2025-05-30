## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc011/tasks/agc011_f

高橋王国には，$ 1 $ 本の鉄道路線が走っています． この路線は $ N $ 個の区間 $ 1 $, $ 2 $, ..., $ N $ と $ N+1 $ 個の駅 $ 0 $, $ 1 $, ..., $ N $ からなり，区間 $ i $ は駅 $ i-1 $ と駅 $ i $ を直接結んでいます． 列車が区間 $ i $ を走行するには，方向によらず，ちょうど $ A_i $ 分かかります． また，$ N $ 個の区間のそれぞれは，区間全体にわたって複線であるか，区間全体にわたって単線であるかのどちらかです． $ B_i\ =\ 1 $ のときは区間 $ i $ は単線，$ B_i\ =\ 2 $ のときは区間 $ i $ は複線です． 複線の区間では両方向の列車がすれ違うことができますが，単線の区間ではすれ違うことはできません． ただし，列車が駅にいる場合は列車同士がすれ違うことができます．

すぬけ君は，この路線に図のように $ K $ 分間隔で列車を走らせようとしています．ここで，太線は列車が走行している位置を表します． (詳しくは，入出力例 1 を見てください．)

![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_agc011_f/f1b66d955f996216abb6aa9bc14f02d5b504cc3c.png)

このとき，駅 $ 0 $ から駅 $ N $ までの列車の所要時間と，駅 $ N $ から駅 $ 0 $ までの列車の所要時間の合計の最小値を求めてください． この問題の制約の下，適切な列車の走らせ方が存在するとき，この最小値は必ず整数になることが証明できます．

なお，列車の発車時刻や到着時刻が満たすべき条件は，厳密に書くと下のようになります．

- どの列車も，駅 $ 0 $ を出発して駅 $ N $ まで向かうか，駅 $ N $ を出発して駅 $ 0 $ まで向かうかのいずれかである．
- どの列車も，区間 $ i $ をちょうど $ A_i $ 分かけて走行する．例えば，駅 $ N $ 行きのある列車が駅 $ i-1 $ を時刻 $ t $ に出発したなら，この列車は駅 $ i $ にちょうど時刻 $ t+A_i $ に到着する．
- ある駅で，時刻 $ s $ に駅 $ N $ 行きの列車が到着し，その列車が時刻 $ t $ に発車したとすると，駅 $ N $ 行きの次の列車は時刻 $ s+K $ に到着し，時刻 $ t+K $ に発車する．また，駅 $ N $ 行きの前の列車は時刻 $ s-K $ に到着し，時刻 $ t-K $ に発車する．駅 $ 0 $ 行きの列車についても同様である．
- 異なる方向の列車が，同時に同じ単線区間（両端の駅を除く）を走行していてはならない．

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ : $ A_N $ $ B_N $

## 输出格式
駅 $ 0 $ から駅 $ N $ までの列車の所要時間と，駅 $ N $ から駅 $ 0 $ までの列車の所要時間の合計の最小値を表す整数を出力せよ． ただし，条件をすべて満たすように列車を走らせることが不可能な場合は，$ -1 $ を出力せよ．

## 题目大意
# 题目描述

在高桥王国中有一条铁路，这条铁路分为$n$个区间$1⋯n$和$n+1$个站台$0⋯n$，区间$i$连接站台$i-1$和$i$

一列火车经过区间$i$会消耗$A_i$的时间，每个区间的铁路是双向的或单向的，如果$B_i=1$那么区间$i$是单向的，否则它是双向的

现在すぬけ(snuke)君想要设计一个火车时间表，满足以下约定

所有的火车要么从站台$0$到站台$n$，要么从站台$n$到站台$0$

对任意终点为$n$的火车，如果它在$t$时刻离开站台$i−1$并开往站台$i$，那么它必须在$t+A_i$时刻到达$i$站台，对反方向要求相同

对任意终点为$n$的火车，如果它在$s$时刻到达站台$i$并在$t$时刻离开站台$i$，那么一列经过站台$i$的终点为$n$的火车必须在$s+K$时刻到达站台$i$并在$t+K$时刻离开站台$i$，对反方向要求相同

在任意时刻不能有两列相向而行的火车在单向区间内互相穿过

现在你要找出一个时间表，使得一列火车从$0$到$n$和从$n$到$0$的时间之和最短，观察样例$1$可以帮助你更好地理解题目

# 输入格式

$ N $ $ K $

$ A_1 $ $ B_1 $ 

$ A_2 $ $ B_2 $ 

:

$ A_N $ $ B_N $ 

# 输出格式

一行一个整数，表示列车上下行最短的开车时间之和，如果不存在合法方案则输出-1

# 数据规模

$1\leq N \leq 100000$

$1\leq K \leq 10^9$

$1\leq A_i \leq 10^9$

$B_i$要么是1要么是2

所有输入的数都是整数

```input1
3 10
4 1
3 1
4 1
```

```output1
26
```

```input2
1 10
10 1
```

```output2
-1
```

```input3
6 4
1 1
1 1
1 1
1 1
1 1
1 1
```

```output3
12
```

```input4
20 987654321
129662684 2
162021979 1
458437539 1
319670097 2
202863355 1
112218745 1
348732033 1
323036578 1
382398703 1
55854389 1
283445191 1
151300613 1
693338042 2
191178308 2
386707193 1
204580036 1
335134457 1
122253639 1
824646518 2
902554792 2
```

```output4
14829091348
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 100000 $
- $ 1\ \leq\ K\ \leq\ 10^9 $
- $ 1\ \leq\ A_i\ \leq\ 10^9 $
- $ A_i $ は整数
- $ B_i\ =\ 1 $ または $ B_i\ =\ 2 $

### 部分点

- $ 500 $ 点分のテストケースでは，すべての区間が単線である．すなわち，$ B_i\ =\ 1 $ が成り立つ．
- 別の $ 500 $ 点分のテストケースでは，$ N\ \leq\ 200 $ が成り立つ．

### Sample Explanation 1

例えば，下図に示すように列車を走らせると，所要時間の合計が $ 26 $ 分になります． !\[\](https://atcoder.jp/img/agc011/a5c221ce77ab6ee8aee48e75a4e5c969.png) 例えば，赤線で示した列車は，時刻 $ 0 $ に駅 $ 0 $ を出発し，時刻 $ 4 $ に駅 $ 1 $ に到着し，時刻 $ 5 $ に駅 $ 1 $ を出発し，時刻 $ 8 $ に駅 $ 2 $ に到着します．

