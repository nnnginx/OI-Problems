## ��Ŀ����
Bob ϲ���߶�����


## ��Ŀ����
����㲻֪���߶��������Կ� ��ʾ˵�� �еĶ��塣

Bob �õ���һ������Ϊ $n$ ������ $a_{1,2,\cdots,n}$����ʼȫΪ $0$��

���� Bob ������ $m$ ������Ӳ�����ÿ�β�����ȸ��ʵش� $[1,n]$ ������ $\dfrac{n(n+1)}{2}$ �������������ѡ��һ�����в�����ÿ�μӵ����� $[-1,V]$ ֮��ȸ��������������

$m$ �β�����֮��Ҫ���ÿһ��λ�õ�ֵ��

���� Bob ϲ���߶������������ش��һ�� $[1,n]$ �ϵ��߶��������������⣬ʹ�����������������ӵ����⡣

�����Ĺ����� Bob ��Ȼ�뵽��������С $\mathrm{Pushdown}$���´������ǣ������ķ�����

+ �޸ĵ�ʱ�� $\mathrm{Pushdown}$�����һ���� $\mathrm{Pushdown}$���� $\mathrm{Pushall}$ ��������

+ $\mathrm{Pushall}$ ��һ���ڵ��ʱ���������ڵ��������Ϊ $0$ ��ô�� $\mathrm{Pushdown}$��

���� Bob ��֪������ $\mathrm{Pushdown}$ �����������������㣬���������㡣

������ Bob д���߶���α���루���� `tag` ����Ϊ�����ǣ���

$
\displaystyle
\begin{array}{l}
\mathrm{pushdown\_counter}\leftarrow 0\\
\\
\textbf{function }\mathrm{Update(Node},l,r,ql,qr,Delta)\\
\qquad \textbf{if } [l,r]\cap [ql,qr] = \varnothing \textbf{ then}\\
\qquad \qquad \textbf{return}\\
\qquad \textbf{end if}\\
\qquad \textbf{if }[l,r] \subseteq [ql,qr] \textbf{ then}\\
\qquad \qquad \mathrm{tag[Node]\leftarrow tag[Node]}+Delta\\
\qquad \qquad \textbf{return}\\
\qquad \textbf{end if}\\
\qquad mid\leftarrow \lfloor\dfrac{l+r}{2}\rfloor\\
\qquad \mathrm{Update(LeftChild},l,mid,ql,qr,Delta)\\
\qquad \mathrm{Update(RightChild},mid+1,r,ql,qr,Delta)\\
\textbf{end function}\\
\\
\textbf{function }\mathrm{Pushdown(Node)} \\
\qquad \mathrm{tag[LeftChild]\leftarrow tag[LeftChild]+tag[Node]}\\
\qquad \mathrm{tag[RightChild]\leftarrow tag[RightChild]+tag[Node]}\\
\qquad \mathrm{pushdown\_counter}\leftarrow \mathrm{pushdown\_counter}+1\\
\textbf{end function}\\
\\
\textbf{function }\mathrm{Pushall(Node},l,r)\\
\qquad \textbf{if } \mathrm{Node\ is\ Leaf} \textbf{ then}\\
\qquad \qquad \textbf{return}\\
\qquad \textbf{end if}\\
\qquad \textbf{if } \mathrm{tag[Node] \not= 0} \textbf{ then}\\
\qquad \qquad \mathrm{Pushdown(Node)}\\
\qquad \textbf{end if}\\
\qquad mid\leftarrow \lfloor\dfrac{l+r}{2}\rfloor\\
\qquad \mathrm{Pushall(LeftChild},l,mid)\\
\qquad \mathrm{Pushall(RightChild},mid+1,r)\\
\textbf{end function}
\end{array}
$


���仰˵����Ҫ�� Bob ��� `pushdown_counter` ������ֵ��

�𰸶� $998244353$ ȡģ��


## �����ʽ
һ���������� $n,m,V$��

## �����ʽ
һ������������ $\mathrm{Pushdown}$ ������ $998244353$ ȡģ�Ľ����

```input1
2 1 0

```

```output1
166374059

```

```input2
2 2 1

```

```output2
813384288

```

```input3
3 2 1

```

```output3
462150164

```

```input4
100 114 514

```

```output4
718571152

```

## ��ʾ
**���������� #1��**

�����߶���ֻ�� $3$ ���ڵ㣺$[1,2],[1,1],[2,2]$��

ֻ�нڵ� $[1,2]$ ���� $\mathrm{Pushdown}$��

������Ϊ $\mathrm{Update(1,2,-1)}$ ��ʱ�򣬸��ڵ��������Ϊ $-1$�� $\mathrm{Pushall}$ �ڸ��Žڵ�� $\mathrm{Pushdown}$���� $\mathrm{Update(1,2,0)}$ ֮�����ڸ��ڵ�������Ϊ $0$ �� $\mathrm{Pushdown}$��

���� $4$ �ֲ������������Ǵ���Ҷ�ӽڵ㣬�� $\mathrm{Update(1,1,-1)},\mathrm{Update(1,1,0)},\mathrm{Update(2,2,-1)},\mathrm{Update(2,2,0)}$������ $\mathrm{Pushdown}$��

���ԣ��ܹ� $6$ ��������� $\mathrm{Pushdown}$ ��ֻ�� $1$ �֣���������Ϊ $\dfrac{1}{6}$��

**���������� #2��**

����������࣬��һһ���ͣ�ֻ����һ�������

���ִ�е� $2$ �β����ֱ�Ϊ $\mathrm{Update(1,2,-1)},\mathrm{Update(1,2,1)}$��������ʱ����ڵ��������Ϊ $0$���� $\mathrm{Pushall}$ ��ʱ����Ȼ���� $\mathrm{Pushdown}$��

---------

**�����ݷ�Χ��**

**�������������ԡ�**

| �������� | $n\le$       | $m\le$       | $V$               | ��ֵ | ʱ������$\text{ / ms}$ |
| :----: | :------------: | :------------: | :-----------------: | :----: | :--------: |
| $1$        | $4$  | $4$   | $\le 2$         | $3$  | $500$    |
| $2$        | $300$ | $300$ | $\le 300$       | $7$  | $500$    |
| $3$        | $1000$ | $1000$ | $\le 1000$      | $10$ | $500$    |
| $4$       | $300$  | $10^5$ | $=1000$          | $15$ | $2000$   |
| $5$        | $10^5$ | $10^5$ | $\le 0$         | $10$ | $3000$   |
| $6$        | $10^5$ | $10^5$ | $=1000$          | $15$ | $3000$   |
| $7$        | $10^5$ | $10^5$ | $\le 998244350$ | $40$ | $3000$   |


���� $100\%$ �����ݣ�$1 \le n \le 10^5$��$1 \le m \le 10^5$��$-1 \le V \le 998244350$��

----------

**���߶������塿**

�߶�����һ��ÿ���ڵ��϶���¼��һ���߶εĶ����������ڵ��¼���߶��� $[1, n]$������ÿ���ڵ㣬������¼���߶��� $[l, r]$ �� $l\not= r$��ȡ $m = \lfloor \dfrac{l+r}{2} \rfloor$�����������Ҷ��ӽڵ��¼���߶ηֱ��� $[l, m]$ �� $[m+1,r]$���� $l=r$��������Ҷ�ӽڵ㡣


