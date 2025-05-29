## ��Ŀ����

Two players play the following game. At the beginning of the game they start with $n$ piles of stones. At each step of the game, the player chooses a pile and remove at least one stone from this pile and move zero or more stones from this pile to any other pile that still has stones. A player loses if he has no more possible moves. Given the initial piles, determine who wins: the first player, or the second player, if both play perfectly.

���� $n$ ��ʯ�ӣ�����������Ϸ��ÿ����ѡһ�ѣ������õ�����һ��ʯͷ��Ȼ���ƶ������ʯ�ӵ�������С�˭�����ƶ��ˣ�˭�����ˡ�

## �����ʽ

Each line of input has one integer $n$, followed by $n$ positive integers denoting the initial piles.

## �����ʽ

For each line of input, output `first player` if first player can force a win, or `second player`, if the second player can force a win.

```input1
3 2 1 3
```

```output1
first player
```

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$1 \le n \le 10^5$��