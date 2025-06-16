


## ��Ŀ����
Bessie the cow is a huge fan of card games, which is quite surprising, given her lack of opposable thumbs. Unfortunately, none of the other cows in the herd are good opponents. They are so bad, in fact, that they always play in a completely predictable fashion! Nonetheless, it can still be a challenge for Bessie to figure out how to win.
Bessie and her friend Elsie are currently playing a simple card game where they take a deck of 2N cards, conveniently numbered 1��2N, and divide them into N cards for Bessie and N cards for Elsie. The two then play NN rounds, where in each round Bessie and Elsie both play a single card. Initially, the player who plays the highest card earns a point. However, at one point during the game, Bessie can decide to switch the rules so that for the rest of the game, the player who plays the lowest card wins a point. Bessie can choose not to use this option, leaving the entire game in "high card wins" mode, or she can even invoke the option right away, making the entire game follow the "low card wins" rule.
Given that Bessie can predict the order in which Elsie will play her cards, please determine the maximum number of points Bessie can win.
��ţBessie��Elsie����һ�ֿ�����Ϸ��һ����2N�ſ��ƣ������ֱ�Ϊ1��2N��ÿͷţ����ֵ�N�ſ��ơ�
��Ϸһ����ΪN�֣���ΪBessie̫�����ˣ�����������Ԥ���ÿ�غ�Elsie���ʲô�ơ�
ÿ����Ϸ���ͷţ�ֱ��һ���ƣ��������߻�ʤ��
ͬʱ��Bessie��һ�λ���ѡ����ĳ��ʱ��㣬���Ǹ�ʱ��ʼ��ÿ�غϵ������߻�ʤ��
Bessie������֪�����Լ�����ܻ�ʤ�����֣�
## �����ʽ
The first line of input contains the value of N (2��N��50,000).
The  next N lines contain the cards that Elsie will play in each of the  successive rounds of the game. Note that it is easy to determine  Bessie's cards from this information.
## �����ʽ
Output a single line giving the maximum number of points Bessie can score.

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
Here, Bessie must have cards 2, 5, and 6, and 7 in her hand, and she can use these to win at most 3 points. For example, she can defeat the 1 card and then switch the rules to "low card wins", after which she can win two more rounds.
## ��Ŀ��Դ
Platinum��лClaris�ṩ����


