## ��Ŀ����
Farmer John ���������һ����Ϸ�����������������ı��硣


## ��Ŀ����
Farmer John has challenged Bessie to the following game: FJ has a board with dots marked at N (2 �� N �� 200) distinct lattice points. Dot i has the integer coordinates Xi and Yi (-1,000 �� Xi �� 1,000; -1,000 �� Yi �� 1,000).

Bessie can score a point in the game by picking two of the dots and drawing a straight line between them; however, she is not allowed to draw a line if she has already drawn another line that is parallel to that line. Bessie would like to know her chances of winning, so she has asked you to help find the maximum score she can obtain.

��Ϸ��ʼ��ʱ ��FJ �������һ�黭�� $N (2 \le N \le 200)$ �����غϵĵ��ľ�壬���е� $i$ ����ĺᡢ������ֱ�Ϊ $X_i$ �� $Y_i (-1000 \le X_i \le 1000, -1000 \le Y_i \le 1000)$��

�������ѡ�����㻭һ�������ǵ�ֱ�ߣ����ҽ���ƽ���ϲ������뻭��ֱ�� ƽ�е�ֱ�ߡ���Ϸ����ʱ����ĵ÷֣�������������ֱ�ߵ���������Ϊ������Ϸ��ʤ���������ҵ����㣬ϣ�����������һ�������ܵ÷֡�


## �����ʽ
�� $1$ ��: ���� 1 ����������$N$

�� $2 \cdots N+1$ ��: �� $i+1$ ���� $2$ ���ÿո����������$X_i,Y_i$�������˵� $i$ �����ꡣ


## �����ʽ
�� 1 ��: ��� 1 ����������ʾ��������÷֣������ܻ����Ļ���ƽ�е��߶���


```input1
4 
-1 1 
-2 0 
0 0 
1 1
```

```output1
4 
```

## ��ʾ
�����ܻ������� $4$ ��б�ʵ�ֱ�ߣ�$-1$��$0$��$\dfrac{1}{3}$ �Լ� $1$��

