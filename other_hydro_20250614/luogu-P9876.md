## ��Ŀ����
Prof. Pang is playing a card game with his two friends Alice and Bob. All cards are drawn from a standard 52-card deck. A standard 52-card deck comprises $13$ ranks in each of the four French suits: clubs ($\clubsuit$), diamonds ($\diamondsuit$), hearts ($\heartsuit$) and spades ($\spadesuit$). Each suit includes an Ace (A), a King (K), a Queen (Q), and a Jack (J), each depicted alongside a symbol of its suit; and numerals or pip cards from the Deuce (Two) to the Ten, with each card depicting that many symbols (pips) of its suit. $\textbf{No card can be drawn more than once.}$

![](https://cdn.luogu.com.cn/upload/image_hosting/3xtu6g4z.png)

Individual cards are ranked as follows (high-to-low): A, K, Q, J, 10, 9, 8, 7, 6, 5, 4, 3, 2. $\textbf{Suits do not affect ranks of the cards.}$ For example, Ace of diamonds and Ace of clubs have the same rank. No one of them is ranked strictly higher than the other.

Initially, Alice and Bob will hold one or more cards while Prof. Pang will hold exactly one card. $\textbf{Each player can see cards held by himself/herself and cards held by other players.}$ They will play the game in the following multi-round rule:

- The initiative player chooses one card and put it out to start one round.
- The next player can pass or put out a new card, then the player after the next can also pass or put out a new card, and so on. The only constraint is that the rank of the newly put card should be strictly higher than all previous cards in this round.
- The round ends when two players choose to pass consecutively. The one who put out the last card becomes the initiative player in the next round.
- If someone put out all the cards in his/her hand, the game ends immediately.

In this game, Alice is the initiative player in the first round. Bob, Prof. Pang,  and Alice are the next players of Alice, Bob,  and Prof. Pang respectively. Prof. Pang will be happy if and only if he is the one that first put out all the cards. (Prof. Pang wants to be happy, of course.) Alice wants to drink milk tea so she decides to make Prof. Pang happy and then asks him to buy milk tea for her. However, Bob doesn't want it to happen, so he decides to avoid Prof. Pang from being happy. If they play the game optimally for themselves, will Prof. Pang be happy in the end?

## �����ʽ
The first line contains a single integer $T$ ($1\le T \le 10^4$) denoting the number of test cases. For each test case:

The first line contains two integers $n,m$ ($1\le n,m \le 50$) denoting the number of cards in Alice's hand and Bob's hand initially.

The second line contains $n$ strings $a_i$ ($1\le i \le n$) denoting the cards in Alice's hand.

The third line contains $m$ strings $b_i$ ($1\le i \le m$) denoting the cards in Bod's hand.

The fourth line contains one string $p$ denoting the card in Prof. Pang's hand.

For each card, the first character of its corresponding string denotes its rank. (Possible ranks are `2` ,`3`,`4`,`5`,`6`,`7`,`8`,`9`,`T`,`J`,`Q`,`K`,`A`. `T` denotes $10$.) The second character denotes its suit. `C` denotes clubs. `D` denotes diamonds. `H` denotes hearts. `S` denotes spades.

It is guaranteed that each card appears at most once in one test case.

## �����ʽ
For each test case, print one line. Print $\texttt{Pang}$ if Prof. Pang will be happy. Otherwise, print $\texttt{Shou}$.

## ��Ŀ����
��ˡ�������¬��ΰ�ڴ����涷������

+ ��Ϊ¬��ΰ�����ٱ��ɻ�ը�����������������**ֻ�ܳ�����**���ƵĴ�С����Ϊ����С�����о٣���$2,3,4,5,6,7,8,9,\texttt{T},\texttt{J},\texttt{Q},\texttt{K},\texttt{A}$��
+ ��Ϊ�����ɫä�������Ƶ�**��ɫ�޹ؽ�Ҫ**����������������ͬʱû�д�С֮�֣���
+ ��Ϊ�����������ˣ�����������**���ƴ�**��
+ �������ͨ������һ����
    + ������ѡһ���ƣ����ȥ��ʼ��һ�ֱ�����
    + ��һ����ҿ��Գ��ƻ�������������������ֵ**�ϸ����**��һ���ơ�
    + ���������������������һ����ҿ�ʼһ���µĻغϣ�����һ����ҳ�Ϊ����������
    + ˭���ƴ��˭��Ӯ�ˡ�
   
���ڣ�����һ���о֣����ʣ $n$ ���ƣ�����ʣ $m$ ���ƣ���������ʦ¬��ΰֻʣһ�����ˡ�

��������һ���غϣ�˳������ˡ�������¬��ΰ���������¬��ΰӮ����������¬��ΰ�䡣

��Ϊ��������Ƭ�������붷�������Ƽң����˶����������������˭��Ӯ��¬��ΰӮ��� `Pang`��������� `Shou`��ע��**���Ӯ����¬��ΰӮ**��

translated by ¬��ΰ��

```input1
2
2 2
2H 2D
3H 3D
4S
2 2
2H 2D
3H 4D
4S
```

```output1
Pang
Shou
```

## ��ʾ
- For the first case, Prof. Pang can always put out his only card ``4S``.
- For the second case, Bob can put out ``4D`` and become the initiative player in the second round regardless of the card Alice put out in the first round, then Bob put out ``3H`` and the game ends.

