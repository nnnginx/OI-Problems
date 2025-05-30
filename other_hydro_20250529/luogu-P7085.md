## 题目描述


Wow! What a lucky day! Your company has just won a social contract for building a garage complex. Almost all formalities are done: contract payment is already transferred to your account.

So now it is the right time to read the contract. Okay, there is a sandlot in the form of $W \times H$ rectangle and you have to place some garages there. Garages are $w \times h$ rectangles and their edges must be parallel to the corresponding edges of the sandlot (you may not rotate garages, even by $90^{◦}).$ The coordinates of garages may be non-integer.

You know that the economy must be economical, so you decided to place as few garages as possible. Unfortunately, there is an opposite requirement in the contract: placing maximum possible number of garages.

Now let's see how these requirements are checked. . . The plan is accepted if it is impossible to add a new garage without moving the other garages (the new garage must also have edges parallel to corresponding sandlot edges).

![](https://www.acmicpc.net/upload/images2/garage.png)

Time is money, find the minimal number of garages that must be ordered, so that you can place them on the sandlot and there is no place for an extra garage.



## 输入格式


The only line contains four integers: $W , H , w , h$ -- dimensions of sandlot and garage in meters. You may assume that $1 \le w \le W \le 30 000$ and $1 \le h \le H \le 30 000$ .



## 输出格式


Output the optimal number of garages.



## 题目大意
你有一个 $W \times H$ 的大长方形。你又有无数个 $w \times h$ 的小长方形。请问，最少放入几个小长方形后，你无法再往这个大长方形里放入更多的小长方形。

所有小长方形不能重叠，也不能旋转。

```input1
11 4 3 2

```

```output1
2

```

```input2
10 8 3 4

```

```output2
2

```

```input3
15 7 4 2

```

```output3
4

```

## 提示
Time limit: 2 s, Memory limit: 256 MB. 



