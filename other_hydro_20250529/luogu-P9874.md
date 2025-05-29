## 题目描述
While most people love to play Wordle these days, Prof. Pang has become addicted to String-dle.

String-dle is an interesting string-guessing game where the player tries to guess a string of $k$ capital letters through several rounds. In each round, the player submits a string of length $k$ as his guess, and the system grades the guess through the following pseudo-code:

```
def grading(answer, guess):
  let count be a hash map
  for i = 1 to k:
    if answer[i] not in count:
      count[answer[i]] = 1
    else:
      count[answer[i]] = count[answer[i]] + 1
  let grade be an array of length k
  for i = 1 to k:
    if answer[i] == guess[i]:
      grade[i] = 'O'
      count[guess[i]] = count[guess[i]] - 1
  for i = 1 to k:
    if answer[i] != guess[i]:
      if count[guess[i]] > 0:
        grade[i] = '-'
        count[guess[i]] = count[guess[i]] - 1
      else:
        grade[i] = 'x'
  return grade
```

The grade consisting of $\tt{O}$ (capital letter O), $\tt{-}$ (dash), and $\tt{x}$ (small letter x) is then returned to the player, and the player may base his next guess on the previous grades. The following is an example of one game Prof. Pang played:

```
G: CRANE
A: xx--x
G: UTTER
A: xxOxx
G: NASAL
A: OOxOO
G: NATAL
A: OOOOO
```

Strings after $\tt{G}$ are Prof. Pang's guesses and strings after $\tt{A}$ are the grades of the guesses. 

Prof. Pang really enjoys the game. He believes that he has developed a perfect strategy for it. However, today he goes mad because he thinks the grading system is bugged! He wants to have someone write an analysis program to figure out the number of possible strings that can be the answer to the puzzle based on his list of guesses and grades.

Since the grading system might be bugged, it might not conform to the pseudo-code given above. So specifically, the task is to find how many strings that are consistent with the input. A string s is consistent with the input if for any guess g in the input and its corresponding grade d, grading(s, g)=d.

And of course, you will be doing the programming.

## 输入格式
The first line consists of two integers $n$ and $k$ $(1 \le n \le 10^4, 1 \le k \le 19)$, which are the number of guesses and the length of the string, respectively.

The following lines consist of the guesses and the grades, one per line, correspondingly.

## 输出格式
An integer, denoting how many possible answers there are, modulo $10^9+7$.

## 题目大意
### 题目描述
当大多数人都沉迷于玩 Wordle 的时候，庞教授却已经沉迷于玩 String-dle 了。

String-dle 是一个有趣的猜字符串的游戏，玩家在玩的时候要通过几轮尝试，猜出一个长度为 $k$ 的字符串。并且在每轮尝试中，玩家要提交一个长度为 $k$ 的字符串来作为他的猜测，而系统通过以下伪代码来为提交的猜测评级：
```
def grading(answer, guess):
  let count be a hash map
  for i = 1 to k:
    if answer[i] not in count:
      count[answer[i]] = 1
    else:
      count[answer[i]] = count[answer[i]] + 1
  let grade be an array of length k
  for i = 1 to k:
    if answer[i] == guess[i]:
      grade[i] = 'O'
      count[guess[i]] = count[guess[i]] - 1
  for i = 1 to k:
    if answer[i] != guess[i]:
      if count[guess[i]] > 0:
        grade[i] = '-'
        count[guess[i]] = count[guess[i]] - 1
      else:
        grade[i] = 'x'
  return grade
```
返回的评级包括 $\tt{O}$（大写字母 O）、$\tt{-}$（破折号）和 $\tt{x}$（小写字母 x），且玩家可以基于先前的评级进行下一次猜测。下面是庞教授玩的一局游戏示例：
```
G: CRANE
A: xx--x
G: UTTER
A: xxOxx
G: NASAL
A: OOxOO
G: NATAL
A: OOOOO
```
在字符串 $\tt{G}$ 后面的是庞教授的猜测，以及在字符串 $\tt{A}$ 后面的是该次猜测的评级。

庞教授非常喜欢这个游戏。他确信他已经知道了这个游戏的完美策略。然而，今天他很生气，因为他认为评级系统出了问题！他想让人写一个分析程序，根据他的猜测与评级找出所有可能的可以作为答案的字符串。

由于评级系统可能出了问题，所以它可能不再符合上面给出的伪代码。具体来说，你需要找到所有符合输入的字符串。一个符合输入的字符串是指，对于输入中任意一个猜测  $g$ 和它的正确评级 $d$，都符合  `grading(s, g)=d`。

当然，你接受了这个任务。

### 输入格式

第一行是两个整数 $n$、$k$ $(1 \le n \le 10^4, 1 \le k \le 19)$，分别是猜测的次数和字符串的长度。

下面共有 $2n$ 行，每两行都对应一个猜测和它对应的评级。

### 输出格式

一个整数，表示有多少种可能的答案，并模 $10^9+7$.

### 样例 #1

#### 样例输入 #1

```
2 5
CRANE
xx--x
NASAL
OOxOO
```

#### 样例输出 #1

```
21
```

### 样例 #2

#### 样例输入 #2

```
1 5
BBBAA
xxxx-
```

#### 样例输出 #2

```
0
```

### 样例 #3

#### 样例输入 #3

```
2 5
ABCDE
-xxxx
ABCDE
xxxxx
```

#### 样例输出 #3

```
0
```

### 样例 #4

#### 样例输入 #4

```
1 3
ABC
---
```

#### 样例输出 #4

```
2
```

### 样例 #5

#### 样例输入 #5

```
1 15
AAAAAAAAAAAAAAB
-xxxxxxxxxxxxxx
```

#### 样例输出 #5

```
918547951
```

## 样例 #6

#### 样例输入 #6

```
1 15
AAAAAAAAAAAAAAA
-xxxxxxxxxxxxxx
```

#### 样例输出 #6

```
0
```

### 样例 #7

#### 样例输入 #7

```
1 1
K
x
```

#### 样例输出 #7

```
25
```

### 提示

对于第二个样例:

如果答案是 $\tt{ACDEF}$，则 $\tt{BBBAA}$ 的评级为 $\tt{xxx-x}$.

```input1
2 5
CRANE
xx--x
NASAL
OOxOO
```

```output1
21
```

```input2
1 5
BBBAA
xxxx-
```

```output2
0
```

```input3
2 5
ABCDE
-xxxx
ABCDE
xxxxx
```

```output3
0
```

```input4
1 3
ABC
---
```

```output4
2
```

```input5
1 15
AAAAAAAAAAAAAAB
-xxxxxxxxxxxxxx
```

```output5
918547951
```

```input6
1 15
AAAAAAAAAAAAAAA
-xxxxxxxxxxxxxx
```

```output6
0
```

```input7
1 1
K
x
```

```output7
25
```

## 提示
For the second example:

If the answer is $\tt{ACDEF}$, the guess $\tt{BBBAA}$ will produce a grade of $\tt{xxx-x}$.

