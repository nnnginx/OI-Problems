## 题目描述
Those tiny music machines that play your digital music are really computers that keep track of and play music files. The CCC music player $(C^3MP)$ is currently in development and will be hitting the stores soon! In this problem, you have to simulate a $C^3MP$.

The $C^3MP$ music player will hold $5$ songs in memory, whose titles will always be `A`, `B`, `C`, `D`, `E`. The $C^3MP$ also keeps track of a playlist, which is an ordering of all the songs. The $C^3MP$ has 4 buttons that the user will press to rearrange the playlist and play the songs.

Initially, the $C^3MP$ playist is `A,B,C,D,E`. The $4$ control buttons do the following:

- button $1$: move the first song of the playlist to the end of the playlist. For example: `A,B,C,D,E` will change to `B,C,D,E,A`.

- button $2$: move the last song of the playlist to the start of the playlist. For example, `A,B,C,D,E` will change to `E,A,B,C,D`.

- button $3$: swap the first two songs of the playlist. For example, `A,B,C,D,E` will change to `B,A,C,D,E`.

- button $4$: stop rearranging songs and output the playlist.

## 输入格式
You need to write a program to simulate a CCC music player. Your program should repeatedly ask for two positive integers b and n. Here b represents the button number that the user wants to press, $1 \leq b \leq 4$, and n represents the number of times that the user wants to press button b. You can assume that n always satisfies $1 \leq n \leq 10$.

## 输出格式
The input will always finish with the pair of inputs $(b = 4, n = 1)$ when this happens, you should print the order of songs in the current playlist and your program should end. You can assume that the user will only ever press button $4$ once.

## 题目大意
你有一个含有五个字符的字符数组，该字符数组初始值为 $\{\text{A,B,C,D,E}\}$，每次操作数据输入都是两个数 $b(1 \leq b \leq 4)$ 和 $n(1 \leq n \leq 10)$，你需要根据 $b$ 的值进行操作：

- $b = 1$ 的情况：将前面第一个字符移到末尾去，执行 $n$ 次。

- $b = 2$ 的情况：将末尾字符移到首位去，执行 $n$ 次。

- $b = 3$ 的情况：交换前 $2$ 个字符的位置，执行 $n$ 次。

- $b = 4$ 的情况：输出当前的字符数组（每个字符用空格隔开），并终止程序。

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

