## ��Ŀ����
Ϊ��������̣�ZJY ��ʼѧϰ�����ۡ���һ�죬���뵽������һ�����⣺����һ��������ɵ� $n$ �������и������������л��಻ͬ������̬�ȸ��ʳ��֣�������Ҷ�ӽڵ����������Ƕ����أ�

�ж��������Ƿ�ͬ����α�������£�

$$
\def\arraystretch{1.2}
    \begin{array}{ll}
    \hline
    \textbf{�㷨 1}&\text{Check}(T1,T2) \\
    \hline
    1&\textbf{Require: }\text{ �������Ľڵ�}T1,T2\\
    2&\qquad\textbf{if}\ \ T1=\text{null}\textbf{ or }T2=\text{null}\textbf{ then }\\
    3&\qquad\qquad\textbf{return}\ \ T1=\text{null}\textbf{ and }T2=\text{null}\\
    4&\qquad\textbf{else}\\
    5&\qquad\qquad\textbf{return}\ \text{Check}(T1\to\mathit{leftson},T2\to\mathit{leftson}) \\ 
    & \qquad\qquad\qquad \textbf{ and }\text{Check}(T1\to\mathit{rightson},T2\to\mathit{rightson})\\
    6&\qquad\textbf{endif}\\
    \hline
    \end{array} 
    $$



## �����ʽ
����һ�������� $n$����ʾ�и����Ľ������


## �����ʽ
��������������Ҷ�ӽڵ�����Ҫ�����С�� $10^{-9}$��


```input1
1
```

```output1
1.000000000
```

```input2
3
```

```output2
1.200000000
```

## ��ʾ
## ���ݷ�Χ

���� $30\%$ �����ݣ�$1 \le n \le 10$��

���� $70\%$ �����ݣ�$1 \le n \le 100$��

���� $100\%$ �����ݣ�$1 \le n \le 10^9$��

