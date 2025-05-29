## ��Ŀ����
���������� $\texttt{MhxMa}$ �������⣬�����Ѿ��� $\texttt{Ferm\_Tawn}$ ���ˣ���ʱ $\texttt{MhxMa}$ ���ڵ�����ǰ����������Ҫ��õ����ݣ��������Լ������ѵ�һ��Ƭѡ�ֵ����������ˡ�

## ��Ŀ����
����һ����Ծ��Ϸ������Ϸ���������������λ�ã������� $n$ ���㣺$1 , 2 , 3, \cdots , n$������������н������� $a_1 , a_2 , \cdots , a_n$��

��Ȼ�������Ϸ�ܼ򵥣�$\texttt{MhxMa}$ û����þͻ�������з��������ǸĽ��˴��룬����˾���ֵ���������

�����н��������� $n$ ���㣬���ӵ� $x$ ������ $y$�����þ���ֵ $\operatorname{score}_{x , y}(1\le x\le y\le n)$��

$$\operatorname{score}_{x,y}=\begin{cases}\operatorname{len}  & \operatorname{gcd}(a_x , a_{x+1} , \dots , a_y)=2 , \operatorname{len \ mod} 2 = 0  \\ \operatorname{len} &\gcd(a_x , a_{x + 1} , \dots , a_y)=3 , \operatorname{len \ mod} 2 = 1\\ 0 & \operatorname{others} \end{cases}$$

���У�$\operatorname {len}$ ��ʾ����ĳ��ȣ��� $y-x+1$��

**����ÿһ��λ�� $(x,y)$�������Ծֻ����һ�ξ���ֵ��**

Ϊ���� $\texttt{MhxMa}$ չ����ı��ʵ���������дһ��������������Ϸ��ˢ���������ֵ��

## �����ʽ
���빲���С�

�����һ�а���һ������ $n$��

�ڶ��а��� $n$ ������ $a_i$��

## �����ʽ
���һ����������ʾ�𰸡�

```input1
5
2 3 6 3 9
```

```output1
8
```

```input2
5
2 2 2 2 2
```

```output2
16
```

```input3
9
6 2 3 6 4 6 8 2 5
```

```output3
19
```

## ��ʾ
**��ʹ�ýϿ�Ķ��뷽ʽ��**

### �������� #1

$\operatorname{score_{2 , 2}}= 1$��

$\operatorname{score_{2 , 4}}= 3$��

$\operatorname{score_{3 , 5}}= 3$��

$\operatorname{score_{4 , 4}}= 1$��

$1+3+3+1=8$��

### �������� #2

$\operatorname{score_{1 , 2}}= 2$��

$\operatorname{score_{1 , 4}}= 4$��

$\operatorname{score_{2 , 3}}= 2$��

$\operatorname{score_{2 , 5}}= 4$��

$\operatorname{score_{3 , 4}}= 2$��

$\operatorname{score_{4 , 5}}= 2$��

$2+ 4 + 2 + 4 + 2 + 2 = 16$��

------------
### ���ݹ�ģ��Լ��

**��������������**��

- Subtask 0��20 pts����$n \le 10^2$�� 

- Subtask 1��10 pts����$n \le 2 \times 10^3$��

- Subtask 2��20 pts����$n \le 10^4$��

- Subtask 3��50 pts����$n \le 6 \times 10^5 $��


�������в������ݣ�$1 \le n \le 6 \times 10^5$��$1 \le a_i \le 10^7$��

