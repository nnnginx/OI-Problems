## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/29ph2q84.png)

## ��Ŀ����
����һ������Ϊ $n$ ������ $\{a\}$���Լ� $q$ ��ѯ�ʡ�

ѯ������ `l r L R p x`����ʾѯ���ж��� $i \in [l,r]$ �� $ a_i \in [L,R]$��$a_i$ �� $p$ ȡ��Ľ���� $x$�� 

ǿ�����ߡ�

## �����ʽ
��һ���������� $ n,\text{type}$��

�ڶ��а��� $n$ ���������� $i$ ��������ʾ $a_i$��

������һ������ $q$��

������ $q$ �У�ÿ�а��������������ֱ��ʾ $l,r,L,R,p,x$����� $\text{type}=0$������������ּ�Ϊ��ʵ��ѯ�ʣ�����ÿһ������Ҫ��λ�������һ��ѯ�ʵĴ� $\text{last}$����ǰ��û��ѯ�ʣ��� $\text{last}=0$��

## �����ʽ
����ÿ��ѯ�ʣ����һ�б�ʾ�𰸡�

```input1
6 0
1 1 4 5 1 4
3
1 6 1 6 2 0
2 3 1 6 3 1
2 5 2 5 4 1
```

```output1
2
2
1
```

```input2
�������е� rvmq_sample2.in��
```

```output2
�������е� rvmq_sample2.out��
```

## ��ʾ
$$
\def\arraystretch{1.2}
\begin{array}{|c|c|c|c|}
\hline
\begin{array}{c}
\tt{subtask}\\\hline
1\\\hline
2\\\hline
3\\\hline
4\\\hline
\end{array}
&
\begin{array}{c}
n,q\\\hline
\le 5\times10^3\\\hline
\le 10^5\\\hline
\le 10^5\\\hline
\le 10^5 
\end{array}
&
\begin{array}{c}
\tt{\tt{��������}}\\\hline
\tt{��}\\\hline
\tt{��֤������Ԫ�� \le 2\times10^4}\\\hline
\tt{��֤ \text{type}= 0 }\\\hline
\tt{��}\\\hline
\end{array}
&
\begin{array}{c}
\tt{pts}\\\hline
10\\\hline
30\\\hline
20\\\hline
40\\\hline
\end{array}
\\\hline
\end{array}
$$



�����������ݣ�$1 \le n \le 10^5$��$1 \le q \le 10^5$��$1 \le a_i \le 2\times10^5$��$1 \le l \le r \le n$��$1 \le L \le R \le n$��$0 \le x < p \le n$��$\text{type} \in \{0,1 \}$��

���������Ϊ�Ǹ�������


