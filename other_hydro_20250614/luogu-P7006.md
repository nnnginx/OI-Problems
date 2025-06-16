## ��Ŀ����


Kabaleo Lite is a board game. The board consists of several stacks of conical chips of various colors. Only the color of the top chip of the stack is visible.

Each player has a unique target color and a set of colored chips. The target color is hidden from other players, while the set of chips is visible to them. On his turn, player selects one of his chips and puts it on one of the board stacks, thus recoloring it to the color of the chosen chip.

After the last turn, the number of visible board chips of each color is calculated. The winning color is the color that occurs the maximum times. The player (if any) that has this color as his target color, wins the game. If there is no such player or if there are two or more colors that occur the maximum times, the game ends in a draw.

You are playing your last chip in the Kabaleo Lite game. Other players also have one chip left. You want to determine all possible moves that lead you to winning the game. You do not know the target colors of other players and you cannot predict their moves, so your move must guarantee your victory regardless of moves of your opponents.



## �����ʽ


The first line contains four integers $n , p , c$ and $h$ -- the number of stacks on the board $(1 \le n \le 10^{6}),$ the number of players $(1 \le p \le 10^{6}),$ the number of chips' colors $(p \le c \le 10^{6}),$ and your hidden color $(1 \le h \le c)$ .

The second line contains $n$ integers $b_{i}$ -- the color of the visible board chip for each stack on the board $(1 \le b_{i} \le c)$ .

The third line contains $p$ integers $l_{i}$ -- the color of the last chip for each player $(1 \le l_{i} \le c)$ . The players are numbered from one (you) to $n$ in the order of their turns.



## �����ʽ


The first line must contain $w$ -- the number of winning moves.

The second line must contain $w$ distinct numbers $m_{i}$ -- the numbers of the stacks on which your chip should be put to win. Stacks are numbered starting from $1$ in the order that their visible colors are given in the input file. You can output their numbers in any order on this line.

Remember, that your move should be winning regardless of the moves of all other players.



## ��Ŀ����
��һ��������Ϸ���������� $n$ �����ӣ�ÿ�������Ͽ��Զѵ����ɸ�����ɫ�ĳ��룬ֻ��ÿ�����������Ϸ��ĳ������ɫ�ǿɼ��ġ�

�μ���Ϸ��ÿ����Ҷ��и��Բ�ͬ��һ��Ŀ����ɫ���Լ�һЩ��ɫ���롣ÿ����ֻ֪���Լ���Ŀ����ɫ��������ӵ�еĳ�����ɫ���������ǹ����ġ�ÿ���غ��У��������������������ѡһ�����ӷ��ó��룬ͬʱ�����·��ĳ��롣��Ϸ���������������Ͽɼ�������������ɫ���Ը���ɫΪĿ����ɫ����Ҽ���ʤ��������ɫ�����κ���ҵ�Ŀ����ɫ�����������ϳ���������ɫ��Ψһ������Ϸƽ�֡�

���ڣ�һ����Ϸ���е�������������������Ҷ�ֻʣ���һ�����롣����ǡ���ֵ���������ڲ�֪�������˵�Ŀ����ɫ��ǰ���£�����֪����һ������Щ�������Ա�֤��ʤ��

### �����ʽ

��һ�� $4$ ������ $n,p,c,h$���ֱ��ʾ���̸������������������ɫ���������Ŀ����ɫ��

�ڶ��� $n$ ������ $b_i$����ʾ���������еĳ�����ɫ�����̸��Ŵ� $1$ ��ʼ��

������ $p$ ������ $l_i$����ʾÿ����ҵ����һö�������ɫ����ұ�Ŵ��㿪ʼ��

### �����ʽ

��һ�� $1$ ������ $w$����ʾ���ж����ֱ�ʤ������

�ڶ��� $w$ ������ $m_i$����ʾ��Ӧ�ðѳ�������ĸ������ϡ�˳���ޡ�

���ݷ�Χ��ԭ�⡣

```input1
6 3 4 2
2 1 2 3 2 2
2 1 1

```

```output1
1
2

```

## ��ʾ
Time limit: 1 s, Memory limit: 128 MB. 



