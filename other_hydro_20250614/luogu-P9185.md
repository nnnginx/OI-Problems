## ��Ŀ����
**Note: The time limit for this problem is 4s, 2x the default.**

To celebrate the start of spring, Farmer John's $N$ cows have invented an intriguing new dance, where they stand in a circle and re-order themselves in a predictable way.

Specifically, there are $N$ positions around the circle, numbered sequentially from $0$ to $N-1$, with position $0$ following position $N-1$.  A cow resides at each position.  The cows are also numbered sequentially from $0$ to $N-1$.  Initially, cow $i$ starts in position $i$.  You are told a set of $K$ positions $0=A_1<A_2<\dots<A_K<N$ that are "active", meaning the cows in these positions are the next to move.

In each minute of the dance, two things happen.  First, the cows in the active positions rotate: the cow at position $A_1$ moves to position $A_2$, the cow at position $A_2$ moves to position $A_3$, and so on, with the cow at position $A_K$ moving to position $A_1$.  All of these $K$ moves happen simultaneously, so the after the rotation is complete, all of the active positions still contain exactly one cow.  Next, the active positions themselves shift:
$A_1$ becomes $A_1+1$, $A_2$ becomes $A_2+1$, and so on (if $A_i = N-1$ for some active position, then $A_i$ circles back around to $0$).

Please calculate the order of the cows after $T$ minutes of the dance.

## �����ʽ
The first line contains three integers $N, K$ and $T$.

The second line contains $K$ integers representing the initial set of active positions
$A_1,A_2, \dots, A_K$.  Recall that $A_1 = 0$ and that these are given in increasing order.

## �����ʽ
Output the order of the cows after $T$ minutes, starting with the cow in position $0$, separated by
spaces.

## ��Ŀ����
### ��Ŀ����

**ע�⣺�����ʱ������Ϊ 4 �룬��Ĭ��ʱ�����Ƶ� 2 ����**

Ϊ����ף����ĵ�����Farmer John �� $N$ ͷ��ţ������һ����Ȥ���赸������Χ��һ��ԲȦ������һ�ֿ�Ԥ��ķ�ʽ���������Լ���

������˵��ԲȦ���� $N$ ��λ�ã���Ŵ� $0$ �� $N-1$������λ�� $0$ ������λ�� $N-1$��ÿ��λ������һͷ��ţ����ţ�ı��Ҳ�� $0$ �� $N-1$����ʼʱ����ţ $i$ λ��λ�� $i$����ᱻ��֪һ�� $K$ ������Ծ��λ�� $0 = A_1 < A_2 < \dots < A_K < N$������ζ����Щλ���ϵ���ţ����һ��Ҫ�ƶ��ġ�

���赸��ÿһ���ӣ��ᷢ�������¡����ȣ���Ծλ���ϵ���ţ����ת��λ�� $A_1$ ����ţ�ƶ���λ�� $A_2$��λ�� $A_2$ ����ţ�ƶ���λ�� $A_3$���������ƣ�λ�� $A_K$ ����ţ�ƶ���λ�� $A_1$��������Щ $K$ ���ƶ�ͬʱ�������������ת��ɺ����л�Ծλ����Ȼǡ����һͷ��ţ������������Ծλ�ñ�����ƶ���$A_1$ ��Ϊ $A_1 + 1$��$A_2$ ��Ϊ $A_2 + 1$���������ƣ����ĳ����Ծλ�� $A_i = N-1$���� $A_i$ ��ѭ���ص� $0$����

������赸���� $T$ ���Ӻ���ţ��˳��

### �����ʽ

��һ�а����������� $N$��$K$ �� $T$��

�ڶ��а��� $K$ ����������ʾ��ʼ�Ļ�Ծλ�� $A_1, A_2, \dots, A_K$��ע�� $A_1 = 0$��������Щλ���ǰ�����˳������ġ�

### �����ʽ

��� $T$ ���Ӻ���ţ��˳�򣬴�λ�� $0$ ����ţ��ʼ���ÿո�ָ���

### ��ʾ

��������������������ǰ�ĸ�ʱ�䲽����ţ˳��ͻ�Ծλ�� $A$��
```
��ʼ��T = 0��˳�� = [0 1 2 3 4]��A = [0 2 3]
T = 1��˳�� = [3 1 0 2 4]
T = 1��A = [1 3 4]
T = 2��˳�� = [3 4 0 1 2]
T = 2��A = [2 4 0]
T = 3��˳�� = [2 4 3 1 0]
T = 3��A = [3 0 1]
T = 4��˳�� = [1 2 3 4 0]
```

$1 \leq K \leq N \leq 2 \cdot 10^5$��$1 \leq T \leq 10^9$��

- ���� 2-7��$N \leq 1000$��$T \leq 10000$��
- ���� 8-13��û�ж������ơ�

```input1
5 3 4
0 2 3

```

```output1
1 2 3 4 0

```

## ��ʾ
For the example above, here are the cow orders and $A$ for the first four timesteps:
```
Initial, T = 0: order = [0 1 2 3 4], A = [0 2 3]
T = 1: order = [3 1 0 2 4]
T = 1: A = [1 3 4]
T = 2: order = [3 4 0 1 2]
T = 2: A = [2 4 0]
T = 3: order = [2 4 3 1 0]
T = 3: A = [3 0 1]
T = 4: order = [1 2 3 4 0]
```

$1 \leq K \leq N \leq 2 \cdot 10^5$, $1\le T\le 10^9$.

- Inputs 2-7: $N \leq 1000, T \leq 10000$.
- Inputs 8-13: No additional constraints.

