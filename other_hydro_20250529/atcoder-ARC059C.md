## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc059/tasks/arc059_c

競プロ幼稚園には$ 1 $～$ N $の番号がついた$ N $人の子供がいます。えび先生は、区別できない$ C $個のキャンディーを子供たちに分配することにしました。子供$ i $の*はしゃぎ度*が$ x_i $の時、キャンディーを$ a $個もらうと子供$ i $の*うれしさ*は$ x_i^a $になります。*幼稚園の活発度*は$ N $人の子供たちの*うれしさ*の**積**になります。各子供にキャンディーを非負整数個配ってC個配りきる方法それぞれに対して*幼稚園の活発度*を計算して、その総和を子供たちの*はしゃぎ度*$ x_1 $,..,$ x_N $の関数とみて$ f(x_1,..,x_N) $とおきます。$ A_i,B_i\ (1≦i≦N) $が与えられるので、 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_arc059_c/5091c620504ef849bc354ad4c33d9ab9a741e860.png)を$ 10^9+7 $で割ったあまりを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ C $ $ A_1 $ $ A_2 $ ... $ A_N $ $ B_1 $ $ B_2 $ ... $ B_N $

## 输出格式
![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_arc059_c/5091c620504ef849bc354ad4c33d9ab9a741e860.png) の値を$ 10^9+7 $で割ったあまりを出力せよ。

## 题目大意
**题目描述**

AtCoder幼儿园里有N个小朋友，编号1~N，Evi先生要把C颗糖果分给他们。

小朋友可以得到任意多颗糖果，如果第$i$个小朋友，得到了$a$颗糖，他会得到$x_i^a$的愉悦度，$x_i$是第$i$个小朋友的兴奋度。幼儿园活跃指数定义为$N$个小朋友愉悦度的乘积。

令$f(x_1,x_2,...,x_N)$表示所有分糖果的方案对应的幼儿园活跃指数的和。

现在给出$A_i,B_i(1<=i<=N)$，要求 $\sum_{x_1=A_1}^{B_1} \sum_{x_2=A_2}^{B_2} ... \sum_{x_N=A_N}^{B_N} f(x_1,x_2,...,x_N)$，对1000000007取模。

**输入格式**

N，C

$A_1,A_2,...,A_N$

$B_1,B_2,...,B_N$


**输出格式**

一行一个整数表示答案

翻译提供者：XHRlyb_2001

```input1
2 3
1 1
1 1
```

```output1
4
```

```input2
1 2
1
3
```

```output2
14
```

```input3
2 3
1 1
2 2
```

```output3
66
```

```input4
4 8
3 1 4 1
3 1 4 1
```

```output4
421749
```

```input5
3 100
7 6 5
9 9 9
```

```output5
139123417
```

## 提示
### 制約

- $ 1≦N≦400 $
- $ 1≦C≦400 $
- $ 1≦A_i≦B_i≦400\ (1≦i≦N) $

### 部分点

- $ A_i=B_i\ (1≦i≦N) $ を満たすデータセットに正解した場合は、部分点として$ 400 $ 点が与えられる。

### Sample Explanation 1

$ A_i=B_i $なので部分点の条件を満たします。 子供$ 1 $,$ 2 $の\*はしゃぎ度\*が共に$ 1 $のもの($ f(1,1) $)を考えればよく、この時、 - 子供$ 1 $に$ 0 $個,子供$ 2 $に$ 3 $個のキャンディーをあげると、\*幼稚園の活発度\*は$ 1^0*1^3=1 $ - 子供$ 1 $に$ 1 $個,子供$ 2 $に$ 2 $個のキャンディーをあげると、\*幼稚園の活発度\*は$ 1^1*1^2=1 $ - 子供$ 1 $に$ 2 $個,子供$ 2 $に$ 1 $個のキャンディーをあげると、\*幼稚園の活発度\*は$ 1^2*1^1=1 $ - 子供$ 1 $に$ 3 $個,子供$ 2 $に$ 0 $個のキャンディーをあげると、\*幼稚園の活発度\*は$ 1^3*1^0=1 $ 従って$ f(1,1)=1+1+1+1=4 $となり、$ f $を足し合わせた答えは$ 4 $です。

### Sample Explanation 2

子供が一人なので、子供$ 1 $の\*うれしさ\*が\*幼稚園の活発度\*になります。また、キャンディの配り方は2つとも子供$ 1 $にあげる$ 1 $通りしかないため、この時の\*幼稚園の活発度\*は$ f $の値に等しくなります。 - 子供$ 1 $の\*はしゃぎ度\*が$ 1 $の時、$ f(1)=1^2=1 $ - 子供$ 1 $の\*はしゃぎ度\*が$ 2 $の時、$ f(2)=2^2=4 $ - 子供$ 1 $の\*はしゃぎ度\*が$ 3 $の時、$ f(3)=3^2=9 $ 従って答えは$ 1+4+9=14 $となります。

### Sample Explanation 3

$ f(1,1)=4\ ,\ f(1,2)=15\ ,\ f(2,1)=15\ ,\ f(2,2)=32 $ となることがわかるので、答えは$ 4+15+15+32=66 $になります。

### Sample Explanation 4

部分点の条件を満たします。

