## ��Ŀ����
Farmer John and his personal trainer Bessie are hiking up Mount Vancowver. For their purposes (and yours), the mountain can be represented as a long straight trail of length $L$ meters ($1 \leq L \leq 10^6$). Farmer John will hike the trail at a constant travel rate of $r_F$ seconds per meter ($1 \leq r_F \leq 10^6$). Since he is working on his stamina, he will not take any rest stops along the way.
Bessie, however, is allowed to take rest stops, where she might find some tasty grass. Of course, she cannot stop just anywhere! There are $N$ rest stops along the trail ($1 \leq N \leq 10^5$); the $i$-th stop is $x_i$ meters from the start of the trail ($0 < x_i < L$) and has a tastiness value $c_i$ ($1 \leq c_i \leq 10^6$). If Bessie rests at stop $i$ for $t$ seconds, she receives $c_i \cdot t$ tastiness units.

When not at a rest stop, Bessie will be hiking at a fixed travel rate of $r_B$ seconds per meter ($1 \leq r_B \leq 10^6$). Since Bessie is young and fit, $r_B$ is strictly less than $r_F$.

Bessie would like to maximize her consumption of tasty grass. But she is worried about Farmer John; she thinks that if at any point along the hike she is behind Farmer John on the trail, he might lose all motivation to continue!

Help Bessie find the maximum total tastiness units she can obtain while making sure that Farmer John completes the hike.

## �����ʽ
The first line of input contains four integers: $L$, $N$, $r_F$, and $r_B$. The next $N$ lines describe the rest stops. For each $i$ between $1$ and $N$, the $i+1$-st line contains two integers $x_i$ and $c_i$, describing the position of the $i$-th rest stop and the tastiness of the grass there.
It is guaranteed that $r_F > r_B$, and $0 < x_1 < \dots < x_N < L $. **Note that $r_F$ and $r_B$ are given in seconds per meter!**

## �����ʽ
A single integer: the maximum total tastiness units Bessie can obtain.

## ��Ŀ����
### ��Ŀ����

Farmer John ������˽�˽��� Bessie �����ʵ��¸绪ɽ��Ϊ�����ǵ�Ŀ�ģ��Լ����Ŀ�ģ�������ɽ���Ա�ʾΪһ������Ϊ $L$ �׵ĳ�ֱ������$1 \leq L \leq 10^6$����Farmer John ����ÿ�� $r_F$ ��ĺ㶨�ٶ�ͽ����$1 \leq r_F \leq 10^6$�������������ڶ�����������������;����Ϣ��

Ȼ����Bessie ����������Ϣվ��Ϣ�������ܻ��������ҵ�һЩ��ζ�Ĳݡ���Ȼ�����������ͣ�������������� $N$ ����Ϣվ��$1 \leq N \leq 10^5$������ $i$ ����Ϣվ���벽����� $x_i$ �ף�$0 < x_i < L$����������һ����ζֵ $c_i$��$1 \leq c_i \leq 10^6$������� Bessie �ڵ� $i$ ����Ϣվ��Ϣ $t$ �룬������ $c_i \cdot t$ ����ζ��λ��

��������Ϣվʱ��Bessie ����ÿ�� $r_B$ ��Ĺ̶��ٶ�ͽ����$1 \leq r_B \leq 10^6$�������� Bessie �����ҽ�����$r_B$ �ϸ�С�� $r_F$��

Bessie ϣ��������������ζ�������������� Farmer John������Ϊ�����ͽ�����κ�ʱ�����ڲ���������� Farmer John�������ܻ�ʧȥ����ǰ���Ķ�����

����� Bessie �ҵ���ȷ�� Farmer John ���ͽ��������£����ܻ�õ��������ζ��λ��

### �����ʽ

����ĵ�һ�а����ĸ�������$L$��$N$��$r_F$ �� $r_B$���������� $N$ ����������Ϣվ������ÿ�� $i$ �� $1$ �� $N$���� $i+1$ �а����������� $x_i$ �� $c_i$���ֱ������� $i$ ����Ϣվ��λ�úͲݵ���ζֵ��
��֤ $r_F > r_B$���� $0 < x_1 < \dots < x_N < L$��**ע�⣬$r_F$ �� $r_B$ �ĵ�λ����ÿ�ף�**

### �����ʽ

���һ��������Bessie �ܻ�õ��������ζ��λ��


### ��ʾ

����������У�Bessie ���ŵĲ������� $x=7$ ����Ϣվ��Ϣ $7$ �루��� $14$ ����ζ��λ����Ȼ���� $x=8$ ����Ϣվ����Ϣ $1$ �루��� $1$ ����ζ��λ���ܹ� $15$ ����ζ��λ����

```input1
10 2 4 3
7 2
8 1
```

```output1
15
```

## ��ʾ
In this example, it is optimal for Bessie to stop for $7$ seconds at the $x=7$ rest stop (acquiring $14$ tastiness units) and then stop for an additional $1$ second at the $x=8$ rest stop (acquiring $1$ more tastiness unit, for a total of $15$ tastiness units).

Problem credits: Dhruv Rohatgi

