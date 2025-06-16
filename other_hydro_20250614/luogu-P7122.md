## ��Ŀ����
Chino ��ѧϰ��һ�ֽ����߶��������ݽṹ����������д�߶���ʱ������һ�����⣺����֪����ʹ�ö��Ŀռ䣬ֻ֪���߶�����Ҷ�ӽ����� $n$ Ϊһ���ڷ�Χ $[a,b]$ ֮�ڵ���������

Chino �� $f(n)$ ��ʾһ�� $n$ ��Ҷ�ӽ����߶�����ռ����������±ꡣ�����������֪����

$$\sum_{n=a}^{b}f(n)$$

��ô�����ܹ��������Ҫ����ʹ�ö��Ŀռ䡣����������̴����������������

����أ�Chino �����߶�����α�������£�

$$
\def\b#1{\textbf{#1}}\def\t#1{\text{#1}}\def\s\qquad\def\P{\mathbb P}\def\l{\underline{\kern{300pt}}}\def\m#1{#1&\,}
\def\if#1{\b{if }#1\b{ then}}\def\endfunc{\b{end function}.}\def\endif{\b{end if}.}\def\func{\b{function}}\def\return{\b{return}}
\begin{aligned}&\l\\&\b{Function: }\t{Build a Segment Tree.}\\[-10pt]&\l\\[-5pt]&\begin{array}{r|l}\\[-9pt]
\m1\func\ \t{BuildSegmentTree}\left(x,l,r\right):\\
\m2\s\if{\left(l\ne r\right)}:\\
\m3\s\s m\gets\left\lfloor\left(l+r\right)/2\right\rfloor.\\
\m4\s\s\t{BuildSegmentTree}\left(2x,l,m\right).\\
\m5\s\s\t{BuildSegmentTree}\left(2x+1,m+1,r\right).\\
\m6\s\endif\\
\m7\endfunc\\[-10pt]\\\end{array}\\[-13pt]&\l\end{aligned}
$$

�߶�����ռ����������±꼴Ϊ�� $\def\t#1{\text{#1}}\t{BuildSegmentTree}\left(1,1,n\right)$ �����е��õ� $\def\t#1{\text{#1}}\t{BuildSegmentTree}$ �в��� $x$ �����ֵ��

## �����ʽ
���빲���С�

��һ��Ϊһ�������� $a$���ڶ���Ϊһ�������� $b$��������������������

## �����ʽ
���һ��һ������������ʾ��Ĵ𰸡�

```input1
1
10

```

```output1
108

```

```input2
233333
666666

```

```output2
588544964910

```

```input3
1
1000000000000000000

```

```output3
1419691012023749904603586777179575510

```

## ��ʾ
### �������� #1
$1\sim 10$ ��Ҷ�ӽ����߶���������±�ֱ�Ϊ $1,3,5,7,9,13,13,15,17,25$����͵õ� $108$��

### ���Ե�Լ��
**�������������ԡ�**

����ȫ�����ݣ��� $1\le a\le b\le10^{10^6}$��

ÿ��������ľ������Ƽ��±�

| �������� | ��ֵ | $b\le$ | $a=b$ |
|:-:|:-:|:-:|:-:|
| 1 | 10 | $10^{10^0}$ | $\times$ |
| 2 | 10 | $10^{10^1}$ | $\times$ |
| 3 | 10 | $10^{10^2}$ | $\times$ |
| 4 | 10 | $10^{10^3}$ | $\surd$ |
| 5 | 10 | $10^{10^3}$ | $\times$ |
| 6 | 10 | $10^{10^4}$ | $\surd$ |
| 7 | 10 | $10^{10^4}$ | $\times$ |
| 8 | 10 | $10^{10^5}$ | $\surd$ |
| 9 | 10 | $10^{10^5}$ | $\times$ |
| 10 | 10 | $10^{10^6}$ | $\times$ |

