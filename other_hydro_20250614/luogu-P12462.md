## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/9eg0us72.png)

## ��Ŀ����
��Ұ����櫸�����һ���� $T(V=\{V_1,V_2,\ldots,V_n\},E)$�����б�Ȩ $\omega: E \mapsto \mathbb{Z^+}$��

���� $S \subseteq E$ ��ȨֵΪ $\omega(S)=\sum_{e \in S} \omega(e)$��

���� $R(V',E')$ �� $T$ �� $\textbf{��ͨ����}$�����ҽ��� $R$ ������$V' \subseteq V$��$E' \subseteq E$��

���� $R$ ��Ȩֵ $\omega(R)=\omega(E')$��

���� $S \subseteq V$ �� Steiner ��Ϊ $f(S)=\min \{\omega(R) | S \subseteq V'\}$������ $R(V',E')$ ����ͨ������

�� $q$ ��ѯ�ʣ��� $i$ �θ��� $L_i,R_i,k_i$���� $\max \{f(S) | S \subseteq \{V_{L_i},V_{L_{i}+1},\ldots,V_{R_i}\},|S|=k_i\}$��

## �����ʽ
��һ��һ������ $n$��

���� $n-1$ �У�ÿ���������� $a,b,z$����ʾ $(V_a,V_b) \in E$���� $\omega[(V_a,V_b)]=z$����֤ $1 \le z \le 10^9$��

����һ��һ������ $q$��

���� $q$ �У��� $i$ ���������� $L_i,R_i,k_i$. ��֤ $1 \le L_i \le L_i + k_i - 1 \le R_i \le n$��

## �����ʽ
$q$ �У�ÿ��һ��������ʾ�𰸡�

```input1
10
1 2 2
2 3 3
3 4 2
1 5 7
2 6 7
4 7 1
1 8 3
4 9 6
7 10 4
10
5 10 5
4 9 6
10 10 1
2 6 3
6 9 3
6 9 4
7 9 2
1 3 2
1 7 3
3 8 3
```

```output1
35
31
0
21
23
24
16
5
22
22
```

## ��ʾ
Idea��nzhtl1477��Solution��rushcheyo&nzhtl1477��Code��rushcheyo��Data��rushcheyo

����������������⡣

�� $K=\max\{k_i\}$��

���������ݣ���֤ $1 \le n \le 3 \times 10^5,1 \le q \le 10^4,K \le 100$.

1. $n,q \le 10$��15 �֣���

2. $n,q \le 100$��15 �֣���
3. $n,q \le 1000$��10 �֣���
4. $n,q \le 5000$��10 �֣���
5. $K=2$��15 �֣���
6. $K=3$��15 �֣���
7. $K \le 10$��10 �֣���
8. û���������ʣ�10 �֣���

