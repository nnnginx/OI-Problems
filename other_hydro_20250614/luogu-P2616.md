## ��Ŀ����
Farmer John needs to travel to town to pick up K (1 <= K <= 100) pounds of feed. Driving D miles with K pounds of feed in his truck costs D\*K cents.

The county feed lot has N (1 <= N <= 100) stores (conveniently numbered 1..N) that sell feed. Each store is located on a segment of the X axis whose length is E (1 <= E <= 350). Store i is at location X\_i (0 < X\_i < E) on the number line and can sell FJ as much as F\_i (1 <= F\_i <= 100) pounds of feed at a cost of C\_i (1 <= C\_i <= 1,000,000) cents per pound. Amazingly, a given point on the X axis might have more than one store.

FJ starts at location 0 on this number line and can drive only in the positive direction, ultimately arriving at location E, with at least K pounds of feed. He can stop at any of the feed stores along the way and buy any amount of feed up to the the store's limit.

What is the minimum amount FJ has to pay to buy and transport the K pounds of feed? FJ knows there is a solution.

Consider a sample where FJ needs two pounds of feed from three stores (locations: 1, 3, and 4) on a number line whose range is 0..5:

```
0   1   2   3   4   5 
+---|---+---|---|---+ 
    1       1   1      Available pounds of feed 
    1       2   2      Cents per pound 
```
It is best for FJ to buy one pound of feed from both the second and third stores. He must pay two cents to buy each pound of feed for a total cost of 4. When FJ travels from 3 to 4 he is moving 1 unit of length and he has 1 pound of feed so he must pay 1\*1 = 1 cents.

When FJ travels from 4 to 5 he is moving one unit and he has 2 pounds of feed so he must pay 1\*2 = 2 cents.

The total cost is 4+1+2 = 7 cents. 

FJ ����ȥ�� $K$ ��ʳ�������ĳ����� $X$ ��ʳ�ÿ��һ��ͻ��� $X$ Ԫ��FJ �ĳ�����һ���ߣ��ܹ� $E$ ��·���� $E+1$ ���ط������ $0\sim E$�� FJ �� $0$ ��ʼ�ߣ��� $E$ ���������������ߣ���Ҫ�� $K$ ��ʳ� ������ $N$ ���̵꣬ÿ���̵��λ���� $X_i$��һ�����Ͽ����ж���̵꣩���� $F_i$ ��ʳ�ÿ�� $C_i$ Ԫ�� �ʵ��� $E$ ���� $K$ ��ʳ�����С���ѡ�

## �����ʽ
![](https://cdn.luogu.com.cn/upload/pic/1718.png)


## �����ʽ
![](https://cdn.luogu.com.cn/upload/pic/1719.png)


```input1
2 5 3
3 1 2
4 1 2
1 1 1
```

```output1
7
```

## ��ʾ
![](https://cdn.luogu.com.cn/upload/pic/1720.png)


