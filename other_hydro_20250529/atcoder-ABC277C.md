## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc277/tasks/abc277_c

$ 10^9 $ 階建てのビルがあり、$ N $ 本のはしごがかかっています。  
 ビルの $ 1 $ 階にいる高橋君ははしごを繰り返し使って（$ 0 $ 回でもよい）できるだけ高い階へ上りたいと考えています。  
 はしごには $ 1 $ から $ N $ までの番号がついており、はしご $ i $ は $ A_i $ 階と $ B_i $ 階を結んでいます。はしご $ i $ を利用すると $ A_i $ 階から $ B_i $ 階へ、または $ B_i $ 階から $ A_i $ 階へ双方向に移動することができますが、それ以外の階の間の移動は行うことはできません。  
 また、高橋君は同じ階での移動は自由に行うことができますが、はしご以外の方法で他の階へ移動することはできません。  
 高橋君は最高で何階へ上ることができますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ \ldots $ $ A_N $ $ B_N $

## 输出格式
答えを出力せよ。

## 题目大意
【题面翻译】

有一座很高的楼，你现在在第一层。

有 $n$ 个传送门，每个传送门连接第 $a_i$ 层与 $b_i$ 层。传送门是双向的。

请你求出你能到达的最高楼层。

translated by @[liangbowen](https://www.luogu.com.cn/user/367488).

【输入格式】

第一行，一个整数 $n$。

接下来 $n$ 行，每行两个数 $a_i$，$b_i$，表示传送门。

【输出格式】

输出你能到达的最高楼层。

【数据范围】

$1 \le n \le 2 \times 10^5$

$1 \le a_i, b_i \le 10^9$

保证 $a_i \ne b_i$。

```input1
4
1 4
4 3
4 10
8 3
```

```output1
10
```

```input2
6
1 3
1 5
1 12
3 5
3 12
5 12
```

```output2
12
```

```input3
3
500000000 600000000
600000000 700000000
700000000 800000000
```

```output3
1
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i,\ B_i\ \leq\ 10^9 $
- $ A_i\ \neq\ B_i $
- 入力はすべて整数
 
### Sample Explanation 1

はしご $ 1 $ で $ 4 $ 階に進み、はしご $ 3 $ で $ 10 $ 階に進むことにより、$ 10 $ 階にたどり着くことができます。

### Sample Explanation 3

他の階への移動ができない場合もあります。

