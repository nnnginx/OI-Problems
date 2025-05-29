## ��Ŀ����
���������� $a, b$������ $R(a, b)$ Ϊ��  

 $\begin{cases}R(b,a)&a<b\\R\left(\left\lfloor\dfrac{a}{b}\right\rfloor,b\right)&1<b\leq a\\a&1=b\leq a\end{cases}$
 
���������� $g, h$���������� $a, b$ ʹ�� $\gcd(a,b)=g$��$R(a,b)=h$��

## �����ʽ
��һ��һ������ $T$����������������  
������ $T$ ��ÿ������������ $g_i, h_i$��

## �����ʽ
��� $T$ �У�ÿ��������������������� $a_i, b_i$��  
Ҫ�� $a, b$ �������� $10^{18}$��  
����֤��һ������������� $a, b$�����ж�����������һ�鼴�ɡ�

```input1
1
1 4
```

```output1
99 23
```

```input2
2
3 2
5 5
```

```output2
9 39
5 5
```

## ��ʾ
**���������� #1��**

$\gcd(99,23)=1$��$R(99,23)=4$

**�����ݷ�Χ��**

���� $100\%$ �����ݣ�$1 \leq g \leq 200,000$��$2 \leq h \leq 200,000$��

Subtask #1��$4$ pts����$g=h$��  
Subtask #2��$7$ pts����$h=2$��  
Subtask #3��$7$ pts����$g=h^2$��  
Subtask #4��$14$ pts����$g,h \leq 20$��  
Subtask #5��$36$ pts����$g,h \leq 2000$��  
Subtask #6��$32$ pts�����޸���Լ����

**��˵����**

���� [Croatian Open Competition in Informatics 2020 ~ 2021 Round 2 C Euklid](https://hsin.hr/coci/contest2_tasks.pdf)��

