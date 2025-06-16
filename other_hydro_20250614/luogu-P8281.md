## ��Ŀ����
Technoblade �� Skyblock ����Ϊһ�� $n$��$n\le 50$���ڵ� $m$ ���ߵļ�����ͼ������Ҫ�����ͼ **����** ���ܶ��ٻ�·������������ $p_1,p_2,\dots,p_n$ ʹ�� $p_1=1$ ���� $p_1\to p_2\to \dots\to p_{n-1}\to p_n\to p_1$ Ϊһ���Ϸ�·����

**���ݱ�֤���ܶ��ٻ�·�������㲢С�� $10^4$**��

**���ݴ����кϷ��������������**

## �����ʽ
��һ������������ $n,m$��

������ $m$ �У�ÿ������������ $u,v$��

## �����ʽ
��������У�ÿ����� $n$ ����������Ϊһ�����ܶ��ٻ�·�����յ����ֵ��������

```input1
3 3
1 2
2 3
3 1
```

```output1
1 2 3
```

```input2
4 6
1 3
1 4
2 1
2 3
3 4
4 2
```

```output2
1 3 4 2
```

```input3
5 8
1 2
2 3
3 4
4 1
2 5
4 5
5 1
5 3
```

```output3
1 2 3 4 5
1 2 5 3 4
```

```input4
5 10
1 2
1 3
2 3
2 4
3 4
3 5
4 1
4 5
5 1
5 2
```

```output4
1 2 3 4 5
1 3 5 2 4
```

```input5
6 15
1 3
1 4
1 5
2 1
2 3
2 4
3 1
3 4
4 2
4 6
5 2
5 3
6 1
6 2
6 3
```

```output5
1 5 2 3 4 6
1 5 2 4 6 3
1 5 3 4 6 2
```

```input6
6 15
1 3
1 5
2 1
2 4
3 1
3 2
3 4
3 5
3 6
4 6
5 1
5 4
5 6
6 3
6 5
```

```output6
1 3 2 4 6 5
1 5 4 6 3 2
```

```input7
6 16
1 3
1 6
2 3
2 4
2 6
3 1
3 6
4 2
4 3
4 5
4 6
5 2
5 6
6 1
6 3
6 5
```

```output7
1 6 5 2 4 3
```

```input8
6 21
1 2
1 5
1 6
2 1
2 3
2 4
2 5
3 1
3 2
3 4
3 6
4 1
4 2
4 6
5 1
5 2
5 4
5 6
6 2
6 3
6 4
```

```output8
1 2 5 4 6 3
1 2 5 6 3 4
1 5 2 3 6 4
1 5 2 4 6 3
1 5 4 6 2 3
1 5 4 6 3 2
1 5 6 2 3 4
1 5 6 3 2 4
1 5 6 3 4 2
1 5 6 4 2 3
1 6 3 2 5 4
1 6 3 4 2 5
```

## ��ʾ
#### ���� 1 ����

![](https://cdn.luogu.com.cn/upload/image_hosting/lth4lrb1.png)

�� $1$ �����ܶ��ٻ�·��

 - $1\to2\to3\to1$��

#### ���� 2 ����

![](https://cdn.luogu.com.cn/upload/image_hosting/if0vz8gm.png)

�� $1$ �����ܶ��ٻ�·��

 - $1\to3\to4\to2\to1$��

#### ���� 3 ����

![](https://cdn.luogu.com.cn/upload/image_hosting/dv1tul62.png)

�� $2$ �����ܶ��ٻ�·��

 - $1\to2\to3\to4\to5\to1$��
 - $1\to2\to5\to3\to4\to1$��

#### ���� 4 ����

![](https://cdn.luogu.com.cn/upload/image_hosting/wggv2mfd.png)

�� $2$ �����ܶ��ٻ�·��

 - $1\to2\to3\to4\to5\to1$��
 - $1\to3\to5\to2\to4\to1$��

#### ���� 5 ����

![](https://cdn.luogu.com.cn/upload/image_hosting/cfi80wob.png)

�� $3$ �����ܶ��ٻ�·��

 - $1\to5\to2\to3\to4\to6\to1$��
 - $1\to5\to2\to4\to6\to3\to1$��
 - $1\to5\to3\to4\to6\to2\to1$��

#### ���� 6 ����

![](https://cdn.luogu.com.cn/upload/image_hosting/wqd9tpl8.png)

�� $2$ �����ܶ��ٻ�·��

 - $1\to3\to2\to4\to6\to5\to1$��
 - $1\to5\to4\to6\to3\to2\to1$��

#### ���� 7 ����

![](https://cdn.luogu.com.cn/upload/image_hosting/jff0k373.png)

�� $1$ �����ܶ��ٻ�·��

 - $1\to6\to5\to2\to4\to3\to1$��

#### ���� 8 ����

![](https://cdn.luogu.com.cn/upload/image_hosting/x2j19zoc.png)

�� $12$ �����ܶ��ٻ�·��

 - $1\to2\to5\to4\to6\to3\to1$��
 - $1\to2\to5\to6\to3\to4\to1$��
 - $1\to5\to2\to3\to6\to4\to1$��
 - $1\to5\to2\to4\to6\to3\to1$��
 - $1\to5\to4\to6\to2\to3\to1$��
 - $1\to5\to4\to6\to3\to2\to1$��
 - $1\to5\to6\to2\to3\to4\to1$��
 - $1\to5\to6\to3\to2\to4\to1$��
 - $1\to5\to6\to3\to4\to2\to1$��
 - $1\to5\to6\to4\to2\to3\to1$��
 - $1\to6\to3\to2\to5\to4\to1$��
 - $1\to6\to3\to4\to2\to5\to1$��

#### ���ݹ�ģ��Լ��

���ڹ̶� $n$ �� $P$������һ�� $m$ ���ߵ�ͼȨ��Ϊ $\left(\frac{1}{P}\right)^m\left(\frac{P-1}{P}\right)^{n^2-n-m}$��

 - Subtask 1��1 pts����Ϊ������
 - Subtask 2��16 pts����$n=15$��
 - Subtask 3��20 pts����$n=30$��
 - Subtask 4��26 pts����$n=40$��
 - Subtask 5��37 pts����$n=50$��


