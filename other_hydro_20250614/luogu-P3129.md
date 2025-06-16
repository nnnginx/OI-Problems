## ��Ŀ����
Bessie the cow is a hu e fan of card games, which is quite surprising, given her lack of opposable thumbs. Unfortunately, none of the other cows in the herd are good opponents. They are so bad, in fact, that they always play in a completely predictable fashion! Nonetheless, it can still be a challenge for Bessie to figure out how to win.

Bessie and her friend Elsie are currently playing a simple card game where they take a deck of $2N$ cards, conveniently numbered $1 \ldots 2N$, and divide them into $N$ cards for Bessie and $N$ cards for Elsie. The two then play $N$ rounds, where in each round Bessie and Elsie both play a single card. Initially, the player who plays the highest card earns a point. However, at one point  during the game, Bessie can decide to switch the rules so that for the rest of the game, the player who plays the lowest card wins a point.  Bessie can choose not to use this option, leaving the entire game in "high card wins" mode, or she can even invoke the option right away, making the entire game follow the "low card wins" rule.

Given that Bessie can predict the order in which Elsie will play her cards, please determine the maximum number of points Bessie can win.

## �����ʽ
The first line of input contains the value of N ($2 \leq N \leq 50,000$).

The next N lines contain the cards that Elsie will play in each of the successive rounds of the game.  Note that it is easy to determine Bessie's cards from this information.

## �����ʽ
Output a single line giving the maximum number of points Bessie can score.


## ��Ŀ����
### ��Ŀ����

��ţ Bessie �ǿ�����Ϸ�Ŀ��Ȱ����ߣ����൱���˾��ȣ���Ϊ��û��������ָ�����ҵ��ǣ�ţȺ�е�������ţ�����ǺõĶ��֡���ʵ�ϣ����ǵı��ַǳ���⣬��������ȫ��Ԥ��ķ�ʽ���ƣ�������ˣ��� Bessie ��˵����λ�ʤ��Ȼ��һ����ս��

Bessie ���������� Elsie ������һ���򵥵Ŀ�����Ϸ��������һ�� $2N$ ���ƣ�����ر��Ϊ $1 \ldots 2N$��������ֳ� $N$ ���Ƹ� Bessie �� $N$ ���Ƹ� Elsie��Ȼ�����˽��� $N$ ����Ϸ��ÿ�� Bessie �� Elsie �����һ���ơ��������������Ƶ���ҵ�һ�֡�Ȼ��������Ϸ�е�ĳ��ʱ�̣�Bessie ���Ծ����ı����ʹ���ڽ���������Ϸ�У���������Ƶ���ҵ�һ�֡�Bessie ����ѡ��ʹ�����ѡ���������Ϸ�����ڡ����ƻ�ʤ��ģʽ��������Ҳ���������������ѡ���������Ϸ��ѭ�����ƻ�ʤ���Ĺ���

��֪ Bessie ����Ԥ�� Elsie ���Ƶ�˳����ȷ�� Bessie ���Ի�õ���������

### �����ʽ

����ĵ�һ�а��� $N$ ��ֵ��$2 \leq N \leq 50,000$����

�������� $N$ �а��� Elsie ����Ϸÿ���н�Ҫ������ơ�ע�⣬����Щ��Ϣ�п��Ժ����׵�ȷ�� Bessie ���е��ơ�

### �����ʽ

���һ�У���ʾ Bessie ���Ի�õ���������

### ˵��/��ʾ

�����Bessie ���е��Ʊ����� 2��5��6 �� 7����������������Щ��Ӯ�� 3 �֡����磬�������Ȼ��� 1 �����ƣ�Ȼ�󽫹����л�Ϊ�����ƻ�ʤ����֮����������Ӯ�����֡�

```input1
4
1
8
4
3
```

```output1
3
```

## ��ʾ
Here, Bessie must have cards 2, 5, and 6, and 7 in her hand, and she can use these to win at most 3 points.  For example, she can defeat the 1 card and then switch the rules to "low card wins", after which she can win two more rounds.

