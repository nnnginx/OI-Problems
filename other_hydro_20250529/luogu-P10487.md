## ��Ŀ����
Last night, little erriyue had a horrible nightmare. He dreamed that he and his girl friend were trapped in a big maze separately. More terribly, there are two ghosts in the maze. They will kill the people. Now little erriyue wants to know if he could find his girl friend before the ghosts find them.

You may suppose that little erriyue and his girl friend can move in 4 directions. In each second, little erriyue can move 3 steps and his girl friend can move 1 step. The ghosts are evil, every second they will divide into several parts to occupy the grids within 2 steps to them until they occupy the whole maze. You can suppose that at every second the ghosts divide firstly then the little erriyue and his girl friend start to move, and if little erriyue or his girl friend arrive at a grid with a ghost, they will die.
Note: the new ghosts also can devide as the original ghost.

## �����ʽ
The input starts with an integer T, means the number of test cases.

Each test case starts with a line contains two integers n and m, means the size of the maze. (1<n, m<800)

The next n lines describe the maze. Each line contains m characters. The characters may be:
- ��.�� denotes an empty place, all can walk on.
- ��X�� denotes a wall, only people can��t walk on.
- ��M�� denotes little erriyue
- ��G�� denotes the girl friend.
- ��Z�� denotes the ghosts.

It is guaranteed that will contain exactly one letter M, one letter G and two letters Z.

## �����ʽ
Output a single integer S in one line, denotes erriyue and his girlfriend will meet in the minimum time S if they can meet successfully, or output -1 denotes they failed to meet.

## ��Ŀ����
**����Ŀ������**

����С erriyue ����һ�����µ�ج�Ρ����ε��Լ���Ů���ѱ�����һ�����Թ�������µ��ǣ��Թ�����������ꡣ���ǻ�ɱ�ˡ�����С erriyue ��֪���ڹ���ҵ�����֮ǰ�����Ƿ����ҵ�����Ů���ѡ�

����С erriyue ������Ů���ѿ������ĸ������ƶ�����ÿһ���У�С erriyue �����ƶ� $3$ ����������Ů����ֻ���ƶ� $1$ ���������а��ģ�ÿһ�����Ƕ�����ѳɼ����֣�ռ����������������ڵ�����ֱ������ռ�������Թ�������Լ�����ÿһ���ӣ�������ȷ��ѣ�Ȼ��С erriyue ������Ů���ѿ�ʼ�ƶ������С erriyue ��������Ů���ѵ���һ���й����������Ǿͻ�������

ע�⣺�µĹ��Ҳ������ԭ���Ĺ��һ�����ѡ�

**�������ʽ��**

������һ������ $T$ ��ʼ����ʾ���԰�����������

ÿ�����԰�����һ�п�ͷ�������������� $n$ �� $m$����ʾ�Թ��Ĵ�С��$(1 < n, m < 800)$

�������� $n$ ���������Թ���ÿ�а��� $m$ ���ַ����ַ������ǣ�
- `.` ��ʾ�յأ������˶������ߡ�
- `X` ��ʾǽ��ֻ�������޷����ߡ�
- `M` ��ʾС erriyue��
- `G` ��ʾŮ���ѡ�
- `Z` ��ʾ��ꡣ

��֤�Թ���ǡ����һ����ĸ `M`��һ����ĸ `G` ��������ĸ `Z`��

**�������ʽ��**

��һ�������һ������ $S$����ʾ��������ܳɹ�������С erriyue ������Ů���ѽ������ʱ�� $S$ ��������������� $-1$ ��ʾ����δ��������

���������ڣ�[ChatGPT](https://chatgpt.com/)

```input1
3
5 6
XXXXXX
XZ..ZX
XXXXXX
M.G...
......
5 6
XXXXXX
XZZ..X
XXXXXX
M.....
..G...

10 10
..........
..X.......
..M.X...X.
X.........
.X..X.X.X.
.........X
..XX....X.
X....G...X
...ZX.X...
...Z..X..X
```

```output1
1
1
-1
```

