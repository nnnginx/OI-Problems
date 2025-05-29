## ��Ŀ����
Those tiny music machines that play your digital music are really computers that keep track of and play music files. The CCC music player $(C^3MP)$ is currently in development and will be hitting the stores soon! In this problem, you have to simulate a $C^3MP$.

The $C^3MP$ music player will hold $5$ songs in memory, whose titles will always be `A`, `B`, `C`, `D`, `E`. The $C^3MP$ also keeps track of a playlist, which is an ordering of all the songs. The $C^3MP$ has 4 buttons that the user will press to rearrange the playlist and play the songs.

Initially, the $C^3MP$ playist is `A,B,C,D,E`. The $4$ control buttons do the following:

- button $1$: move the first song of the playlist to the end of the playlist. For example: `A,B,C,D,E` will change to `B,C,D,E,A`.

- button $2$: move the last song of the playlist to the start of the playlist. For example, `A,B,C,D,E` will change to `E,A,B,C,D`.

- button $3$: swap the first two songs of the playlist. For example, `A,B,C,D,E` will change to `B,A,C,D,E`.

- button $4$: stop rearranging songs and output the playlist.

## �����ʽ
You need to write a program to simulate a CCC music player. Your program should repeatedly ask for two positive integers b and n. Here b represents the button number that the user wants to press, $1 \leq b \leq 4$, and n represents the number of times that the user wants to press button b. You can assume that n always satisfies $1 \leq n \leq 10$.

## �����ʽ
The input will always finish with the pair of inputs $(b = 4, n = 1)$ when this happens, you should print the order of songs in the current playlist and your program should end. You can assume that the user will only ever press button $4$ once.

## ��Ŀ����
����һ����������ַ����ַ����飬���ַ������ʼֵΪ $\{\text{A,B,C,D,E}\}$��ÿ�β����������붼�������� $b(1 \leq b \leq 4)$ �� $n(1 \leq n \leq 10)$������Ҫ���� $b$ ��ֵ���в�����

- $b = 1$ ���������ǰ���һ���ַ��Ƶ�ĩβȥ��ִ�� $n$ �Ρ�

- $b = 2$ ���������ĩβ�ַ��Ƶ���λȥ��ִ�� $n$ �Ρ�

- $b = 3$ �����������ǰ $2$ ���ַ���λ�ã�ִ�� $n$ �Ρ�

- $b = 4$ ������������ǰ���ַ����飨ÿ���ַ��ÿո������������ֹ����

```input1
2
1
3
1
2
3
4
1
```

```output1
B C D A E
```

