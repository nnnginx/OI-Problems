## ��Ŀ����
On the stage, $2N$ beavers are standing in a row. They are members of the chorus. Each beaver sings either the alto part or the bass part of the chorus. This information is given by a string $S$. Precisely, the $i$-th beaver ($1\le i\le 2N$) from the stage right (i.e., from left when seen from the audience seats) sings the alto part if the $i$-th character of $S$ is $\text{`\texttt{A}'}$. The $i$-th beaver sings the bass part if the $i$-th character of S is $\text{`\texttt{B}'}$. There are $N$ beavers singing the alto part, and $N$ beavers singing the bass part.

From now, the beavers will sing $K$ songs. However, since all the songs are very difficult, each beaver sings exactly one song only, and does not sing other songs. Moreover, in order to make singing voice more beautiful, for every song, the following conditions should be satisfied.

- At least one beaver sings the song.
- The number of beavers singing the alto part of the song is equal to the number of beavers singing the bass part of the song.
- If we consider the beavers singing the song only, every alto beaver stands the stage right of every bass beaver.

Bitaro, the conductor, tried to find a way to allot songs to beavers which satisfies the conditions. Since Bitaro is bright, he notices that it might be impossible to allot songs to beavers.

In order to cope with this issue, Bitaro will perform the following operation several times so that there is a way to allot songs to beavers which satisfies the conditions.

- Swap the position of two adjacent beavers.

Since Bitaro thinks efficiency is important, he wants to minimize the number of operations. However, it turns out to be a surprisingly difficult problem. Since you are a brilliant programmer, Bitaro asks you to solve this problem.

Write a program which, given information of the chorus and the number of songs $K$, calculates the minimum
number of operations Bitaro needs to perform. Note that, under the constraints of this task, it is possible to perform the operations several times so that there is a way to allot songs to beavers which satisfies the conditions.

## �����ʽ
Read the following data from the standard input.

> $N\ K$
> 
> $S$

## �����ʽ
Write one line to the standard output. The output should contain the minimum number of operations Bitaro needs to perform.

## ��Ŀ����
#### ��Ŀ����
����̨�ϣ��� $2N$ ֻ�����ų�һ�С������Ǻϳ��ŵĳ�Ա��ÿֻ���곪�Ÿ����������������Щ��Ϣ��һ���ַ��� $S$ ����������أ���� $S$ �ĵ� $i$ ���ַ��� $A$�����Ϊ $i$ �ĺ��꣨���ұ߿�̨����������������� $S$ �ĵ� $i$ ���ַ��� $B$�����Ϊ $i$ �ĺ��곪�������� $N$ ֻ���곪�������� $N$ ֻ���곪������

����������Щ���꽫Ҫ�ݳ� $K$ �׸衣Ȼ������Ϊ���и����ǳ����ӣ�ÿֻ����ֻ��һ�׸��������ᳪ�������������⣬Ϊ��ʹ�����������ÿ�׸���������������������

+ ������һֻ���곪���׸衣

+ �����׸�ĳ������ͳ������ĺ�������Ӧ����ȡ�

+ ���ֻ���ǳ����׸�ĺ��꣬���г������ĺ��궼�ڳ������ĺ�����ұߡ�

ָ�Ӽ� Bitaro ���ҵ�һ�ַ�����������Щ���곪���׸裬���������������������� Bitaro �ر��������ע�⵽������޷�ʵ�֡�Ϊ��Ӧ��������⣬Bitaro ������������ֻ�����λ�ö�Σ��Ա���һ�ַ�ʽ���Ե��亣�꣬�Ӷ���������������

���� Bitaro ��ΪЧ�ʺ���Ҫ������������С��Ҫִ�еĲ�������Ȼ��������һ���ǳ����ѵ����⡣��������һλ��ɫ�ĳ���Ա��Bitaro ��������������⡣

��дһ�ݳ����ڸ����ϳ����ݳ��������� $K$ ����Ϣʱ������ Bitaro ��Ҫִ�е���С����������ע�⣬�ڱ�����������£�����ִ�в�����Σ��Ա���һ�ַ�ʽ�����ں���֮������������������������
#### �����ʽ

�ӱ�׼�����ȡ��������:

> $N\ K$
> 
> $S$

#### �����ʽ

���׼���д��һ�С����Ӧ�ð��� Bitaro ��Ҫִ�е���С��������

#### ��������

���������� 1 �У����� Bitaro ����ִ�����²����������»��߱�ʾ�� Bitaro ��������ֻ�����λ�ã�

+ ��������ֻ����ʹ��Ҳ���̨��ʼ�ĵ���ֻ���ꡣ�˲���֮���ַ�����ʾ���Ҳൽ���ĺ��겿�ֱ�Ϊ $\text{`\texttt{AA\underline{AB}BABBAB}'}$��

+ �����ڰ�ֻ����ʹ��Ҳ���̨��ʼ�ĵھ�ֻ���ꡣ�˲���֮���ַ�����ʾ���Ҳൽ���ĺ��겿�ֱ�Ϊ $\text{`\texttt{AAABBAB\underline{AB}B}'}$��

������Щ����֮��Bitaro �������·��亣�곪���׸裺

+ �������������� $1,2,3,4,5,7$ ֻ���곪��һ�׸衣

+ �������������� $6,8,9,10$ ֻ���곪�ڶ��׸衣

���ַ�ʽʹ�����������õ����㡣

��������������� $2$���򲻴���һ�����������ĺ�����䷽ʽ�������� $2$��

```input1
5 2
AABABABBAB
```

```output1
2

```

```input2
5 3
AABABABBAB
```

```output2
0
```

```input3
3 1
BBBAAA
```

```output3
9
```

```input4
10 3
ABABBBBABBABABABAAAA
```

```output4
37
```

## ��ʾ
**���������� #1��**

In this sample input, for example, Bitaro can perform the following operations. Here, the underline denotes the positions of the two beavers swapped by Bitaro.

1. Swap the third beaver and the fourth beaver from the stage right.  
  After this operation, the string which denotes the parts of the beavers from the stage right becomes
$\text{`\texttt{AA\underline{AB}BABBAB}'}$.
2. Swap the eighth beaver and the ninth beaver from the stage right.  
  After this operation, the string which denotes the parts of the beavers from the stage right becomes
$\text{`\texttt{AAABBAB\underline{AB}B}'}$.  

After these operations, Bitaro can allot songs to beavers as follows.

- From the stage right, the $1, 2, 3, 4, 5, 7$-th beavers sing the first song.
- From the stage right, the $6, 8, 9, 10$-th beavers sing the second song.

This way to allot songs to beavers satisfies the conditions.

If the number of operations is less than $2$, there does not exist a way to allot songs to beavers which satisfies the conditions. Therefore, output $2$.

������������������������ơ�

**���������� #2��**

Without performing operations, Bitaro can allot songs to beavers as follows.

- From the stage right, the $1, 2, 3, 5$-th beavers sing the first song.
- From the stage right, the $4, 6, 7, 8$-th beavers sing the second song.
- From the stage right, the $9, 10$-th beavers sing the third song.

This way to allot songs to beavers satisfies the conditions. Therefore, output $0$.

������������������������ơ�

**���������� #3��**

������������������������ơ�

**���������� #4��**

������������������������ơ�

**�����ݷ�Χ��**

�������в������ݣ����� $1\le N\le 10^6$��$1\le K\le N$��$S$ ��һ������Ϊ $2N$ ���ַ��������� $S$ �У���ĸ $\verb!A!$ �� $\verb!B!$ �������� $N$ �Ρ���֤ $N,K$ ��Ϊ������

| �������� | ��ֵ | ���� |
| :----------: | :----------: | :----------: |
| $1$ | $16$ | $N\le 10$ |
| $2$ | $24$ | $N\le 500$ |
| $3$ | $21$ | $N\le 5000$ |
| $4$ | $26$ | $N\le 10^5$ |
| $5$ | $13$ | �� |


