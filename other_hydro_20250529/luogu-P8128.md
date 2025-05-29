## ��Ŀ����
ICPC2020 WF A

## ��Ŀ����
The Great Cardoni, Master Prestidigitator, has a deck of 21 numbered cards which he uses in a
trick as follows:

> A spectator secretly selects a number between $1$ and $21$, inclusive, after which
> Cardoni deals the $21$ cards, face-up, row by row in order from $1$ to $21$,
> into a
> $3$-column grid. The spectator then indicates which of the three
> columns contains the selected card, at which point the magician picks up
> the cards by columns, picking up the specified column second (the
> order of collecting the other two columns is unimportant).
> Cards are collected face up, beginning with the top card in each column and
> placing each succeeding card immediately beneath the previously collected card.
> The cards are then redealt by rows into a $3$-column grid, starting from the
> top of the face-up deck. The process is
> repeated two more times; each time, the column indicated by the spectator
> is the second column picked up by the magician. After three such
> iterations, Cardoni announces, "I have penetrated to the heart of your
> mind; your card lies at the heart of this display." And it's true---the
> selected card is located at the "heart" of the array (row four, column
> two). Moreover, the selected card will always remain in this stable
> location for any further iterations of the column indication and card
> redealing process.

The process always works, no matter the number selected, provided that
the column containing the secret number is the second column to be
picked up and redealt.

Cardoni would like to expand his trick to use different numbers of
cards, rows, and columns, and to experiment with different orderings
of picking up the columns after the spectator indicates a
column. However, it is not a trivial problem. For instance, when using $24$
cards in $8$ rows and $3$ columns, and always picking up the indicated
column as the second one to redeal, the number $5$ eventually
ends up in stable location row $4$, column $3$, while the number $20$
ends up in stable location row $5$, column $1$. Also, neither location
is one of the two "heart" positions in column $2$ of rows $4$ or
$5$.  Moreover, Cardoni is uncertain of how many iterations of the
"indicate column and redeal" process are needed before a
selected card reaches a stable location.

Given the number of rows and columns of cards, help Cardoni set up his
trick in such a way that there is a unique stable location that is as
close to the center as possible.

## �����ʽ
The input consists of a single line with two integers $r$ and $c$ ($2 \le r, c \le 10^6$), the number of rows and columns used in the trick.
The cards are numbered from $1$ to $r \cdot c$ and are initially dealt row by row in increasing order.

## �����ʽ
Output a line containing four integers $p$, $i$, $j$, and $s$, where:

- the column indicated by the spectator should be picked up as the $p^{\text{th}}$ column,
- using this value of $p$ causes all cards to eventually end up in the stable location at row $i$ column $j$, and
- $s$ is the maximum number of iterations required for any card to reach the stable location.

The value of $p$ should be chosen so that the stable location $(i, j)$
is as close as possible to any of the one, two or four central
positions in the grid, where the distance between locations $(i, j)$
and $(i', j')$ is $|i-i'| + |j-j'|$.  If more than one value of $p$
results in the same minimum distance, choose the smallest such $p$.


## ��Ŀ����
�������ܵ�ѡ��һ������1��21֮�䣨����1��21�������֣�Ȼ�󿨶��Ὣ��21�����泯�ϣ���1��21��˳�����з���һ��3�е������С�Ȼ�����ָ�������е���һ�а�����ѡ���ƣ���ʱħ��ʦ����ʰȡ�ƣ�Ȼ��ʰȡָ�����У��ռ��������е�˳����Ҫ������Ƭ�ռ�ʱ�泯�ϣ���ÿ����������Ŀ�Ƭ��ʼ��Ȼ������ÿ�ſ�Ƭ����֮ǰ�ռ��Ŀ�Ƭ�����·���Ȼ�󣬴����泯�ϵĿ�Ƭ�鶥����ʼ������Ƭ�����������е�3�е������С��ù������ظ����Σ�ÿһ�Σ�����ָʾ������ħ��ʦʰȡ�ĵڶ������������������ķ���֮�󣬿����������������Ѿ����뵽��������ģ������λ������չʾ�ĺ��ġ���������ġ�����ѡ�Ŀ�λ������ġ����ġ��������У��ڶ��У������⣬��ѡ����ʼ�ձ����ڸ��ȶ�λ�ã��Ա��һ��������ָʾ�Ϳ����µ������̡�



ֻҪ�������ܺŵ�����Ҫʰȡ�������滻�ĵڶ��У�������ѡ��������Ƕ��٣��ù���ʼ����Ч��



����������չ���ļ��ɣ�ʹ�ò�ͬ�����Ŀ�Ƭ���к��У����ڹ���ָʾһ�к󣬳��Բ�ͬ��˳��ʰȡ�С�Ȼ�����ⲻ��һ��΢����������⡣���磬����8��3����ʹ��24�ſ�����ʼ�ս�ָʾ����Ϊ�ڶ�������ָ������ʱ������5���ջ����ȶ�λ�õ�4�е�3�н�����������20�������ȶ�λ�õ�5�е�1�н��������⣬����λ�ö����ǵ�4�л��5�е�2���е����������ࡱλ��֮һ�����⣬Cardoni��ȷ����ѡ���Ŀ������ȶ�λ��֮ǰ����Ҫ���ٴΡ�ָʾ�к�����ָ�������̵ĵ�����



���ǵ���Ƭ�������������������������������ļ��ɣ�ʹ����һ�����ص��ȶ�λ�ã������ܿ������ġ�

#### ���ݷ�Χ
$2 \le r, c \le 10^6$��r��c�У�

```input1
7 3
```

```output1
2 4 2 3
```

```input2
8 3

```

```output2
1 1 1 3
```

