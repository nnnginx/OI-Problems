## ��Ŀ����
![](https://cdn.luogu.com.cn/upload/image_hosting/9ez2u5m2.png)

Blue-edged Shot is forbidden from playing Genshin Impact by LeavingZ, so she turned to Go game.

A game of Go involves two players, one playing with Black stones and the other with White stones. Two players take turns making moves, with the Black stones going first. The Go board is composed of a grid of $19\times 19$ intersections, and we use $(x,y)$ to represent the intersection at the $x$-th row and $y$-th column. The stones are placed on the intersections. The top left corner is $(1,1)$, while the bottom right corner is $(19,19)$.

The intersections $(x_1,y_1)$ and $(x_2,y_2)$ are adjacent if and only if $|x_1-x_2| + |y_1-y_2| = 1$. Adjacent intersections with stones of the same color belong to the same group of stones. The number of `liberties` for a stone is equal to the number of adjacent intersections to the stone's intersection that do not have any stones on them. The liberties of a group of stones equal the sum of the liberties of all the stones belonging to that group. A group of stones with zero liberties is considered dead and must be removed from the board.

Note that after Black plays, priority is given to removing any dead White stones, and then recalculating the liberties for Black stones. This is because there might be situations where, after Black plays, both Black and White stones have zero liberties, but removing the dead White stones increases the liberties for Black stones. As for White, process the stones similarly. After White plays, priority is given to removing any dead Black stones, and then recalculating the liberties for White stones.

Now there is a game of Go, starting with an empty board, and a total of $m$ moves have been made by both players. Given the positions where each stone is placed, output after each move, how many Black and White stones are removed respectively causing by this move. Obviously, black stones are played on odd-numbered moves, and white stones are played on even-numbered moves. It's guaranteed that stones are placed on empty intersections. Note that stones can be placed on $\textbf{any}$ intersections that do not have stones on them at the moment, regardless of violating the Go rules in real life.

## �����ʽ
Input $m$ ($1 \le m \le 5\times 10^5)$ lines, the $i$-th line contains two integers $x_i,y_i$ ($1 \le x_i,y_i \le 19$), representing the $i$-th move puts stone on $(x_i,y_i)$.

It's guaranteed that stones are placed on intersections that do not have stones on them at the moment.

## �����ʽ
Output $m$ lines, each line contains two integers. The first integer in the $i$-th line represents the number of Black stones removed after the $i$-th move, while the second for White stones.

## ��Ŀ����
### ��������

LeavingZ���㱻��ֹ�桶ԭ�񡷡�


### ��Ŀ����

����Ǧ����LeavingZ�Ľ�ֹ���޷��桶ԭ�񡷣�������ת����Χ�塣

Χ����Ϸ��������ҽ��У�һ��ʹ�ú��ӣ���һ��ʹ�ð��ӡ���������������ӣ��������С�Χ��������$19\times 19$�Ľ������ɣ�������$(x,y)$��ʾ��$x$�е�$y$�еĽ���㡣���ӷ����ڽ�����ϡ����Ͻ�Ϊ$(1,1)$�����½�Ϊ$(19,19)$��

���$|x_1-x_2| + |y_1-y_2| = 1$����ô�����$(x_1,y_1)$��$(x_2,y_2)$�����ڵġ����ڵĽ�����Ϸ�����ͬ��ɫ����������ͬһ�����ӡ�һ�����ӵġ����������ڸ��������ڽ��������ڽ������û�����ӵĸ�����һ�����ӵġ����������ڸ����������������ӵġ�������֮�͡�һ�����������������Ϊ�㣬����Ϊ�����塱���ұ�����������Ƴ���

ע�⣬�ں������Ӻ������Ƴ��κ������İ��ӣ�Ȼ�����¼�����ӵġ���������������Ϊ���ܳ���������������������Ӻ󣬺ڰ����������Ӷ�û�С����������Ƴ������İ��ӻ����Ӻ��ӵġ��������������ӵĴ���ʽ���ơ��ڰ������Ӻ������Ƴ��κ������ĺ��ӣ�Ȼ�����¼�����ӵġ���������

������һ��Χ�壬�ӿ����̿�ʼ���ܹ�������$m$��������ÿ�����ӵķ���λ�ã������ÿ���������Ӻ󣬷ֱ��ж��ٿź��ӺͰ��ӱ��Ƴ�����Ȼ�����������������ӣ�������ż�������ӡ���֤���ӷ����ڿյĽ�����ϡ�ע�⣬���ӿ��Է�����$\textbf{����}$��ǰû�����ӵĽ�����ϣ������Ƿ�Υ������ʵ�е�[Χ�����](https://zhuanlan.zhihu.com/p/440794632)$^{(1)}$��

ע�ͣ�
- (2):���߲���

### �����ʽ

������� $m$ �У�$1 \le m \le 5\times 10^5$������ $i$ �а����������� $x_i, y_i$ ��$1 \le x_i, y_i \le 19$������ʾ�� $i$ ���� $(x_i, y_i)$ λ�÷������ӡ�

��֤���ӷ����ڵ�ǰû�����ӵĽ�����ϡ�



### �����ʽ

������� $m$ �У�ÿ�а��������������� $i$ �еĵ�һ��������ʾ�� $i$ �����Ƴ��ĺ����������ڶ���������ʾ���Ƴ��İ���������

�����ߣ�[Immunoglobules](https://www.luogu.com.cn/user/1066251)

```input1
8
2 1
1 1
1 2
2 2
1 1
1 3
2 3
3 1
```

```output1
0 0
0 0
0 1
0 0
0 0
0 0
0 0
3 0
```

## ��ʾ
![](https://cdn.luogu.com.cn/upload/image_hosting/u15z6yt8.png)

