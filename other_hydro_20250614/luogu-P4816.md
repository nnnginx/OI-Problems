## ��Ŀ����
Bessie the cow is a huge fan of card games, which is quite surprising, given her lack of opposable thumbs. Unfortunately, none of the other cows in the herd are good opponents. They are so bad, in fact, that they always play in a completely predictable fashion! Nonetheless, it can still be a challenge for Bessie to figure out how to win.

Bessie and her friend Elsie are currently playing a simple card game where they take a deck of $2N$ cards, conveniently numbered $1��2N$, and divide them into $N$ cards for Bessie and $N$ cards for Elsie. The two then play $N$ rounds, where in each round Bessie and Elsie both play a single card. In the first $N/2$ rounds, the player with the highest card earns a point, and in the last $N/2$ rounds, the rules switch and the player who plays the lowest card wins a point.

Given that Bessie can predict the order in which Elsie will play her cards, please determine the maximum number of points Bessie can win. 

## �����ʽ
The first line of input contains the value of $N$ ($2 �� N �� 50,000$; N will be even).

The next $N$ lines contain the cards that Elsie will play in each of the successive rounds of the game. Note that it is easy to determine Bessie's cards from this information. 

## �����ʽ
 Output a single line giving the maximum number of points Bessie can score. 

## ��Ŀ����
### ��Ŀ����

��ţ Bessie �ǿ�����Ϸ�Ŀ��Ȱ����ߣ�������û�ж���Ĵָ�����Ⲣ��Ӱ���������顣�ź����ǣ�����ͬ�����ڿ�����Ϸ����ˮƽ���ǣ���������˳����ȫ��Ԥ�⣡������ˣ�Bessie ���辫�Ĳ߻����ܻ�ʤ��

Bessie ���������� Elsie ������һ���򵥵Ŀ�����Ϸ������ʹ��һ������ $2N$ �ſ��Ƶ����飨���Ϊ $1 \ldots 2N$���������Ʒֳɸ� $N$ �š������� $N$ �ֱ�����ÿ��˫�������һ���ơ���ǰ $N/2$ ���У�����ϴ����ֵ���ҵ� 1 �֣��ں� $N/2$ ���У�����ת�������С���ֵ���ҵ� 1 �֡�

��֪ Bessie ����Ԥ֪ Elsie ÿ�ֳ��Ƶ�˳������� Bessie �ܹ���õ���������

### �����ʽ

��һ������������� $N$��$2 \leq N \leq 50,000$���� $N$ Ϊż������

������ $N$ �а�˳����� Elsie ��ÿ�ֱ����н�����Ŀ��ơ�ע�������Щ��Ϣ�����ƶϳ� Bessie ���еĿ��ơ�

### �����ʽ

���һ�У����� Bessie �ܹ���õ���������

### ˵��/��ʾ

�ڴ������У�Bessie ���еĿ���Ϊ $2$��$5$��$6$ �� $7$��������ͨ���ڱ������α��� $2$ �����ƣ��Ӷ������ 2 �֡�

��Ŀ�ṩ�ߣ�Brian Dean

```input1
4
1
8
4
3

```

```output1
2
```

## ��ʾ
Here, Bessie must have cards 2, 5, and 6, and 7 in her hand, and she can use these to win at most 2 points, by saving her '2' card until one of the hands in the second half of the game.

Problem credits: Brian Dean 

