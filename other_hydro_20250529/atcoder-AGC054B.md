## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc054/tasks/agc054_b

みかんが $ N $ 個あり，$ 1 $ から $ N $ までの番号がついています． みかん $ i $ の重さは $ W_i $ です． 高橋くんと青木くんがこれらを以下のようにして分けます．

- $ (1,2,\cdots,N) $ の順列 $ (p_1,\ p_2,\ \cdots,\ p_N) $ を選ぶ．
- $ i\ =\ 1,\ 2,\ \cdots,\ N $ について，この順に以下のことを行う
  
  
  - 高橋くんがすでにとったみかんの重さの合計が，青木くんがすでにとったみかんの重さの合計以下なら，みかん $ p_i $ を高橋くんがとる． そうでないならみかん $ p_i $ を青木くんが取る．

最終的に二人が取るみかんの重さの合計が等しくなるような順列 $ p $ が何通りあるかを $ 998244353 $ で割った余りを求めてください．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ N $ $ W_1 $ $ W_2 $ $ \cdots $ $ W_N $

## 输出格式
答えを出力せよ．

## 题目大意
有 $n(2\le n\le100)$ 个数，每个数有一个权值 $a_i(1\le a_i\le 100)$。现在对于一个排列 $p$，有两个人 $A$ 和 $B$ 会做如下操作：

- 对于 $1\sim n$ 从小到大的每个 $i$，如果 $A$ 手上数的权值和不大于 $B$ 的，那么 $A$ 拿走第 $p_i$ 个数，否则 $B$ 拿走。

问有多少个排列使得 $A$ 和 $B$ 最终手上的数的权值和一样。答案对 $998244353$ 取模。

```input1
3
1 1 2
```

```output1
4
```

```input2
4
1 2 3 8
```

```output2
0
```

```input3
20
2 8 4 7 5 3 1 2 4 1 2 5 4 3 3 8 1 7 8 2
```

```output3
373835282
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ W_i\ \leq\ 100 $
- 入力される値はすべて整数

### Sample Explanation 1

条件を満たす $ p $ は，$ (1,3,2),(2,3,1),(3,1,2),(3,2,1) $ の $ 4 $ 通りです． 例えば，$ p=(3,2,1) $ の時は，以下のように進行します． - $ i=1 $: 高橋くんがすでにとったみかんの重さの合計は $ 0 $ で，青木くんがすでにとったみかんの重さの合計は $ 0 $ である． 高橋くんがみかん $ p_i=3 $ をとる． - $ i=2 $: 高橋くんがすでにとったみかんの重さの合計は $ 2 $ で，青木くんがすでにとったみかんの重さの合計は $ 0 $ である． 青木くんがみかん $ p_i=2 $ をとる． - $ i=3 $: 高橋くんがすでにとったみかんの重さの合計は $ 2 $ で，青木くんがすでにとったみかんの重さの合計は $ 1 $ である． 青木くんがみかん $ p_i=1 $ をとる． よって $ p=(3,2,1) $ は条件を満たす順列です．

