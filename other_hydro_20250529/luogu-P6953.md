## 题目描述


Bella is working in a factory that produces boxes. All boxes are in a shape of rectangular parallelepipeds. A net of the corresponding parallelepiped is cut out of a flat rectangular piece of cardboard of size $w$ *h . This net is a polygon with sides parallel to the sides of the rectangle of the cardboard. The net is bent along several lines and is connected along the edges of the resulting parallelepiped to form a box. The net is bent only along the edges of the resulting box.

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15284/1.png)

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15284/2.png)

The first example

The third example

Bella is a software developer and her task is to check whether it is possible to make a box of size $a \times b \times c$ out of a cardboard of size $w \times h$ . Bella did write a program and boxes are being produced. Can you do the same?



## 输入格式


The first line contains three integers a , $b$ , and $c$ -- the dimensions of the box.

The second line contains two integers $w$ and $h$ -- the width and the height of the cardboard.

All integers are positive and do not exceed $10^{8}.$



## 输出格式


Print `Yes` if it is possible to cut a box a $ \times b \times c$ out of a cardboard of size $w \times h$ . Print `No` otherwise.



## 题目大意
给出一个长方体的长、宽、高（分别是 $a, b, c$），问：能否在一张长为 $w$，宽为 $h$ 的纸上裁出这个长方体的某一个侧面展开图。

如果可以，请输出 `Yes`，否则输出 `No`。

```input1
1 2 3
6 5

```

```output1
Yes

```

```input2
1 2 3
5 5

```

```output2
No

```

```input3
1 1 1
10 2

```

```output3
Yes

```

## 提示
Time limit: 3 s, Memory limit: 512 MB. 



