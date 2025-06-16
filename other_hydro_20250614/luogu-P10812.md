## ��Ŀ����
ԭ�����ӣ�<https://oier.team/problems/S2C>��

---

![](https://cdn.luogu.com.cn/upload/image_hosting/kq7nqgu8.png)

~~��һ�������һ��~~

~~����������ͽ������Լ��ҡ�~~

## ��Ŀ����
����һ�������ᣬ��Χ�� $1\sim n$��ÿ���� $i$ �������� $i+1$��$i+1\le n$���� $i-1$��$i-1\ge 1$�����������Ӵ���ÿ����ֻ�ܵ���һ�Ρ��ʴӵ� $n$ ���� $1$ һ���ж��ٷ������𰸶� $p$ ȡģ��

���ַ�����ͬ���ҽ�������һ����Ծ���λ�ò�ͬ�����һ����Ծ�����಻ͬ��

## �����ʽ
һ���������� $n,p$��

## �����ʽ
һ��һ����������ʾ�𰸶� $p$ ȡģ��Ľ����

```input1
3 1000000007
```

```output1
3
```

```input2
4 1000
```

```output2
7
```

```input3
100 511609
```

```output3
272799
```

## ��ʾ
**���������� \#1��**

�� $\rightarrow$ ��ʾ���ϻ���������$\Rightarrow$ ��ʾ�����ӡ������ַ������¡�
+ $3\Rightarrow1$
+ $3\rightarrow2\rightarrow1$
+ $3\rightarrow2\Rightarrow1$

**���������� \#2��**

�� $\rightarrow$ ��ʾ���ϻ���������$\Rightarrow$ ��ʾ�����ӡ������ַ������¡�

+ $4\rightarrow3\Rightarrow1$
+ $4\rightarrow3\rightarrow2\rightarrow1$
+ $4\rightarrow3\rightarrow2\Rightarrow1$
+ $4\Rightarrow2\rightarrow3\Rightarrow1$
+ $4\Rightarrow2\rightarrow1$
+ $4\Rightarrow2\Rightarrow1$
+ $4\Rightarrow1$

**�����ݷ�Χ��**

**�������������ԡ�**

- Subtask 0��8 pts����$n\le20$��
- Subtask 1��11 pts����$n\le150$��
- Subtask 2��23 pts����$n\le300$��
- Subtask 3��26 pts����$n\le1000$��
- Subtask 4��32 pts�������������ơ�

�������в������ݣ�$1\le n\le5\times10^3$��$2\le p\le 10^9+7$��

