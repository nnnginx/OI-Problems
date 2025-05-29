## ��Ŀ����
Passport is a certificate which is used worldwide when a traveler enters foreign countries.

In a planet, there are $N$ countries, numbered from $1$ to $N$. Each country issues a passport. When a traveler has a passport issued by the country $i \ (1 \le i \le N)$, the traveler can enter the countries $L_i, L_{i + 1}, \dots, R_i$. **Here, it is guaranteed that the traveler can enter the country where the passport was issued. Namely, $L_i \le i \le R_i$ is satisfied.**

You have a friend who likes traveling. Although he dreams of traveling around the world, he does not have a passport in the beginning. Thus, he plans to visit all of the $N$ countries by repeating the following two actions.

- He gets a passport issued by the country where he is currently staying.
- He moves to a country where he can enter using a passport he currently has.

When you hear about his plan, you are wondering whether it is possible to realize the plan, and, if it is possible, what is the minimum number of passports he needs to get. Since you do not know where he lives, you consider $Q$ possible countries $X_1, X_2, \dots, X_Q$ where he lives.

Write a program which, given information of the passports and the possibilities of his living place, for each possibility, determines whether it is possible for him to visit all of the $N$ countries, and, if it is possible, calculates the minimum number of passports he needs to get.

## �����ʽ
Read the following data from the standard input.

> $N$
>
> $L_1 \ R_1$
>
> $L_2 \ R_2$
>
> $\vdots$
>
> $L_N \ R_N$
>
> $Q$
>
> $X_1$
>
> $X_2$
>
> $\vdots$
>
> $X_Q$

## �����ʽ
Write $Q$ lines to the standard output. The $j$-th line $(1 \le j \le Q)$ corresponds to the case where your friend lives in the country $X_j$. If it is possible for him to visit all of the $N$ countries, this line should contain the minimum number of passports he needs to get. Otherwise, this line should contain $-1$.

## ��Ŀ����
## ��Ŀ����

���������мҽ�������ʱʹ�õ�֤����

��һ���������� $N$ �����ң��� $1$ �� $N$ ��š�ÿ�����Ҷ�ǩ��һ�ֻ��ա������мһ���ɹ���$i \ (1 \le i \le N)$ ǩ���Ļ��պ����ܹ�������� $L_i, L_{i + 1}, \dots, R_i$��**���ﱣ֤���м��ܹ�������ǩ֤��ǩ��������ʽ�ϵ�˵, $L_i \le i \le R_i$ ��Ȼ������**

����һ�������е����ѡ���ʹ�������ܻ������磬�������һ�ֻ���Ҳû�С���ˣ�����ͨ��һ���ظ�����������Ϊ�������� $N$ �����ҡ�

- �������ǰ���ڹ���ǩ���Ļ��ա�
- �������еĻ��ս���ĳ�����ҡ�

֪�����ļƻ�������֪������ƻ����Ƿ���У���������еĻ�����������Ҫ�Ļ�����������Ϊ�㲢��������������ι���������Ԥ���� $Q$ ������������ס���ǵĹ��� $X_1, X_2, \dots, X_Q$��

���ڸ����������յ���Ϣ $L_i, R_i$ �������ܾ�ס�� $Q$ �����ң�����Ҫдһ�����򣬶���ÿһ�����ܾ�ס�Ĺ��ң��ж����Ƿ���ܻ����� $N$ �����ң�������ܵĻ������������Ҫ�����ٻ���������

## �����ʽ

�ӱ�׼������룺

> $N$
>
> $L_1 \ R_1$
>
> $L_2 \ R_2$
>
> $\vdots$
>
> $L_N \ R_N$
>
> $Q$
>
> $X_1$
>
> $X_2$
>
> $\vdots$
>
> $X_Q$

## �����ʽ

��� $Q$ ������׼������� $j \ (1 \le j \le Q)$ ��һ�������������������λ�ڹ��� $X_j$ �Ĵ𰸡������ܻ����� $N$ �����ң����������Ҫ�����ٻ���������������� $-1$��

## ��ʾ

**���������� #1��**

����������Ѿ�ס�ڹ��� $X_1 = 1$��һ�ֿ��еķ�ʽ���£����������� $2$ �ֻ��գ�

1. ��ù��� $1$ ǩ���Ļ��ա�
2. �ù��� $1$ ǩ���Ļ���ȥ���� $2$ ���С�
3. ��ù��� $2$ ǩ���Ļ��ա�
4. �ù��� $1$ ǩ���Ļ���ȥ���� $3$ ���С�
5. �ù��� $2$ ǩ���Ļ���ȥ���� $4$ ���С�

����֤��������ʹ�û���������С�ķ���������� $2$��

������������������������ơ�

**���������� #2��**

����������Ѿ�ס�ڹ��� $X_1 = 3$��һ�ֿ��еķ�ʽ���£����������� $4$ �ֻ��գ�

1. ��ù��� $3$ ǩ���Ļ��ա�
2. �ù��� $3$ ǩ���Ļ���ȥ���� $2$ ���С�
3. ��ù��� $2$ ǩ���Ļ��ա�
4. �ù��� $2$ ǩ���Ļ���ȥ���� $4$ ���С�
5. ��ù��� $4$ ǩ���Ļ��ա�
6. �ù��� $4$ ǩ���Ļ���ȥ���� $5$ ���С�
7. ��ù��� $5$ ǩ���Ļ��ա�
8. �ù��� $5$ ǩ���Ļ���ȥ���� $1$ ���С�

����֤��������ʹ�û���������С�ķ���������� $4$��

���������������� $2 \sim 5$ �����ơ�

**���������� #3��**

���磬���������Ѿ�ס�� $X_3 = 3$��һ�ֿ��еķ������ù��� $3$ ǩ���Ļ��գ�������������ȥ���� $1, 2, 4, 5$ ���С��ʵ�������� $3$��

�����������Ѿ�ס�ڹ��� $X_5 = 5$����ʹ������˹��� $5$ ǩ���Ļ��գ���Ҳ�����ܽ����κ��������ң���ˣ����޷�ʵ���Լ������мƻ����ʵ�������� $-1$��

���������������� $4 \sim 5$ �����ơ�

**���������� #4��**

���������������� $4 \sim 5$ �����ơ�

```input1
4
1 3
2 4
2 3
4 4
1
1

```

```output1
2

```

```input2
5
1 5
2 4
2 3
3 5
1 5
1
3

```

```output2
4

```

```input3
5
1 1
2 3
1 5
3 4
5 5
5
1
2
3
4
5

```

```output3
-1
2
1
2
-1

```

```input4
4
1 2
1 2
3 4
3 4
4
1
2
3
4

```

```output4
-1
-1
-1
-1

```

## ��ʾ
**���������� #1��**

Assume that your friend lives in the country $X_1 = 1$. It is possible for him to visit all of the $4$ countries if he acts in the following way. Then, he gets $2$ passports.

1. He gets a passport issued by the country $1$.
2. Using the passport issued by the country $1$, he moves to the country $2$.
3. He gets a passport issued by the country $2$.
4. Using the passport issued by the country $1$, he moves to the country $3$.
5. Using the passport issued by the country $2$, he moves to the country $44.

Since it is impossible to realize the plan if he gets less than or equal to $1$ passport, output $2$.

������������������������ơ�

**���������� #2��**

Assume that your friend lives in the country $X_1 = 3$. It is possible for him to visit all of the $5$ countries if he acts in the following way. Then, he gets $4$ passports.
1. He gets a passport issued by the country $3$.
2. Using the passport issued by the country $3$, he moves to the country $2$.
3. He gets a passport issued by the country $2$.
4. Using the passport issued by the country $2$, he moves to the country $4$.
5. He gets a passport issued by the country $4$.
6. Using the passport issued by the country $4$, he moves to the country $5$.
7. He gets a passport issued by the country $5$.
8. Using the passport issued by the country $5$, he moves to the country $1$.

Since it is impossible to realize the plan if he gets less than or equal to $3$ passports, output $4$.

���������������� $2 \sim 5$ �����ơ�

**���������� #3��**

For example, if your friend lives in the country $X_3 = 3$, it is possible to realize the plan if he gets a passport issued by the country $3$, and uses it to visit the countries $1, 2, 4, 5$ in this order. Therefore, output $1$ in the third line.

On the other hand, if your friend lives in the country $X_5 = 5$, it is impossible for him to enter other countries even if he gets a passport issued by the country $5$. Thus, he cannot realize the plan. Therefore, output $-1$ in the fifth line.

���������������� $4 \sim 5$ �����ơ�

**���������� #4��**

���������������� $4 \sim 5$ �����ơ�

**�����ݷ�Χ��**

�������в������ݣ����� $2 \le N \le 2 \times 10 ^ 5$��$1 \le L_i \le i \le R_i \le N$��$1 \le Q \le N$��$1 \le X_1 < X_2 < \dots < X_Q \le N$����֤���������Ϊ������

|��������|��ֵ|����|
|:-:|:-:|:-:|
|$1$|$6$|$Q = 1$��$X_1 = 1$|
|$2$|$16$|$N \le 300$��$Q = 1$|
|$3$|$24$|$N \le 2500$��$Q = 1$|
|$4$|$8$|$N \le 2500$|
|$5$|$46$|��|

