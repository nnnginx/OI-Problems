## 题目描述
[problemUrl]: https://atcoder.jp/contests/cf16-relay-open/tasks/relay_b

`b`, `d`, `p`, `q` の $ 4 $ 種類の文字から構成される文字列 $ S $ が与えられます。 $ S $ が「鏡文」かどうかを判定してください。

ここで、「鏡文」というのは以下の操作を文字列 $ S $ に施したときに、元と同じ文字列が得られるような文字列 $ S $ のことです。

1. $ S $ の順序を逆転する。
2. `b` を `d` に、`d` を `b` に、`p` を `q` に、`q` を `p` に置換する。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ S $ が「鏡文」ならば `Yes` を、そうでないならば `No` を出力せよ。

## 题目大意
# 题目描述

给出由b、d、p、q四种字符组成的字符串$S$。请判断$S$是不是“镜像字符串”。

这里的“镜像字符串”是指对字符串S进行以下操作后，可得到与原字符串相同的字符串。
1. 反转S。（例："bdpq"=>"qpdb"）
2. 改b为d，改d为b，改p为q，改q为p（不要搞错对应关系）

# 输入输出格式
## 输入格式：
标准输入，格式如下：

	S
    
## 输出格式：
如果$S$是镜像字符串，输入"Yes"，否则输出"No"。（不要输出引号）
# 输入输出样例（略）
# 说明：
## 条件：
- $1≤|S|≤10^5$（$|S|$表示$S$的长度）
- $S$由且仅由b、d、p、q四种字符构成

感谢@std_cpp 提供的翻译

```input1
pdbq
```

```output1
Yes
```

```input2
ppqb
```

```output2
No
```

## 提示
### 制約

- $ 1\ \leq\ |S|\ \leq\ 10^5 $
- $ S $ は `b`, `d`, `p`, `q` の $ 4 $ 種類の文字のみから構成される。

