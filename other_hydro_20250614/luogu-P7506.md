## ��Ŀ����
#### ��Ϸ�ſ�

����¶ŵ��������Ϸ����ڻ�������ơ�������һ�����ɿ��ֵĶ���ҿ��ƻغ�����Ϸ��

**ע�⣺����Ĺ����������ϵĢ��ƹ��򲻾���ͬ**�����ڢ�������̫�಻�����״�����������Ĺ���������� $\text{NEU}$ ��Ϸ��

��Ϸ���� $n$ ����ң�Χ��һȦ��һ������� $m$ �֡�ÿ����ҳ�ʼʱ�� $3$ �����ơ���Ϸ��һ�� $k$ ���Ƶ��ƶѡ��ڱ����У��������Ϊ**��������ƶѳ�������**����ģ������⣬���ݸ�������Ĺ����㲻��Ҫ����ѡ�����Ƶ�˳��

Ϊ�˼�����Ϸ�����������Ϊÿһ����Ϸ����һ�����ͱ����������� $\text{int}$ ���ͼĴ����� $p$ ����Ҵ�����Ʊ������Ƕ� $p$ ���в�����

**ע**����ע�������С��֡������֡������غϡ��Ĺ�ϵ��������ֻ�����һ����Ϸ��ÿ���� $m$ �֣�ÿһ�ֻ������ɻغϣ�ÿһ�غϻ���һ����ҳ��ơ�

ÿһ�ֿ�ʼʱ��$p$ �ᱻ��ʼ��Ϊ $0$ ��Ȼ��ӳ�ʼ��ҿ�ʼ������**˳ʱ��˳��**��$1,2,3,\cdots n-1,n,1,2,\cdots$ ����ʱ��ͬ�������γ��ơ�������ǵ�һ�֣���ô��ʼ��Ҿ��� $1$ ����ҡ���ĳ����ҳ���ĳ���ƺ������ʱ $p> 99$ ����������ҳ�Ϊ�þֵ�**ʧ����**���������ͻ�**���̴��ƶѶ���ȡ��һ����**�����뵽��һ�غϡ�ʧ���߻ᶪʧ��������������ƣ������ƶѶ��������������Ʒ����Լ��������С�ͬʱ��ʧ���߻��Ϊ**��һ�ֳ�ʼ���**����һ����Ϸ���У��ƶ������ֻ����������ʹ�õ��Ʋ���ص��ƶѵ��С�

������ܸ�ħ�İ���Ϸ�����͡�

#### ������

�����ƿ��Է�Ϊ���ࣺ�ӷ��ơ������ơ��˷��ơ������ơ��̶��ơ�

- �ӷ��ƣ�һ���� $7$ �֣� $A_{1},A_{2},A_{5},A_{9},A_{19},A_{49},A_{99}$ �����У� $A_x$ ������Ч���ǣ�ʹ $p$ ���������ϵ����֡��� $p\gets p+x$ ��  
- �����ƣ�һ���� $3$ �֣� $B_{1},B_{9},B_{19}$ ������Ч����ӷ������ƣ�ֻ������ʹ $p$ ��ȥ�����ϵ����֡�  
- �˷��ƣ�һ��ֻ�� $1$ �֣� $C_2$ ����������Ч������ $p$ ���϶�Ӧ�����֣��� $p\gets p\times x$ ��  
- �����ƣ�ͬ��ֻ�� $1$ �֣� $D_2$ ������ $p$ ���Զ�Ӧ�����֣�**����ȡ��**���� $p\gets \lfloor p\div x\rfloor$ ��  
- �̶��ƣ�һ���� $3$ �֣� $E_{0},E_{49},E_{99}$ ���Ὣ $p$ ֱ������Ϊ�����ϵ����֡�

#### ����

�����ǿ���ʹһ����������ûغϣ�������һЩ����Ч����һ���ơ�

- $\tt{PASS}$ �������㣬ת����һ����ҡ�
- $\tt{TURN}$ �������㣬����˳��ת��˳ʱ���Ϊ��ʱ�룬��ʱ���Ϊ˳ʱ�롣����һ����Ϸ��ʼʱ������Ϊ˳ʱ�룩��
- $\tt{DOUBLE}$ �������㣬Ȼ�����һ�����ʩ�� $\verb!"DOUBLE"!$ Ч����Ҳ��Ҫ�������ƣ��ȴ�һ��һ���ٴ�һ��һ����Ҫ����ȫ������������ $99$ ���ܱ�֤��ʧ�ܣ���

$\tt{DOUBLE}$ Ч����һЩ˵��������㱻ʩ���� $\tt{DOUBLE}$ ��Ч�����������һ�ų��˽��ƣ����ֽ��ƶ����ԣ�����ô��ͻ�������� $\tt{DOUBLE}$ Ч����������һ�غϣ�**���ҽ�Ч��ת�Ƶ���һ�����**�� $\tt{DOUBLE}$ Ч�����ܵ��ӡ�

--- 

�������ļ��У������������� $\colorbox{#f0f0f0}\verb!A1 A99 D2 PASS DOUBLE!$ �ȵȡ�

#### ����

��һ���ֽ��ὲ��������������ҵ������߼���

���������ô������ʧ�ܣ���ô��Ҿͻ������һ���Ʋ���Ϊʧ���ߣ���Ȼ����������Ʋ������Ϸ��ֲ���ʵ���ϵ�Ӱ�죩����������������Σ�

1. �����ʱû�б�ʩ�� $\tt{DOUBLE}$ Ч����
   - ÿ����һ����ȿ�����ͨ�ƣ�����ѡ���ڲ���Ϊʧ���ߵ�ǰ����ʹ $p$ ���**�����ܴ�**�����ַ���������ж��ַ�������ʹ�� $p$ ����Ǿͻᰴ��**�˷��ơ��ӷ��ơ������ơ������ơ��̶���**��˳������ѡ����Ȼ��ͬһ����ͨ���еĲ�ͬ������Ʋ���ʹ $p$ ������ͬ��ֵ����
   - ���û����ͨ�ƣ����߳��ƺ���Ϊʧ���ߣ���ô�Ϳ���ʹ�ý��ơ���һ����ο�����ͷ�Ƿ��� $\tt{PASS,TURN,DOUBLE}$ �ơ�����У��ʹ�������ơ�
2. �����ʩ���� $\tt{DOUBLE}$ Ч����
   - ���ȿ���ʹ�ý��ơ����ο���$\tt{PASS,TURN,DOUBLE}$ ������У��ʹ�������ơ�
   - ����ѡ���ڲ���Ϊʧ���ߵ�ǰ����ʹ $p$ ���**������С**�����ַ���������ж��ַ�������ʹ�� $p$ ��С���Ǿͻᰴ��**�����ơ������ơ��ӷ��ơ��˷��ơ��̶���**��˳������ѡ�񣩡���ʱ��һᱻ��� $\tt{DOUBLE}$ ״̬���������ᰴ������ $1$ �����ߡ�

## �����ʽ
��һ������������ $n,m,k$ ��������������ʾ��

������ $n$ �У�ÿ���ĸ��ַ��� $name,card_1,card_2,card_3$ ����ʾ������ҵ������Լ������������ơ�������ƽ��ɴ�СдӢ����ĸ��ɣ��������ո񣬳��Ȳ����� $20$ ��

������һ�У� $k$ ���ַ��������մ������µ�˳�������ƶ�����ơ�

������Բο�����������

## �����ʽ
���µ�һ�ֿ�ʼʱ������Ҫ����� $\colorbox{f0f0f0}\verb!Round XXX:!$ �����У�$\verb!XXX!$ ��ʾ���ǵڶ����֣���

ÿ����ҳ���ʱ�����������ʧ���ߣ�����Ҫ����� $\colorbox{f0f0f0}\verb!XXX used YYY,now p=ZZZ.!$ �����У�$\verb!XXX!$ ��������� $\verb!YYY!$ �ǿ������� $\verb!ZZZ!$ �ǵ�ǰ $p$ ��ֵ����

���򣬵�һ����ҳ�Ϊʧ����ʱ�����ֽ�������Ҫ�����$\colorbox{f0f0f0}\verb!XXX lost the game.!$ �����У�$\verb!XXX!$ �����������

������Բο����������

```input1
2 1 10
JoesSR B9 A99 PASS
Cirno C2 D2 A49
E49 DOUBLE PASS A19 A49 A99 A99 A99 A99 A99  
```

```output1
Round 1:
JoesSR used A99,now p=99.
Cirno used D2,now p=49.
JoesSR used E49,now p=49.
Cirno used C2,now p=98.
JoesSR used B9,now p=89.
Cirno used DOUBLE,now p=89.
JoesSR used PASS,now p=89.
Cirno lost the game.
```

```input2
3 2 25
Cirno A9 A19 B1
Reimu TURN A9 C2
Marisa DOUBLE D2 D2
A9 B9 C2 PASS PASS A9 A1 A99 A99 A99 A99 A99 A99 A99 A99 A99 A99 A99 A99 A99 A99 A99 A99 A99 A99

```

```output2
Round 1:
Cirno used A19,now p=19.
Reimu used C2,now p=38.
Marisa used D2,now p=19.
Cirno used A9,now p=28.
Reimu used A9,now p=37.
Marisa used C2,now p=74.
Cirno used A9,now p=83.
Reimu used B9,now p=74.
Marisa used A9,now p=83.
Cirno used A1,now p=84.
Reimu used PASS,now p=84.
Marisa used D2,now p=42.
Cirno used B1,now p=41.
Reimu used TURN,now p=41.
Cirno used PASS,now p=41.
Marisa used DOUBLE,now p=41.
Reimu lost the game.
Round 2:
Reimu used A99,now p=99.
Marisa lost the game.

```

## ��ʾ
#### ���� 1 ˵��

�Ƶ�ʹ�����������������С������˵��ÿ��һ���ƺ�ÿ����ҵ�ǰ���Ƶ����������ΪʲôҪʹ��ĳ���ƣ����Բο���Ŀ������

$$
\def\c#1{\texttt{#1}}
\def\arraystretch{1.5}
\begin{matrix}
\begin{gathered}
\textbf{\textsf{��ʼ}}\cr
\begin{array}{|c|c|c|c|} \hline
\textbf{�����} & \textbf{���� 1} & \textbf{���� 2}  & \textbf{���� 3} \cr\hline
\text{JoesSR} & \c{B9} & \c{A99} & \c{PASS} \cr\hline
\text{Cirno} & \c{C2} & \c{D2} & \c{A49} \cr\hline
\end{array}\cr
\textbf{\textsf{��һ�غ�}}\quad (p: 0\to 99)\cr
\begin{array}{|c|c|c|c|} \hline
\textbf{�����} & \textbf{���� 1} & \textbf{���� 2}  & \textbf{���� 3} \cr\hline
\text{JoesSR} & \c{B9} & \c{E49} & \c{PASS} \cr\hline
\text{Cirno} & \c{C2} & \c{D2} & \c{A49} \cr\hline
\end{array}\cr
\textbf{\textsf{�ڶ��غ�}}\quad (p:99\to 49)\cr
\begin{array}{|c|c|c|c|} \hline
\textbf{�����} & \textbf{���� 1} & \textbf{���� 2}  & \textbf{���� 3} \cr\hline
\text{JoesSR} & \c{B9} & \c{E49} & \c{PASS} \cr\hline
\text{Cirno} & \c{C2} & \c{DOUBLE} & \c{A49} \cr\hline
\end{array}\cr
\textbf{\textsf{�����غ�}}\quad (p:49\to 49)\cr
\begin{array}{|c|c|c|c|} \hline
\textbf{�����} & \textbf{���� 1} & \textbf{���� 2}  & \textbf{���� 3} \cr\hline
\text{JoesSR} & \c{B9} & \c{PASS} & \c{PASS} \cr\hline
\text{Cirno} & \c{C2} & \c{DOUBLE} & \c{A49} \cr\hline
\end{array}\cr
\end{gathered}
&
\begin{gathered}
\textbf{\textsf{���Ļغ�}}\quad (p:49\to 98)\cr
\begin{array}{|c|c|c|c|} \hline
\textbf{�����} & \textbf{���� 1} & \textbf{���� 2}  & \textbf{���� 3} \cr\hline
\text{JoesSR} & \c{B9} & \c{PASS} & \c{PASS} \cr\hline
\text{Cirno} & \c{A19} & \c{DOUBLE} & \c{A49} \cr\hline
\end{array}\cr
\textbf{\textsf{����غ�}}\quad (p:98\to 89)\cr
\begin{array}{|c|c|c|c|} \hline
\textbf{�����} & \textbf{���� 1} & \textbf{���� 2}  & \textbf{���� 3} \cr\hline
\text{JoesSR} & \c{A49} & \c{PASS} & \c{PASS} \cr\hline
\text{Cirno} & \c{A19} & \c{DOUBLE} & \c{A49} \cr\hline
\end{array}\cr
\textbf{\textsf{�����غ�}}\quad (p:89\to 89)\cr
\begin{array}{|c|c|c|c|} \hline
\textbf{�����} & \textbf{���� 1} & \textbf{���� 2}  & \textbf{���� 3} \cr\hline
\text{JoesSR} & \c{A49} & \c{PASS} & \c{PASS} \cr\hline
\text{Cirno} & \c{A19} & \c{A99} & \c{A49} \cr\hline
\end{array}\cr
\textbf{\textsf{���߻غ�}}\quad (p:89\to 89)\cr
\begin{array}{|c|c|c|c|} \hline
\textbf{�����} & \textbf{���� 1} & \textbf{���� 2}  & \textbf{���� 3} \cr\hline
\text{JoesSR} & \c{A49} & \c{A99} & \c{PASS} \cr\hline
\text{Cirno} & \c{A19} & \c{A99} & \c{A49} \cr\hline
\end{array}\cr
\end{gathered}
\end{matrix}
$$

**ע**����ʼ�غ��Լ��� $2,4,6$ �غ϶��� $\text{JoesSR}$ ���ƣ��� $1,3,5,7$ �غ϶�����¶ŵ���ơ�ֵ��ע����ǣ����ܵ� $5$ �غ���¶ŵʹ���� $\tt{DOUBLE}$ ������Ϊ��һ�غϱ� $\tt{PASS}$ �ˣ����Ե� $7$ �غ���Ȼ����¶ŵ���ơ�

��ʱ��¶ŵ������ζ���ʧ�ܣ�������¶ŵ��Ϊ��ʧ���ߡ�

#### ���� 3

���·�������

#### ���ݹ�ģ��Լ��

- ���� $30\%$ �����ݣ���������ͨ�ƣ����� $n\le 3$ ��
- �������� $15\%$ �����ݣ������� $\tt{TURN}$ �ƺ� $\tt{PASS}$ �ơ�
- �������� $15\%$ �����ݣ������� $\tt{DOUBLE}$ �ơ�
- ���� $100\%$ �����ݣ� ���� $1\le n\le 30;1\le m\le 100;1\le k\le 3\times 10^5$ ����֤�κ�ʱ�� $|p|<10^4$ ��

#### �ο�����

[���������ο��š�NEU�������ơ�����ʮ��ǰ��ͬ��](https://www.bilibili.com/read/cv9951620)

