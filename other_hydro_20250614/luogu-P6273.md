## ��Ŀ����
����һ������Ϊ $n$ ���ַ��� $S$���� $S$ �в�ͬ���ַ���Ϊ $k$ ��

�����ַ������Ӵ�Ϊ���ַ���ĳһ�����Ρ�

�� ***��ħ�����Ӵ�*** ������Ϊ $S$ **��ĳһ�ǿ��Ӵ���������Ӵ��в�ͬ���ַ���Ϊ** $k$ **����ÿ���ַ��ĳ��ֵĴ�������ͬ**��

����Ҫ��������ַ��� $S$ �Ĳ�ͬ�� ��ħ�����Ӵ� �ĸ�����

�������Ӵ������Ҷ˵㲻ͬ�����������Ӵ���ͬ��

## �����ʽ
��һ�У�һ������ $n$ ��ʾ�ַ������ȡ�

�ڶ��У�һ���ַ��� $S$ ��

## �����ʽ
һ��������ʾ�� $\bmod (10^9+7)$ ��ֵ��

```input1
8
abccbabc
```

```output1
4
```

```input2
7
abcABCC
```

```output2
1
```

```input3
20
SwSSSwwwwSwSwwSwwwwS
```

```output3
22
```

## ��ʾ
#### ����������������͡�

**���� 1 ����**

- �����������Ӵ��У� $\texttt{abc},\texttt{cba},\texttt{abc},\texttt{abccba}$

**���� 2 ����**

- ���Ӵ� $\texttt{abcABC}$ Ϊ ��ħ�����Ӵ������ִ�Сд���� $\texttt{a}\ne \texttt{A}$����

**���� 3 ����**

- ����һ���� $\texttt{SwSwwS}$��

#### �����ݹ�ģ��Լ����

**������ö���Ե�������ԣ����� 4 ��������**��

- Subtask 1��10 points����$2\le n\le 100$��
- Subtask 2��20 points����$2\le n\le 2\times 10^3$��
- Subtask 3��30 points����$2\le n\le 10^5,k=2$ ���� $S$ ��ֻ�������ַ�����
- Subtask 4��40 points�������������ơ�

�����������ݣ���֤ $2\le n\le 10^5$���ַ���Ϊ $ [\texttt{a},\texttt{z}] \cup [\texttt{A},\texttt{Z}]$

#### ��˵����

ԭ�����ԣ�[eJOI 2017](www.ejoi.org) Problem A [Magic](http://ejoi.org/wp-content/themes/ejoi/assets/pdfs/tasks_day_1/EN/magic_statement-en.pdf)

�����ṩ��@[```_Wallace_```](https://www.luogu.com.cn/user/61430)

