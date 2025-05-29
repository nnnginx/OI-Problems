## ����
Dicing is a two-player game and its outcome is fully random. Lately its popularity increases all over Byteotia. There is even a special club for dicing amateurs in the capital city of Byteotia. The club patrons take their time talking to each other and playing their favourite game with a randomly chosen opponent every once in a while. Everyone who wins the most games one day gains the title of the lucky chap. Sometimes it happens that the night at the club is a quiet one and only few games are played. It is a time when even one win can make you a lucky chap.

Once upon a time a most unlucky fellow, Byteasar, won the glorious title. He was so deeply shocked that he completely forgot how many games he had won. Now he is wondering how good his luck was and whether fortune finally smiled upon him - perhaps his luck changed for good? He knows exactly how many games and between whom were played that lucky night. However, he does not know the results. Byteasar desires to find out what is the smallest number of wins that could provide the title of the lucky chap. Be a good fellow and help him satisfy his curiosity!

TaskWrite a programme that:

for each game played reads from the standard input the pair of players who competed in it.

finds the smallest number $k$, such that a set of games' outcomes exists in which each player wins $k$ games at the most,writes the number $k$ and the results of games in the found set to the standard output.

��������һ��˫����Ϸ�����Ľ������ȫ����ġ������������ Byteotia ��÷ǳ����С��� Byteotia ���׶�������һ���ر��������ҵ�మ���߾��ֲ������ֲ����������ǻ�ʱ�以�����첢ÿ��һ���Ӿͺ�һ�����ѡ��Ķ�������������ϲ������Ϸ��һ����Ӯ�������Ϸ���˻�õ��������ߡ�ͷ�Ρ���ʱ���Ͼ��ֲ��ܰ�����ֻ�к��ٵı�������������Ӯһ��Ҳ�ܻ�á������ߡ�ͷ�ε�ʱ�䡣

�ܾúܾ���ǰ��һ���ܲ����˵��ˣ��� Byteasar��Ӯ����������ٵ�ͷ�Ρ����������������������ȫ�������Ѿ�Ӯ�˶��ٳ�����������֪�����ж����ˣ��Լ�����֮���Ƿ����ջ�����΢Ц����Ҳ�������������ã���ȷ�е�֪�����Ǹ����˵������ж��ٳ���Ϸ�Լ���˭��ġ�Ȼ��������֪�������Byteasar ϣ����������ҪӮ�������ܻ�á������ߡ�ͷ�Ρ��������ˣ������������ĺ����İɣ�

����ÿ����Ϸ�Ӷ����ⳡ��Ϸ��һ������ҵ���С���� $k$��ʹ�ô���һ����Ϸ����ļ��ϣ�����Ӯ�������Ӯ�� $k$ ��������� $k$ ���ҵ��ļ�������Ϸ�Ľ��

## �����ʽ
In the first line of the standard input there is a pair of integers $n$ and $m$ separated by a single space, $1\le n\le 10^4$, $0\le m\le 10^4$; $n$ denotes the number of players, while $m$ is the number of games. The players are numbered from $1$ to $n$. In the following $m$ lines there are pairs of players' numbers depicting the sequence of games, separated by single spaces. One pair may occur many times in the sequence.

�����һ����һ��һ����һ���ո�ֿ����� $n$ �� $m$��$n$ ��ʾ�������$m$ ��ʾ��Ϸ������Ҵ� $1$ �� $n$ ��š��ڽ�������m������ÿ����Ϸ��һ����ҵı�ţ���һ���ո�ֿ�����������Ϸ�����С�һ����ҿ��ܻ�����������ж�γ��֡�

## �����ʽ
The first line of the standard output should contain the determined number $k$. For each pair of players' numbers $a$, $b$ specified in the $i$'th line of the input, in the $i$'th line of the output the number $1$ should be written if the player no. $a$ wins against player no. $b$ in the found set of outcomes, or $0$ otherwise.

�����һ��Ӧ�ð���һ��ȷ������ $k$������������ĵ� $i$ ��ָ����һ����� $a, b$��������ҵ��Ľ�������� $a$ ʤ�� $b$����������ĵ� $i$ ����� `1`, ������� `0`.

## ��������
```plain
4 4
1 2
1 3
1 4
1 2
```

## �������
```plain
1
0
0
0
1
```

## ���ݹ�ģ��Լ��

���� $100 \%$ �����ݣ� $1 \le n,m \le 10^4$