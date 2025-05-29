## 描述
Dicing is a two-player game and its outcome is fully random. Lately its popularity increases all over Byteotia. There is even a special club for dicing amateurs in the capital city of Byteotia. The club patrons take their time talking to each other and playing their favourite game with a randomly chosen opponent every once in a while. Everyone who wins the most games one day gains the title of the lucky chap. Sometimes it happens that the night at the club is a quiet one and only few games are played. It is a time when even one win can make you a lucky chap.

Once upon a time a most unlucky fellow, Byteasar, won the glorious title. He was so deeply shocked that he completely forgot how many games he had won. Now he is wondering how good his luck was and whether fortune finally smiled upon him - perhaps his luck changed for good? He knows exactly how many games and between whom were played that lucky night. However, he does not know the results. Byteasar desires to find out what is the smallest number of wins that could provide the title of the lucky chap. Be a good fellow and help him satisfy his curiosity!

TaskWrite a programme that:

for each game played reads from the standard input the pair of players who competed in it.

finds the smallest number $k$, such that a set of games' outcomes exists in which each player wins $k$ games at the most,writes the number $k$ and the results of games in the found set to the standard output.

掷骰子是一种双人游戏，它的结果是完全随机的。最近它在整个 Byteotia 变得非常流行。在 Byteotia 的首都甚至有一个特别的掷骰子业余爱好者俱乐部。俱乐部的老主顾们花时间互相聊天并每隔一阵子就和一个随机选择的对手玩这他们最喜欢的游戏。一天中赢得最多游戏的人会得到“幸运者”头衔。有时晚上俱乐部很安静，只有很少的比赛。这是哪怕赢一场也能获得“幸运者”头衔的时间。

很久很久以前有一个很不走运的人，叫 Byteasar，赢得了这个光荣的头衔。他被深深地震惊了以至于完全忘了他已经赢了多少场。现在他想知道他有多幸运，以及幸运之神是否最终会向他微笑——也许他的运气会变好？他确切地知道在那个幸运的晚上有多少场游戏以及是谁玩的。然而，他不知道结果。Byteasar 希望查明至少要赢几场才能获得“幸运者”头衔。做个好人，帮他满足他的好奇心吧！

对于每场游戏从读入这场游戏的一对玩家找到最小的数 $k$，使得存在一个游戏结果的集合，其中赢最多的玩家赢了 $k$ 场。输出数 $k$ 和找到的集合中游戏的结果

## 输入格式
In the first line of the standard input there is a pair of integers $n$ and $m$ separated by a single space, $1\le n\le 10^4$, $0\le m\le 10^4$; $n$ denotes the number of players, while $m$ is the number of games. The players are numbered from $1$ to $n$. In the following $m$ lines there are pairs of players' numbers depicting the sequence of games, separated by single spaces. One pair may occur many times in the sequence.

输入第一行有一个一对由一个空格分开整数 $n$ 和 $m$。$n$ 表示玩家数，$m$ 表示游戏数。玩家从 $1$ 到 $n$ 编号。在接下来的m行中有每场游戏的一对玩家的编号，由一个空格分开，描述了游戏的序列。一对玩家可能会在这个序列中多次出现。

## 输出格式
The first line of the standard output should contain the determined number $k$. For each pair of players' numbers $a$, $b$ specified in the $i$'th line of the input, in the $i$'th line of the output the number $1$ should be written if the player no. $a$ wins against player no. $b$ in the found set of outcomes, or $0$ otherwise.

输出第一行应该包含一个确定的数 $k$。对于在输入的第 $i$ 行指定的一对玩家 $a, b$，如果在找到的结果集合中 $a$ 胜过 $b$，则在输出的第 $i$ 行输出 `1`, 否则输出 `0`.

## 输入样例
```plain
4 4
1 2
1 3
1 4
1 2
```

## 输出样例
```plain
1
0
0
0
1
```

## 数据规模及约定

对于 $100 \%$ 的数据： $1 \le n,m \le 10^4$