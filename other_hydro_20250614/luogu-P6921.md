## ��Ŀ����
My birthday is coming up. Alas, I am getting old and would like to feel young again. Fortunately, I have come up with an excellent way of feeling younger: if I write my age as a number in an appropriately chosen base $b$, then it appears to be smaller. For instance, suppose my age in base $10$ is $32$. Written in base $16$ it is only $20$!

However, I cannot choose an arbitrary base when doing this. If my age written in base $b$ contains digits other than $0$ to $9$, then it will be obvious that I am cheating, which defeats the purpose. In addition, if my age written in base $b$ is too small then it would again be obvious that I am cheating.

Given my age $y$ and a lower bound $\ell $ on how small I want my age to appear, find the largest base $b$ such that $y$ written in base $b$ contains only decimal digits, and is at least $\ell $ when interpreted as a number in base $10$.

## �����ʽ
The input consists of a single line containing two base 10 integers $y$ ($10 \le y \le 10^{18}$ �C yes, I am very old) and $\ell $ ($10 \le \ell \le y$).

## �����ʽ
Display the largest base $b$ as described above.

## ��Ŀ����
# ��Ŀ����
�ҵ����տ쵽�ˣ�������������Ѿ����ˣ��������»������ĸо���

���˵��ǣ��������һ�����˸о�������ĺ÷���������Ұ��ҵ��������ʵ�ѡ���$b$������д����ô�����������С�����磬��������$10$������д��������$32$�ꣻ��$16$������д����ֻ��$20$($0x20$)��

Ȼ������������ʱ���Ҳ���ѡ������������������$b$����Ϊ��д���ҵ��������$0-9$��������֣���ô�������������ף���Υ����Ŀ�ġ����⣬����ҵ�����Ľ�����$b$̫С����ô�������������ס�

����ϣ���ҵ����俴�����ж�С��������,���ǵ��ҵ�����$y$������$l$���ҵ����Ľ�����$b$������д�ڻ���$b$�е�$y$ֻ����ʮ�������֣����ҵ����俴��һ��ʮ��������ʱ������$l$��
# �����ʽ
������һ����ɣ����а�������$10$���Ƶ�����$y$ ($10\le y\le10^{18}$ �C�ǵ�,�Һ��ϣ���$l$($10\le l \le y$)
# �����ʽ
���������������������$b$��
# ˵��/��ʾ
ʱ�����ƣ�$1s$���ڴ����ƣ�$1GB$

(�������ʵ����$512MB$,��ԭ����$1GB$)

$2016��$���ʴ�ѧ����̴���$ACM$-$ICPC$�����ܾ���

```input1
32 20

```

```output1
16

```

```input2
2016 100

```

```output2
42

```

## ��ʾ
Time limit: 1000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2016

