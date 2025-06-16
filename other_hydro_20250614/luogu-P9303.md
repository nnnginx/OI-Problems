## ��Ŀ����
In the CCC Word Hunt, words are hidden in a grid of letters. The letters of a hidden word always appear in order on horizontal, vertical, or diagonal line segments in one of two ways.One way is for the letters of a word to appear on one line segment. The other way is for the letters of a word to appear on one line segment up to some letter and then on a second line segment that forms a right angle at this letter.

Given a grid of letters and a single word to search for, your job is to determine the number of times that particular word is hidden in the grid.

## �����ʽ
The first line of input will contain a string of distinct uppercase letters $W$,representing the word you are to search for in the grid. The length of $W$ will be at least two. The second line of input will be an integer $R(1 \le R \le 100)$, where $R$ is the number of rows in the grid.The third line of input will be an integer $C(1 \le C \le 100)$, where $C$ is the number of columns in the grid.

The remaining input will provide the letters in the grid. It will consist of $R$ lines, where each line contains $C$ uppercase letters separated by single spaces.

## �����ʽ
The following table shows how the available 15 marks are distributed:

| Marks | Word Placement |
| :----------: | :---------- |
| $2$ | On one horizontal line segment |
| $2$ | On one horizontal or vertical line segment |
| $2$ | On one horizontal, vertical, or diagonal line segment |
| $9$ | On one line segment or two perpendicular line segments |

The output will consist of a single non-negative integer $H$, representing the number of times the word is hidden in the grid.

## ��Ŀ����
�� CCC Word Hunt �����Ϸ�У�����ÿһ�ض������һ��Ŀ���ַ��� $W$��$2 \leq |W| \leq R + C - 1$����Ȼ������Ҫ��һ�� $R \times C$��$1 \leq R,C \leq 100$���ľ�����Ѱ������ַ����������ҵ�Ŀ���ַ����ķ������ҽ��� $2$ �֣��ֱ�Ϊ��

- ��������ַ�����ˮƽ����ֱ��Խ�б���ų���һ��ֱ�ߡ�

- ��������ַ����Ƚ���һ�Σ�Ȼ��ת $90$ ���ٽ���һ�Ρ�

�������� $R \times C$ �ľ�����һ���������������ַ�����

```input1
MENU
5
7
F T R U B L K
P M N A X C U
A E R C N E O
M N E U A R M
M U N E M N S
```

```output1
3
```

```input2
NATURE
6
9
N A T S F E G Q N
S A I B M R H F A
C F T J C U C L T
K B H U P T A N U
D P R R R J D I R
I E E K M E G B E
```

```output2
4
```

## ��ʾ
**��������������**��

- Subtask $1$��$2$ points���������ַ���һ����һ��ˮƽ�߶��ϡ�
- Subtask $2$��$2$ points���������ַ���һ����һ��ˮƽ��ֱ�߶��ϡ�
- Subtask $3$��$2$ points���������ַ���һ����һ��ˮƽ����ֱ��Խ����߶��ϡ�
- Subtask $4$��$9$ points���������ַ���һ����һ���߶λ��������ഹֱ���߶��ϡ�

���� $1$ ͼ�⣺

![](https://cdn.luogu.com.cn/upload/image_hosting/wqo2un8k.png)

���� $2$ ͼ�⣺

![](https://cdn.luogu.com.cn/upload/image_hosting/v082p2qr.png)

