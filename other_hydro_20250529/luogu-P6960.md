## 题目背景
这是一道 IO 交互题。

## 题目描述
Ivan wants to play a game with you. He took all integers from $1$ to $n$ inclusive, shuffled them and then put all even numbers into array $e$ and all odd numbers into array $o$ .

Your task is to find arrays $e$ and $o$ .

You can ask Ivan questions of certain kind. Each question consists of two integers $i$ and $j$ . For each question Ivan says whether $e[i] < o[j]$ or not.

You can ask at most $300 000$ questions.

# Interaction Protocol

First, the testing system writes the integer $n (1 \le n \le 10 000)$ -- the number of integers Ivan used.

Your solution shall print requests of two types:

• “? i j”. $1 \le i \le ⌊n/2⌋, 1 \le j \le ⌈n/2⌉$. The testing system responds with the symbol $“<”$ if $e[i] < o[j]$ or with the symbol $“>”$ otherwise.

• “!\ $e_1\ e_2\ \cdots e_{⌊n/2⌋}\ o_1\ o_2 \cdots o_{⌈n/2⌉}$” tells the values of $e$ and $o$ that your program has determined.

Don't forget to flush the output after each request!

Your solution must issue exactly one request of the second type, which must be the last request, and thesolution must terminate gracefully after issuing it.

Your solution is allowed to issue at most $300 000$ requests of the first type.

For each test case the number $n$ is fixed and the numbers are shuffled using Java built-in shuffle functionwith fixed seed.




## 题目大意
有一个长度为 $n(n\le 10000)$ 的排列，所有奇数组成的序列设为 $o$，所有偶数组成的序列设为 $e$。

你可以进行不超过 $300000$ 次询问 `? i j`，每次交互库会返回一个 `<` 或 `>` 表示 $e_i$ 和 $o_j$ 的大小关系，最后你需要求出 $e,o$ 并输出，格式为 `! e o`。

保证数据随机。

```input1
5
>
>
<
>
<
<

```

```output1
? 1 1
? 1 2
? 1 3
? 2 1
? 2 2
? 2 3
! 4 2 1 3 5
```

