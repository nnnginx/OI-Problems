## ��Ŀ����
������ [COCI 2017/2018 Contest #2](https://hsin.hr/coci/archive/2017_2018/) T4��San����[ԭ������](https://hsin.hr/coci/archive/2017_2018/contest2_tasks.pdf)��

����ԭ�⣬ʱ������ 1 �룬�ռ����� 64 MB������ 120 �֡�

## ��Ŀ����
Have you ever dreamt that you were the main character in a computer game? The protagonist of this story, Branimir, is having that dream right now.

The world in Branimir's dream consists of $N$ skyscrapers ordered from left to right. For the $i^{th}$ skyscraper, we know the height $H_i$ and the number of gold coins $G_i$ on the roof of the skyscraper. The game begins with a jump on any of the skyscrapers and consists of several steps. In each step, Branimir can jump on a skyscraper to the right from the one he's currently on (it is possible for him to jump over a couple of them too) and if it is not lower than the current one. On each skyscraper roof he's on, Branimir will collect all the gold coins. Branimir can end the game after any number of steps (zero as well), but he must collect at least $K$ gold coins in order to advance to the next level.

Branimir wants to know the number of different ways for him to play the game in order to advance to the next level. Two games are played in different ways if there is a skyscraper that was visited in one game, and not in the other.

## �����ʽ
The first line of input contains positive integers $N(1\leq N \leq 40)$ and $K(1\leq K\leq 4\times 10^{10}$), the numbers from the task.

The $i^{th}$ of the following 
$N$ lines contains two positive integers, $H_i$ and $G_i(1\leq H_i,G_i \leq 10^9$), the numbers from the task.

## �����ʽ
You must output the number of different ways to play the game from the task.

## ��Ŀ����
�� $N$ ��¥���������У��� $i$ ��¥�ĸ߶�Ϊ $H_i$��¥���� $G_i$ ����ҡ�

��ҿ��Դ�����һ��¥��ʼ��ÿһ�����Դӵ�ǰλ�������������ⲻ���ڵ�ǰ¥�ĸ߶ȵ�¥�ϡ�Ȼ����Ի��ÿ��¥�ϵĽ�ҡ�

��ҿ���һֱ����������ʱ������Ϸ������Ҫ��֤��õĽ���� $\geq K$��

������֪�����ж��ٲ�ͬ�ķ�����

---
�����ʽ��

��һ������ $N,K$��

������ $N$ �У�ÿ��������������ʾ $H_i,G_i$��

---
���� $40\%$ �����ݣ��� $N\leq 20$��

```input1
4 6
2 1
6 3
7 2
5 6
```

```output1
3
```

```input2
2 7
4 6
3 5
```

```output2
0
```

```input3
4 15
5 5
5 12
6 10
2 1
```

```output3
4
```

## ��ʾ
#### Explanation for Sample Output 1

The following three games will take Branimir to the next level (the numbers represent the labels of the skyscrapers he visited): {1, 2, 3}, {1, 4} and {4}.

#### Scoring

In test cases worth 40% of total points, it will hold 
$N\leq 20$.

