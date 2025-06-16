## ��Ŀ����
������ <http://czoj.com.cn/p/955>������Ϊ������ݡ�

## ��Ŀ����
С Y ��һ�� $n\times n$ ���̣���ʼʱ�������ÿ�����ӵ���ɫ�ǰ׺����ģ�����һ�еĵ� $1,3,5\cdots$ �������ǰ�ɫ���� $2,4,6\cdots$ �������Ǻ�ɫ���ڶ��е� $2,4,6\cdots$ �������ǰ�ɫ���� $1,3,5\cdots$ �������Ǻ�ɫ������ͼ��ʾ��


$$
\def\b{\color{ff}\rule{10px}{10px}\kern{1px}}
\def\w{\color{white}\rule{10px}{10px}\kern{1px}}
\def\bg{\color{black}\rule{33.5px}{33.5px}}
\def\eps{\\[-39.5px]}
\def\ep{\\[-5.5px]}
\begin{aligned}
\bg\eps
\w\b\w\ep
\b\w\b\ep
\w\b\w
\end{aligned}
$$

С Y ����� $q$ �β�����ÿ�β����Ὣĳһ�л���ĳһ�е����и��ӵ���ɫ��ת������ɫ���ӱ�ɺ�ɫ���ӣ���ɫ���ӱ�ɰ�ɫ���ӡ�

С Y ��֪������ÿ�β���֮��һ���ж��ٸ�ͬ��ɫ��ȫ�ڻ�ȫ�ף�����ͨ����������ָͨ����**����ͨ**������������֮���б����ڲ�����ͨ��



## �����ʽ
�� $1$ �� $2$ �������� $n,q$����ʾ���̵Ĵ�С�Ͳ����Ĵ�����

�� $2$ �� $q+1$ ��ÿ�� $2$ �������� $\text{opt}_i,a_i$���� $\text{opt}_i=1$ ���ʾ��ת�����У�$\text{opt}_i=2$ ���ʾ��ת�����У�$a_i$ ��ʾ��ת���ǵڼ��У��У���

## �����ʽ
��� $q$ ��ÿ��һ����������ʾ�ھ����ôβ�����һ���ж��ٸ�ͬ��ɫ����ͨ����



```input1
3 3
1 2
2 3
1 2
```

```output1
3
2
6
```

```input2
100000 1
1 1
```

```output2
9999900000
```

```input3
15000 5
1 90
1 1231
1 91
1 1233
1 1232
```

```output3
224970000
224940000
224940000
224910000
224940000
```

## ��ʾ
### ���� $\textbf 1$ ����
$$
\def\b{\color{ff}\rule{10px}{10px}\kern{1px}}
\def\w{\color{white}\rule{10px}{10px}\kern{1px}}
\def\bg{\color{black}\rule{33.5px}{33.5px}}
\def\eps{\\[-39.5px]}
\def\ep{\\[-5.5px]}
\begin{aligned}
\bg\eps
\w\b\w\ep
\b\w\b\ep
\w\b\w
\end{aligned}
\to
\begin{aligned}
\bg\eps
\w\b\w\ep
\w\b\w\ep
\w\b\w
\end{aligned}
\to
\begin{aligned}
\bg\eps
\w\b\b\ep
\w\b\b\ep
\w\b\b
\end{aligned}
\to
\begin{aligned}
\bg\eps
\w\b\b\ep
\b\w\w\ep
\w\b\b
\end{aligned}
$$

### ���ݷ�Χ
�����������ݣ�$1��q, n��10^5, 1��\text{opt}_i��2, 1��a_i��n$��

|���Ե���|$n$|$q$|��������|
|:-:|:-:|:-:|:-:|
|$1\sim4$|$\le 4$|$\le 10$|��|
|$5\sim6$|$\le10^5$|$=1$|��|
|$7\sim9$|$\le10^5$|$\le10^5$|$\alpha$|
|$10$|$\le10^5$|$\le10^5$|��|

- �������� $\alpha$����֤ͬһ�����Ե����е� $\text{opt}_i$ ����ȡ�

