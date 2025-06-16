## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc005/tasks/agc005_b

すぬけ君はある日友人から長さ $ N $ の順列 $ a_1,\ a_2,\ ...,\ a_N $ を貰いました。

![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_agc005_b/7385c80af4629f5f6d11fed58e1b38d3c006d06d.png)

を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ a_2 $ $ ... $ $ a_N $

## 输出格式
$ 1 $ 行に答えを出力する。

なお、32bit整数型に答えが収まるとは限らないことに注意すること。

## 题目大意
**Translated by [aoweiyin](https://www.luogu.org/space/show?uid=77834)**

## 题意翻译

给你一个长度为 $N(1\leq N\leq 200,000)$ 的，是 $(1,2\dots,N)$ 的排列的数组 $a$。

求 $\sum^{N}_ {l=1}\sum^{N}_ {r=l} \min(a_l,a_{l+1},\dots,a_r)$。

#### 输入格式：

$N$

$a_1\ a_2\dots a_N$




```input1
3
2 1 3
```

```output1
9
```

```input2
4
1 3 2 4
```

```output2
19
```

```input3
8
5 4 8 1 2 6 7 3
```

```output3
85
```

## 提示
### 制約

- $ 1\ ≦\ N\ ≦\ 200,000 $
- $ (a_1,\ a_2,\ ...,\ a_N) $ は $ (1,\ 2,\ ...,\ N) $ を並び替えたものである

