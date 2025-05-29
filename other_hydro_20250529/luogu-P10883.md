## ��Ŀ����
������ [COCI 2017/2018 Contest #2](https://hsin.hr/coci/archive/2017_2018/) T3��Doktor����[ԭ������](https://hsin.hr/coci/archive/2017_2018/contest2_tasks.pdf)��

Special Judge �ɰ������ṩ������й���˽�ţ�лл��

## ��Ŀ����
> And the Mrs, Ms, says:
>
>"I've been riding horses for fifteen years, and it is impossible to shoe a horse upside down!"
>
> (��)

"Yes, that's upside down" - whispers Domagoj, looking at Mate's hand while playing, for the purposes of this task, a heavily modified version of the card game Hanabi. For the sake of simplicity, Mate is holding $N$ cards in his hands, numbered from $1,2,\dots,N$
 in a certain order. (Each number from $1$ to $N$
appears exactly once.) As when playing the real game, he cannot voluntarily change the card order.

Just so the task is at least somewhat related to the story, Domagoj will point for Mate to a contiguous subarray of cards. (He can point to a single card too, but he will point to at least one card.) Mate will then "rotate" that contiguous subarray and put it back.

(The rotating can be thought of as taking all the cards in the given subarray and rotating all of them for 180 degrees. This means that the first and last card swap places, as well as the second and the second to last card, and so on.)

Like all of us, Domagoj is very fond of fixed points. In other words, cards whose numbers match their position in hand, counting from Domagoj's left side. Therefore, he'd like the number of fixed points to be as great as possible after rotating the given subarray.

Help Domagoj find out which contiguous subarray he needs to point out so that the number of fixed points in Mate's hand after rotating that subarray is maximal.

## �����ʽ
 The first line of input contains the positive integer $N (1 \leq N \leq 500000)$, the number of cards in Mate's hand.
 
 The following line contains the numbers on the cards in Mate's hand in the order that Domagoj sees them.

## �����ʽ
 You must output a single line containing $A$ and 
$B$, the numbers on the cards that are the beginning and the end of the required contiguous subarray, in that order. If there are multiple options, output any of them.

## ��Ŀ����
��һ����Ϊ $N(N\leq 5\times 10^5)$ ������ $a$�����ֵ����Ϊ $\sum\limits_{i=1}^N [a_i=i]$���������������� $a_i = i$  �� $i(1\leq i \leq n)$ �ĸ�����

����Է�תĳһ�����䣬��һ�β���֮�����ļ�ֵ����תָ���ǽ�����ǰ��ߵ������練ת `3 2 1 4` ��õ� `4 1 2 3`��

ע�⣬����Ҫ�����**������**����ֵ�������������֮�����ȡ������ֵ��**��ת��������Ҷ˵���ԭ�����е�ֵ**���������� 1 �У���ת $[1,3]$ �����Ž⣬��Ӧ�����ԭ�����еķ�ת����Ķ˵��±��Ӧ��ֵ $a_1=3$ �Լ� $a_3=1$��

�����ж���⣬������������һ�顣

```input1
4
3 2 1 4
```

```output1
3 1
```

```input2
2
1 2
```

```output2
1 1
```

```input3
7
3 6 5 7 4 1 2 
```

```output3
3 2
```

## ��ʾ
In the first test case, after rotating the contiguous subarray that starts with 3 and ends with 1, the cards will be ordered 1 2 3 4, and now all the cards are fixed points. In this example, the given output is the only correct output.

 In the second test case, rotating any subarray consisting of only one card results with the same card order, the one that produces the maximal number of fixed points.

