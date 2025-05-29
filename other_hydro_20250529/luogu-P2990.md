## ��Ŀ����
The cows have reverted to their childhood and are playing a game similar to human hopscotch. Their hopscotch game features a line of N (3 <= N <= 250,000) squares conveniently labeled 1..N that are chalked onto the grass.

Like any good game, this version of hopscotch has prizes!  Square i is labeled with some integer monetary value V\_i (-2,000,000,000 <= V\_i <= 2,000,000,000). The cows play the game to see who can earn the most money.

The rules are fairly simple:

\* A cow starts at square '0' (located just before square 1; it has no monetary value).

\* She then executes a potentially empty sequence of jumps toward square N. Each square she lands on can be a maximum of K (2 <= K <= N) squares from its predecessor square (i.e., from square 1, she can jump outbound to squares 2 or 3 if K==2).

\* Whenever she wishes, the cow turns around and jumps back towards square 0, stopping when she arrives there. In addition to the restrictions above (including the K limit), two

additional restrictions apply:

\* She is not allowed to land on any square she touched on her outbound trip (except square 0, of course).

\* Except for square 0, the squares she lands on during the return trip must directly precede squares she landed on

during the outbound trip (though she might make some larger leaps that skip potential return squares altogether).

She earns an amount of money equal to the sum of the monetary values of all the squares she jumped on. Find the largest amount of cash a cow can earn.

By way of example, consider this six-box cow-hopscotch course where K has the value 3:

```cpp
Square Num:    0      1      2      3      4      5      6 
+---+  +---+  +---+  +---+  +---+  +---+  +---+ 
|///|--|   |--|   |--|   |--|   |--|   |--|   | 
+---+  +---+  +---+  +---+  +---+  +---+  +---+ 
Value:    -      0      1      2     -3      4      5 
```
One (optimal) sequence Bessie could jump (shown with respective bracketed monetary values) is: 1[0], 3[2], 6[5], 5[4], 2[1], 0[0] would yield a monetary total of 0+2+5+4+1+0=12.

If Bessie jumped a sequence beginning with 0, 1, 2, 3, 4, ... then she would be unable to return since she could not legally jump back to an untouched square.

��ţ�����ڻ�ζͯ�꣬��һ�����������ӵ���Ϸ���������Ϸ���


ţ���ڲݵ��ϻ���һ��N�����ӣ�(3 <=N <= 250,000)�����Ϊ1..N��

�����κ�һ������Ϸһ������������������ϷҲ�н�������i�����ӱ���һ������V\_i(-2,000,000,000 <=V\_i <= 2,000,000,000)��ʾ������ӵ�Ǯ����ţ���뿴�����˭�ܵõ�����Ǯ��

����ܼ򵥣�

\* ÿ����ţ��0�Ÿ��ӳ�����(0�Ÿ�����1��֮ǰ������ûǮ)

\* ����N�Ÿ��ӽ���һϵ�е���Ծ(Ҳ���Բ���)��ÿ���������ĸ��������Ժ�ǰһ����ŵĸ��Ӳ�K��(1 <= K <= N)(�ȷ�˵����ǰ��1�Ÿ�K=2, ��������2�ź�3�Ÿ���)

\*���κ�ʱ����������ѡ���ͷ��0�Ÿ�������ֱ������0�Ÿ��ӡ����⣬�������Ϲ���֮�⣬

��ͷ����ʱ������������

\*����������֮ǰͣ���ĸ��ӡ�

\*����0�Ÿ���֮�⣬���ڻ�����ʱ��ͣ���ĸ��ӱ�����ǡ�ɹ�ȥ��ʱ��ͣ����ĳ�����ӵ�ǰһ��(��Ȼ��Ҳ��������ĳЩ��ȥ��


## �����ʽ
\* Line 1: Two space separated integers: N and K

\* Lines 2..N+1: Line i+1 contains a single integer: V\_i


## �����ʽ
\* Line 1: A single line with a single integer that is the maximum amount of money a cow can earn


```input1
6 3 
0 
1 
2 
-3 
4 
5 

```

```output1
12 

```

