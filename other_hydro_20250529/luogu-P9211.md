## ��Ŀ����
����������������������ν�Ĳ��������������һ��������޾���ʱ�����޾���ѭ��������

��Ȼ��û��Ǳ��ò��ϲ����������ɡ�

## ��Ŀ����
������ġ�һ�������Ա�����һ�����Ȳ����� $l_{\max}$ ���ַ��� $S_0$�����޾����ֻغ��γ���һ�����޳����ַ��� $S_{\mathrm{inf}}=S_0+S_0+S_0+\cdots$�����ڽ�ȡ $S_{\mathrm{inf}}$ ǰ $l$ ���ַ�����Ϊ�ɹ۲�ʱ���ﲻ��������� $S_{\mathrm{fin}}$��

Ȼ����ν���ֻز����ǻ�е�����ѭ����������ˣ�$S_\mathrm{fin}$ ���л���**������ $n$ ���ַ�**���޸ĳ��˱���ַ�������� $S_{\mathrm{real}}$��

���ڹ۲⵽�� $S_{\mathrm{real}}$������ϣ���ҵ����ֻص����� $S_0$��Ȼ�����ڲ�������ֻ�̫������������ֻϣ���ҵ�����һ�� $S_0'$��ʹ���������ɵ� $S_\mathrm{fin}'$ �޸�**������ $m$ ���ַ�**��Ϳ��Ա�� $S_{\mathrm{real}}$��


## �����ʽ
��һ�����ĸ������� $l,l_{\max},n,m$��

�ڶ��������۲⵽�ĳ���Ϊ $l$ ���ַ��� $S_{\mathrm{real}}$��

## �����ʽ
��һ�����һ�������� $l_0$����ʾ�����ҵ��� $S_0$ �ĳ��ȡ���Ӧ����֤ $1\le l_0\le l_{\max}$��

�ڶ������һ������Ϊ $l_0$ ���ַ��� $S_0$����ʾ�����ҵ����ַ�����

```input1
25 8 5 10
aaacdaabbbaabccaabcdaabcd

```

```output1
5
aaacd
```

## ��ʾ
### ��������

��������������⣬**���������ݷ�Χ��Լ��**������Լ����μ������ݷ�Χ��Լ������

���� $S_{\mathrm{real}}$ ���õ� $S_0=\verb!aabcd!$��

- �ɴ����� $S_{\mathrm{inf}}=\verb!aabcdaabcdaabcdaabcdaabcd!\cdots$��
- �ɴ����� $S_{\mathrm{fin}}=\verb!aabcdaabcdaabcdaabcdaabcd!$��
- �ɴ����� $S_{\mathrm{real}\kern{-2.5pt}}=\verb!aaacdaabbbaabccaabcdaabcd!$��

�������������һ�����ܵ� $S_0'=\verb!aaacd!$���ɴ˼���� $S_{\mathrm{fin}}'$ �� $S_{\mathrm{real}}$ �Ĳ�ࣺ

$$\begin{aligned}
S_{\mathrm{fin}}'=&\texttt{aaacdaa\textcolor{red}a\textcolor{red}c\textcolor{red}daa\textcolor{red}ac\textcolor{red}daa\textcolor{red}acdaa\textcolor{red}acd}\cr
S_{\mathrm{real}}=&\texttt{aaacdaabbbaabccaabcdaabcd}\cr
\end{aligned}$$

���Ϊ $7$�������� $m=10$�����Ա����ܡ�

### ���ݷ�Χ��Լ��

����ȫ�����ݣ���֤ $l=3\times 10^5$��$n=3\times 10^3$��$m=10^4$��$1\le l_{\max} \le 10^5$��

