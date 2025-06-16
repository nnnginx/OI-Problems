## ��Ŀ����
ICPC2020 WF D

## ��Ŀ����
International Cell Processing Company (ICPC) is a world leader in the analysis of genetic
sequences. A genetic sequence is a sequence of nucleotides, which in this problem is
represented by a string containing only the letters $\texttt{A}$, $\texttt{C}$, $\texttt{G}$, and $\texttt{T}$ 
in some combination, each letter representing a single nucleotide 
($\textbf{A}$denine, $\textbf{C}$ytosine, $\textbf{G}$uanine, and $\textbf{T}$hymine, respectively).

One of the key discoveries made by ICPC is that through a process called Genetically Optimized
Organic Folding (GOOF), they can take a genetic sequence and transform it into a simpler one,
while preserving many of the properties of the sequence that ICPC wants to analyze.

A single application of GOOF works as follows. Find a point between two adjacent 
nucleotides in the nucleotide sequence, such that the sequence reads the same from that point in
both directions, up until the nearer end of the sequence. For instance, in the sequence $\texttt{ATTACC}$,
there are two such points: $\texttt{AT-TACC}$ and $\texttt{ATTAC-C}$. Then pick one of these points
(say, the first one), and fold the genetic sequence at that point, merging the identical nucleotides (so, in this
case the $\texttt{AT}$ and $\texttt{TA}$ would become merged, and the resulting sequence would be $\texttt{CCAT}$
or $\texttt{TACC}$).

Through repeated application of GOOF, a nucleotide can potentially be made much shorter.
However, manually searching for the appropriate folding points is very time-consuming.  ICPC
reached out to you to write a program that would automate the process of finding the folding
points and choosing them so as to obtain the shortest possible genetic sequence from a given
input sequence.


## �����ʽ
The input contains a single string $s$ representing the nucleotide sequence to be analyzed. 
The string consists of characters $\texttt{A}$, $\texttt{C}$, $\texttt{G}$, and $\texttt{T}$ only. 
The length of $s$ is between $1$ and $4 \cdot 10^6$, inclusive.

## �����ʽ
Output the smallest possible length of a sequence obtained from
the input by applying GOOF zero or more times.

## ��Ŀ����
### ��Ŀ����
����ϸ���ӹ���˾(ICPC)�ڻ������з������洦���������ȵ�λ���Ŵ������Ǻ���������У�����������У�����һ��ֻ������ĸ$\texttt{A}$��$\texttt{C}$��$\texttt{G}$��$\texttt{T}$��ĳ����ϵ��ַ�������ʾ��ÿ����ĸ�ֱ����һ�������������ʣ�$\textbf{A}$denine��������ण�$\textbf{C}$ytosine���������ʣ�$\textbf{G}$uanine����������ण�$\textbf{T}$hymine����

ICPC��һ����Ҫ�����ǣ�ͨ��һ�ֱ���Ϊ�����Ż��л��۵�(GOOF)�Ĺ��̣����ǿ��Խ�һ����������ת��Ϊһ�����򵥵����У�ͬʱ����ICPC��Ҫ���������е�������ԡ�

������GOOF��һ��Ӧ�á��ں������������������ں�����֮���ҵ�һ���㣬ʹ�Ӹõ㿪ʼ�����������������϶�����ͬ�ģ�ֱ�����е����һ���㡣���磬������$\texttt{ATTACC}$�У������������ĵ�:$\texttt{AT-TACC}$��$\texttt{ATTAC-C}$��Ȼ��ѡ������һ����(�����һ����)�����Ǹ����۵��������У��ϲ���ͬ�ĺ�����(��ˣ�����������£�$\texttt{AT}$��$\texttt{TA}$��ϲ����õ������н���$\texttt{CCAT}$��$\texttt{TACC}$)��

ͨ���ظ�ʹ��GOOF������ʹ�������ø��̡����ǣ��ֹ�Ѱ�Һ��ʵ��۵���ǳ���ʱ��ICPC�ҵ��㣬����дһ���������Զ��ҵ��۵��㲢ѡ�����ǣ��Ӷ��Ӹ��������������л�þ����̵ܶĻ������С�

### �����ʽ
�������һ����ʾҪ�����ĺ��������е��ַ�����ֻ����$\texttt{A}$��$\texttt{C}$��$\texttt{G}$��$\texttt{T}$�� _s_ ������$1$ ~ $4\cdot10^6$֮�䡣

### �����ʽ
�����������Ӧ����λ���GOOF�õ������е���С���ܳ��ȡ�

```input1
ATTACC
```

```output1
3
```

```input2
AAAAGAATTAA
```

```output2
5
```

