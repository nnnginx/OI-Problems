# AT_abc310_d [ABC310D] Peaceful Teams

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc310/tasks/abc310_d

$ N $ 人のスポーツ選手がいます。

$ N $ 人の選手たちには互いに相性の悪い選手のペアが $ M $ 組あり、相性の悪い組のうち $ i\ (1\leq\ i\leq\ M) $ 組目は $ A\ _\ i $ 番目の選手と $ B\ _\ i $ 番目の選手です。

あなたは、選手を $ T $ チームに分けます。 どの選手もちょうど一つのチームに属さなければならず、どのチームにも少なくとも一人の選手が属さなければなりません。 さらに、どの $ i=1,2,\ldots,M $ についても、 $ A\ _\ i $ 番目の選手と $ B\ _\ i $ 番目の選手が同じチームに属していてはいけません。

この条件を満たすチーム分けの方法は何通りあるか求めてください。 ただし、チーム分けの方法が異なるとは、ある二人が存在して、彼らが一方のチーム分けでは同じチームに所属し、もう一方では異なるチームに所属することをいいます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ T $ $ M $ $ A\ _\ 1 $ $ B\ _\ 1 $ $ A\ _\ 2 $ $ B\ _\ 2 $ $ \vdots $ $ A\ _\ M $ $ B\ _\ M $

## 输出格式

答えを $ 1 $ 行で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 2 2
1 3
3 4
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
5 1 2
1 3
3 4
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
6 4 0
```

### 输出 #3

```
65
```

## 输入输出样例 #4

### 输入 #4

```
10 6 8
5 9
1 4
3 8
1 6
4 10
5 7
5 6
3 7
```

### 输出 #4

```
8001
```

## 说明/提示

### 制約

- $ 1\leq\ T\leq\ N\leq10 $
- $ 0\leq\ M\leq\dfrac{N(N-1)}2 $
- $ 1\leq\ A\ _\ i\lt\ B\ _\ i\leq\ N\ (1\leq\ i\leq\ M) $
- $ (A\ _\ i,B\ _\ i)\neq\ (A\ _\ j,B\ _\ j)\ (1\leq\ i\lt\ j\leq\ M) $
- 入力はすべて整数
 
### Sample Explanation 1

次の $ 4 $ 通りのチーム分けが条件を満たします。 !\[\](https://img.atcoder.jp/abc310/b92c2629f68d56350fe18e6d0a8fa060.png) 他に条件を満たすチーム分けは存在しないので、$ 4 $ を出力してください。

### Sample Explanation 2

条件を満たすチーム分けがひとつも存在しないこともあります。

### Sample Explanation 3

相性の悪いペアがひとつも存在しないこともあります。