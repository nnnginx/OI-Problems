## ��Ŀ����
���� $n$ ����ѧ����ʽ��

ÿ�����뷴Ӧ�ķ��������ɸ�ԭ����ɣ�ÿ��ԭ����һ����ĸ��һ�����ֱ�ʾ���ֱ����Ԫ�����ƺͷ����и�ԭ�ӵ����������������Ӳ��뷴Ӧ�������ǰ���һ�����ֱ�ʾ��ѧ��������������ֻ�迼��ÿһԭ�ӵ������������ؿ��Ƿ���ʽ�ĺ����ԡ����磬$\texttt{3AC4B}$ ����ֱ����Ϊ $3$ �� $\texttt A$��$3$ �� $\texttt B$ �� $12$ �� $\texttt C$ ���뷴Ӧ�����в�ͬ����λ�ڷ���ʽͬһ��ʱ���� $\texttt +$ ���ӡ�

��������Ƿֱ���ÿ������ʽ�Ƿ��Ѿ���ƽ��ֻ�迼������ԭ�������Ƿ񶼶�Ӧ��ȣ���

## �����ʽ
��һ��һ�������� $n$����ʾ����ʽ�ĸ�����

�������� $n$ �У�ÿ��һ������ʽ�����ݱ�֤ÿ������ʽ�ַ������Ȳ����� $1000$����ÿ��Ԫ�ض�ֻ����һ����д��ĸ��

## �����ʽ
����ÿ������ʽ������Ѿ���ƽ����� $\texttt{DA}$��������� $\texttt{NE}$��

```input1
3
A+B->AB
AB+CD->AC+DB
AB+B->AB
```

```output1
DA
DA
NE
```

```input2
2
2AB+A->3AB
2AB+2AC+2BC->4ABC
```

```output2
NE
DA
```

```input3
4
2H2O+2CO2->2H2CO3
H2SO4->H2O4
NH3+H2SO4->NH4SO4
CH4+2O2->CO2+2H2O
```

```output3
DA
NE
NE
DA
```

## ��ʾ
**������ 3 ���͡�**

|���|���ԭ��|�Ҳ�ԭ��|���|
| :----------: | :----------: | :----------: | :----------: |
|$1$|$4 \times \texttt H, 6 \times \texttt O, 2 \times \texttt C$|$4 \times \texttt H, 6 \times \texttt O, 2 \times \texttt C$|$\green{\texttt{DA}}$|
|$2$|$2 \times \texttt H, \red{1 \times \texttt S}, 4 \times \texttt O$|$2 \times \texttt H, 4 \times \texttt O$|$\red{\texttt{NE}}$|
|$3$|$1 \times \texttt N, \red{5 \times \texttt H}, 1 \times \texttt S, 4 \times \texttt O$|$1 \times \texttt N, \red{4 \times \texttt H}, 1 \times \texttt S, 4 \times \texttt O$|$\red{\texttt{NE}}$|
|$4$|$1 \times \texttt C, 4 \times \texttt H, 4 \times \texttt O$|$1 \times \texttt C, 4 \times \texttt H, 4 \times \texttt O$|$\green{\texttt{DA}}$|

**�����ݹ�ģ��Լ����**

**�������������ԡ�**

- Subtask 1��10 pts��������ʽ�о��������֡�
- Subtask 2��10 pts��������ʽ�о��������֡�
- Subtask 3��30 pts�������������ơ�

���� $100\%$ �����ݣ�$1 \le n \le 1000$��

**����Դ��[COCI 2021-2022#5](https://hsin.hr/coci/contest5_tasks.pdf) Task 1 Kemija��**

