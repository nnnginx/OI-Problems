## ��Ŀ����
С A ��һ���ַ��� $t$�������Խ������²������е� $t$ ��һ��ǰ/��׺�������е���ǰ/��׺Ϊ**�и��** $t$ ���Ӵ���С A ��õ��ַ��� $s$��������������Ҫ���ж��ٴβ������޽���� $-1$��

## �����ʽ
�����ַ����ֱ��ʾ $t,s$��

## �����ʽ
һ��һ����������ʾ�𰸡�

```input1
abbabb
ba
```

```output1
3
```

```input2
fxofoxxooffoxooo
fox
```

```output2
8
```

```input3
abcdefghijklmnopq
rstuvwxyzz
```

```output3
-1
```

```input4
ycxcy
cxy
```

```output4
-1
```

## ��ʾ
������˵����

���� $1$��$\texttt{abbabb}\to \texttt{abba}\to \texttt{bba}\to \texttt{ba}$��������Ψһ��

���� $2$��$\texttt{fxofoxxooffoxooo}\to\texttt{xofoxxooffoxooo}\to\texttt{foxxooffoxooo}\to\texttt{xooffoxooo}\to\texttt{ffoxooo}\to\texttt{ffoxoo}\to\texttt{ffoxo}\to\texttt{ffox}\to\texttt{fox}$��������Ψһ��

�����ݷ�Χ��Լ����

**�������������ԡ�**

- Subtask 1��1 points����$s=t$��
- Subtask 2��9 points����$s$ ��������ĸ $\texttt{a}$��
- Subtask 3��15 points����$|t|\leq 100$��
- Subtask 4��17 points����$|t|\leq 500$��
- Subtask 5��18 points����$|t|\leq 1.5\times 10^3$��
- Subtask 6��15 points����$|s|=4$��*���������
- Subtask 7��25 points�������������ơ�

���� $100\%$ �����ݣ�$1 \leq |s| \leq |t| \leq 5\times 10^3$���ַ��� $\in[\texttt{a,z}]$��

*���������$s,t$ �ַ���������ַ��� $\in[\texttt{a,c}]$��

**��ע�ⳣ���Ż���**

---

����Ŀ��Դ��

[Sweet Round 05](https://www.luogu.com.cn/contest/28195) E��    
idea & solution��[Isaunoya](https://www.luogu.com.cn/user/96580) & [Alex_Wei](https://www.luogu.com.cn/user/123294)��

