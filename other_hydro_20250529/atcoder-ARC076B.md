## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc065/tasks/arc076_b

平面上に、$ N $ 個の街があります。$ i $ 個目の街は、座標 $ (x_i,y_i) $ にあります。同じ座標に、複数の街があるかもしれません。

座標 $ (a,b) $ にある街と座標 $ (c,d) $ にある街の間に道を造るのには、$ min(|a-c|,|b-d|) $ 円かかります。街と街の間以外に、道を造ることはできません。

任意の $ 2 $ つの街の間を、道を何本か通って行き来できるようにするためは、最低で何円必要でしょうか。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ x_1 $ $ y_1 $ $ x_2 $ $ y_2 $ : $ x_N $ $ y_N $

## 输出格式
任意の $ 2 $ つの街の間を道を何本か通って行き来できるようにするためにかかるお金の最小値を出力せよ。

## 题目大意
## 题目描述
平面上有 $N$ 个城市。第 $i$ 个城市的坐标为 $(x_i,y_i)$ 。同一个坐标上可能有多个城市。在坐标为 $(a,b)$ 的城市和坐标为 $(c,d)$ 的城市间建造一条道路需要 $min(|a-c|,|b-d|)$ 円。只能在城市与城市间建造道路。
要使任意两个城市之间有直接或间接道路相连，最少需要多少円？

## 数据范围
- $2 \leq N \leq 10^5$
- $0 \leq x_i,y_i \leq 10^9$
- 输入全为整数

## 输入
输入按以下形式：
$$ N $$
$$ x_1 \space y_1 $$
$$ x_2 \space y_2 $$
$$ : $$
$$ x_N \space y_N $$

## 输出
请输出使任意两城市间有直接或间接道路连接所需最少钱数。

## 样例1解释
在城市 $1$ 与城市 $2$ 间建造一条道路，在城市 $2$ 与城市 $3$ 间建造一条道路，花费 $2+1=3$ 円。

感谢@ミク 提供的翻译

```input1
3
1 5
3 9
7 8
```

```output1
3
```

```input2
6
8 3
4 9
12 19
18 1
13 5
7 6
```

```output2
8
```

## 提示
### 制約

- $ 2\ ≦\ N\ ≦\ 10^5 $
- $ 0\ ≦\ x_i,y_i\ ≦\ 10^9 $
- 入力は全て整数である

### Sample Explanation 1

街 $ 1 $ と $ 2 $ 、街 $ 2 $ と $ 3 $ の間に道を造ると、かかるお金は $ 2+1=3 $ 円になります。

