## ��Ŀ����
Mirko �� Slavko ��������ʱ�仨���������Ϻ͹ۿ� _The Biggest Loser_ �ϡ�



## ��Ŀ����
Mirko and Slavko are spending their free time playing with polygons and watching a new season of *The Biggest Loser*. Mirko recently drew a convex polygon with an even number of vertices $N$. Slavko then considered each pair of oposite sides (two sides are opposite if there are $\dfrac N2 - 1$ sides between them), drew straight lines that lie on those sides and colored them along with the part of the plane that lies between them and contains the polygon. Finally, Mirko found a set of $Q $ points and decided to challenge Slavko to answer for each point whether it lies in the colored or uncolored part of the plane. The new episode of *The Biggest Loser* is about to start and Slavko doesn��t have the time to answer Mirko��s queries. Can you help him?

## �����ʽ
��һ�У�һ������ $T$������������ Mirko ��ѯ�Ĳ����� ������ֻ������ $0$ �� $1$��

�ڶ��У�һ�������� $n$��

�� $3 \sim n + 2$ �У�ÿ�� $2$ �������� $x_i, y_i$ ����ʾ����ε�һ�����㡣�����ǰ���ʱ��˳������ģ�û�����������Ķ����ǹ��ߵġ�

�� $n + 3$ �У�һ�������� $q$��

������ $q$ �У�ÿ�ж����������� $a_i, b_i$�����������ڵ� $i$ �� Mirko ��ѯ�����ɵ�Ĳ�����$x_i$ ���� Mirko ��ѯ�ĵ� $i$ ������ $i$ �㣩��ƽ���ɫ�����ϵĵ����� ��Ȼ��$x_0 = 0$��Ȼ��Ӧ�� Mirko �� $i$ ����ѯ�ĵ�����Ϊ��

$$p_i = (a_i \oplus (T \times x^{3}_{i-1}), b_i \oplus(T \times x^{3}_{i-1}))$$

���� $\oplus$ ����λ������㡣

 

## �����ʽ
��� Mirko ��ѯ�ĵ� $i$ ����λ��ƽ�����ɫ���֣�������ĵ� $i$ ��Ϊ $\tt DA$�� ���򣬵� $i$ ��Ϊ $\tt NE$��

## ��Ŀ����
Mirko ���������һ������ż�������� $n$ ��͹����Ρ�

Slavko ѡ����ÿ��Աߣ����������֮���� $\dfrac{n}{2}-1$ �ߣ����������߶Աߣ�������λ����Щ���ϵ�ֱ�ߣ�����������λ������֮�䡢��������ε�ƽ�沿��һ��Ϳ����ɫ��

���գ�Mirko ѡ���� $q$ ���㣬�������� Slavko ѯ�ʣ�����ÿ�����Ƿ�λ����ɫ����ɫ���֡�

*The Biggest Loser* ��Ŀ������ʼ��Slavko û��ʱ��ش� Mirko �����⡣���ܰ�����


```input1
0
4
1 1
5 1
4 3
2 2
4
3 2
2 4
6 2
4 5

```

```output1
DA
NE
DA
NE
```

```input2
0
6
-1 -1
2 -1
3 3
2 4
1 4
-2 1
6
2 2
3 0
1 -6
2 6
-5 5
5 10

```

```output2
DA
DA
NE
NE
NE
NE
```

```input3
1
6
-1 -1
2 -1
3 3
2 4
1 4
-2 1
6
2 2
3 0
1 -6
2 6
-5 5
5 10

```

```output3
DA
DA
DA
NE
NE
NE
```

## ��ʾ
#### ���ݹ�ģ��Լ��

�������������ԡ�
| Subtask ��� | ��ֵ | ���ݷ�Χ |
| :-----------: | :-----------: | :-----------: |
| $1$ | $20$ | $1 \le n, q \le 2000$��$T = 0$|
| $2$ | $30$ | $1 \le n, q \le 10^5$��$T = 0$|
| $3$ | $60$ | $1 \le n, q \le 10^5$��$T = 1$|��

���⣬���� $100\%$ �����ݣ�$0 \le |x_i|, |y_i| \le 10^9, 0 \le |a_i|, |b_i| \le 2 \times 10^{18}$��

#### ˵��

**�����ֵ�� COCI ԭ�����ã����� $110$��**

**��Ŀ���� [COCI2019-2020](https://hsin.hr/coci/archive/2019_2020/) [CONTEST #2](https://hsin.hr/coci/archive/2019_2020/contest2_tasks.pdf) *T5 Zvijezda*��**



