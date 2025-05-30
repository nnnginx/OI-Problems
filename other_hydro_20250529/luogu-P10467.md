## 题目描述
You may have heard that no two snowflakes are alike. Your task is to write a program to determine whether this is really true. Your program will read information about a collection of snowflakes, and search for a pair that may be identical. Each snowflake has six arms. For each snowflake, your program will be provided with a measurement of the length of each of the six arms. Any pair of snowflakes which have the same lengths of corresponding arms should be flagged by your program as possibly identical.

## 输入格式
The first line of input will contain a single integer $n$, $0 < n \le 100000$ , the number of snowflakes to follow. This will be followed by $n$ lines, each describing a snowflake. Each snowflake will be described by a line containing six integers (each integer is at least $0$ and less than $10000000$) , the lengths of the arms of the snow ake. The lengths of the arms will be given in order around the snowflake (either clockwise or counterclockwise), but they may begin with any of the six arms. For example, the same snowflake could be described as $1 2 3 4 5 6$ or $4 3 2 1 6 5$ . 

## 输出格式
If all of the snowflakes are distinct, your program should print the message:

`No two snowflakes are alike.`

If there is a pair of possibly identical snow akes, your program should print the message:

`Twin snowflakes found.`

## 题目大意
**【题目描述】**

你可能听说过没有两片雪花是相同的。你的任务是编写一个程序来确定这是否真的是正确的。你的程序将读取关于一组雪花的信息，并搜索可能相同的一对雪花。每片雪花有六条“角”。对于每片雪花，你的程序将提供每条角的长度测量。任何一对长度对应的角相同的雪花都应该被你的程序标记为可能相同。

**【输入格式】**

输入的第一行包含一个整数 $n$，$0 < n \le 100000$，表示接下来的雪花数量。接下来的 $n$ 行描述每片雪花。每片雪花由包含六个整数的一行描述（每个整数至少为 $0$ 且小于 $10000000$），表示雪花的六条角的长度。角的长度将按顺序围绕着雪花给出（顺时针或逆时针），但它们可以从六个角中的任何一条开始。例如，同一片雪花可以描述为 $1\ 2\ 3\ 4\ 5\ 6$ 或 $4\ 3\ 2\ 1\ 6\ 5$。

**【输出格式】**

如果所有的雪花都是不同的，你的程序应该打印消息：

`No two snowflakes are alike.`

如果有一对可能相同的雪花，你的程序应该打印消息：

`Twin snowflakes found.`

翻译来自于：[ChatGPT](https://chatgpt.com/)

```input1
2 
1 2 3 4 5 6 
4 3 2 1 6 5
```

```output1
Twin snowflakes found.
```

