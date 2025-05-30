## 题目描述
You are trying to schedule a special event on one of five possible days.

Your job is to determine on which day you should schedule the event, so that the largest number of interested people are able to attend.

## 输入格式
The first line of input will contain a positive integer $N$, representing the number of people interested in attending your event. The next $N$ lines will each contain one person's availability using one character for each of Day 1, Day 2, Day 3, Day 4, and Day 5(in that order).

The character `Y` means the person is able to attend and a period (`.`) means the person is
not able to attend.

The following table shows how the available 15 marks are distributed:
| Marks | Description |
| :----------: | :----------: |
| 6 | There will be exactly one day on which every person will be able to attend. |
| 6 | There will be exactly one day on which the largest number of people will be able to attend. |
| 3 | There might be more than one day on which the largest number of people will be able to attend. |


## 输出格式
The output will consist of one line listing the day number(s) on which the largest number of
interested people are able to attend.

If there is more than one day on which the largest number of people are able to attend,output all of these day numbers in increasing order and separated by commas (without spaces).

## 题目大意
你的公司需要开一场会议，一共有 $5$ 天可以开会。这个公司有 $N$ 位员工，每个员工的日程安排都不同，你作为一个公司的董事长，想要听取更多员工的意见，你需要知道哪几天能来开会的员工最多，你准备在这几天中选一天开会。

你需要实现一个程序，第一行输入一个 $N$（$1\leq N \leq 20$），表示有 $N$ 个员工，然后 $N$ 行，每行 $5$ 个字符，`Y` 表示该员工那天能来，`.` 表示不能，现在请你求出哪几天能来开会的员工最多，如果有多天，请以一个 `,` 间隔。

```input1
3
YY.Y.
...Y.
.YYY.
```

```output1
4
```

```input2
5
YY..Y
.YY.Y
.Y.Y.
.YY.Y
Y...Y
```

```output2
2,5
```

## 提示
**本题采用捆绑测试**。

- Subtask $1$（$6$ points）：有且只有一天全部人都可以开会。
- Subtask $2$（$6$ points）：有且只有一天开会人数最多。
- Subtask $3$（$3$ points）：有可能有多天满足条件。


