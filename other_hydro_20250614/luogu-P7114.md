## ��Ŀ����
С C ѧϰ�����ַ���ƥ���������ݣ�������������һ��ϰ�⡣

����һ���ַ��� $S$����ĿҪ�����ҵ� $S$ �����о���������ʽ�Ĳ�ַ�������

$S = ABC$��$S = ABABC$��$S = ABAB \ldots ABC$������ $A$��$B$��$C$ ���Ƿǿ��ַ������� $A$ �г��������ε��ַ����������� $C$ �г��������ε��ַ�������

������أ����ǿ��Զ��� $AB$ ��ʾ�����ַ��� $A$��$B$ �����ӣ����� $A = \texttt{aab}$��$B = \texttt{ab}$���� $AB = \texttt{aabab}$��

���ݹ�ض��� $A^1=A$��$A^n = A^{n - 1} A$��$n \ge 2$ ��Ϊ�������������� $A = \texttt{abb}$���� $A^3=\texttt{abbabbabb}$��

��С C ��ϰ������ $S = {(AB)}^iC$ �ķ����������� $F(A) \le F(C)$��$F(S)$ ��ʾ�ַ��� $S$ �г��������ε��ַ������������ַ�����ͬ���ҽ�����ֳ��� $A$��$B$��$C$ ��������һ���ַ�����ͬ��

С C ������������⣬ֻ����������������������

## �����ʽ
�����ж������ݣ������ļ���һ��һ�������� $T$ ��ʾ����������

ÿ�����ݽ�һ��һ���ַ��� $S$���������Ŀ������$S$ ����Ӣ��Сд��ĸ���ɡ�

## �����ʽ
����ÿ���������һ��һ��������ʾ�𰸡�

```input1
3
nnrnnr
zzzaab
mmlmmlo

```

```output1
8
9
16

```

```input2
5
kkkkkkkkkkkkkkkkkkkk
lllllllllllllrrlllrr
cccccccccccccxcxxxcc
ccccccccccccccaababa
ggggggggggggggbaabab

```

```output2
156
138
138
147
194

```

```input3
�������е� string/string3.in
```

```output3
�������е� string/string3.ans
```

```input4
�������е� string/string4.in
```

```output4
�������е� string/string4.ans
```

## ��ʾ
**������ #1 ���͡�**

���ڵ�һ�����ݣ����еķ���Ϊ

1. $A=\texttt{n}$��$B=\texttt{nr}$��$C=\texttt{nnr}$��
2. $A=\texttt{n}$��$B=\texttt{nrn}$��$C=\texttt{nr}$��
3. $A=\texttt{n}$��$B=\texttt{nrnn}$��$C=\texttt{r}$��
4. $A=\texttt{nn}$��$B=\texttt{r}$��$C=\texttt{nnr}$��
5. $A=\texttt{nn}$��$B=\texttt{rn}$��$C=\texttt{nr}$��
6. $A=\texttt{nn}$��$B=\texttt{rnn}$��$C=\texttt{r}$��
7. $A=\texttt{nnr}$��$B=\texttt{n}$��$C=\texttt{nr}$��
8. $A=\texttt{nnr}$��$B=\texttt{nn}$��$C=\texttt{r}$��

**�����ݷ�Χ��**

| ���Ե��� | $\lvert S \rvert \le$ | �������� |
|:-:|:-:|:-:|
| $1 \sim 4$ | $10$ | �� |
| $5 \sim 8$ | $100$ | �� |
| $9 \sim 12$ | $1000$ | �� |
| $13 \sim 14$ | $2^{15}$ | $S$ ��ֻ����һ���ַ� |
| $15 \sim 17$ | $2^{16}$ | $S$ ��ֻ���������ַ� |
| $18 \sim 21$ | $2^{17}$ | �� |
| $22 \sim 25$ | $2^{20}$ | �� |

�������в��Ե㣬��֤ $1 \le T \le 5$��$1 \le |S| \le 2^{20}$�� 

