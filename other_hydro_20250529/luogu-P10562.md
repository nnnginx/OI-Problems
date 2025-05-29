## 题目描述
There are three points $A(a, 0)$, $B(0, b)$, $C(0, 0)$ in the plane rectangular coordinate system. Define the size of triangle $ABC$ as the number of squares that belong to it.
    
    
    
For integers $x,y$, one square is defined by four points $(x, y)$, $(x + 1, y)$, $(x, y + 1)$, $(x + 1, y + 1)$. We consider a square to belong to a triangle if half or more of it is inside the triangle.
    
    
    
For example, when $a = 8, b = 6$, the size of triangle $ABC$ will be $24$. The image below shows which squares are counted in the triangle.

![](https://cdn.luogu.com.cn/upload/image_hosting/3fnqi74y.png)

## 输入格式

    
The first and only line contains two integers $a\ (1\le a\le 10^6)$ and $b\ (1\le b\le 10^6)$.

## 输出格式

Print an integer: the size of triangle $ABC$.
    

```input1
6 8
```

```output1
24
```

```input2
5 5

```

```output2
15
```

```input3
1 999999
```

```output3
500000
```

