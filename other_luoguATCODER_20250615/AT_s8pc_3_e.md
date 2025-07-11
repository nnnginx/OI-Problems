# AT_s8pc_3_e 円と三角形

## 题目描述

[problemUrl]: https://atcoder.jp/contests/s8pc-3/tasks/s8pc_3_e

半径が $ 1 $ の円があり、頂点 $ 1 $ ～ $ N $ が時計回りに並んでいます。  
 頂点は, 円周を $ N $ 等分しています。  
 square1001は, $ 3 $ つの頂点を選んで三角形を作ろうとしています。

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_s8pc_3_e/c30927b9a1715796bda6cd457dcb8ef524309208.png)

   
 $ \frac{N(N-1)(N-2)}{6} $ 通りの作り方のうち, 面積が小さい順に数えて $ K $ 番目となる三角形の面積を出力してください。  
 ただし, 面積が同じ場合は、面積だけを出力すればいいので順番は適当で構いません。  
  
 例えば, $ N\ =\ 4,\ K\ =\ 3 $ のとき, 次のようになります。  
- 3頂点の番号が $ (1,2,3) $ のとき, 面積 $ =\ 1 $
- 3頂点の番号が $ (1,2,4) $ のとき, 面積 $ =\ 1 $
- 3頂点の番号が $ (1,3,4) $ のとき, 面積 $ =\ 1 $
- 3頂点の番号が $ (2,3,4) $ のとき, 面積 $ =\ 1 $
 
 よって, 3番目の三角形の面積 $ =\ 1.0 $ となります。  
 問題作成者：E869120

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N\ K $

- 1行目に, 円周上にある点の数 $ N $ と, 何番目の三角形かを表す整数 $ K $ が, 空白区切りで与えられる。

## 输出格式

- 面積が小さい順から数えて $ K $ 番目となる三角形の面積を出力しなさい。
- ただし, 絶対誤差または相対誤差が $ 10^{-9} $ 以下であれば正解とみなされる。

## 输入输出样例 #1

### 输入 #1

```
4 3
```

### 输出 #1

```
1.000000000000000000
```

## 输入输出样例 #2

### 输入 #2

```
6 9
```

### 输出 #2

```
0.86602540378
```

## 输入输出样例 #3

### 输入 #3

```
12 220
```

### 输出 #3

```
1.29903810568
```

## 说明/提示

### 制約

- $ 3\ \le\ N\ \le\ 200,000 $
- $ 1\ \le\ K\ \le\ \frac{N(N\ -\ 1)(N\ -\ 2)}{6} $

### 小課題

 小課題1 \[ $ 160 $ 点 \]

- $ N\ \le\ 100 $
 
 小課題2 \[ $ 240 $点 \]   
- $ N\ \le\ 1000 $
 
 小課題3 \[ $ 450 $点 \]   
- 追加の制約はない。

### Sample Explanation 1

この入力例は問題文で説明したとおりです。

### Sample Explanation 2

$ N\ =\ 6 $ のとき, 面積が $ \frac{\sqrt{3}}{4} $ となるような頂点の選び方は $ 6 $ 通り, 面積が $ \frac{\sqrt{3}}{2} $ となるような頂点の選び方は $ 12 $ 通り, 面積が $ \frac{3\ \sqrt{3}}{4} $ となるような頂点の選び方は $ 2 $ 通りあります。 よって, $ K\ =\ 9 $ 番目の三角形の面積は $ \frac{\sqrt{3}}{2} $ となります。

### Sample Explanation 3

$ N\ =\ 12 $ のとき, 三角形の作り方は $ \frac{12\ \times\ 11\ \times\ 10}{6}\ =\ 220 $ 通りあります。 この中で面積が一番大きいのは正三角形となるときなので, $ K\ =\ 220 $ 番目の三角形の面積は $ \frac{3\ \sqrt{3}}{4} $ となります。