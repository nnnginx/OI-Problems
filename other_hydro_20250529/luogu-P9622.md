## 题目描述
In 2018, hosted by Nanjing University of Aeronautics and Astronautics (NUAA), the $\textit{International Collegiate Programming Contest}$ (ICPC) regional was held in Nanjing again after a few years' gap. There were over $400$ teams in the contest and team $\textit{Power of Two}$ from Tsinghua University won the champion.

Two years have passed and after the great success in 2018 and 2019, NUAA continues to hold the ICPC Nanjing Regional in 2020. Although we can't gather in Nanjing this time due to the pandemic, we should still be grateful for the hard work done by all staff and volunteers for this contest. Thank you all for your great contribution to this contest!

![](https://cdn.luogu.com.cn/upload/image_hosting/z82ge8hi.png)

In the 2018 contest, problem K, $\textit{Kangaroo Puzzle}$, requires the contestants to construct an operation sequence for the game. Let's first recall the content of that problem:

> The puzzle is a grid with $n$ rows and $m$ columns ($1 \le n, m \le 20$) and there are some (at least $2$) kangaroos standing in the puzzle. The player's goal is to control them to get together. There are some walls in some cells and the kangaroos cannot enter the cells with walls. The other cells are empty. The kangaroos can move from an empty cell to an adjacent empty cell in four directions: up, down, left, and right. It's guaranteed that kangaroos can reach from any empty cell to any other empty cells by going through adjacent empty cells. It is also guaranteed that there is no cycle in the puzzle -- that is, it's impossible that one kangaroo can move from an empty cell, pass by several distinct empty cells, and then back to the original cell.
>
> There is exactly one kangaroo in every empty cell in the beginning and the player can control the kangaroos by pressing the button U, D, L, R on the keyboard. The kangaroos will move simultaneously according to the button you press. For instance, if you press the button R, a kangaroo would move one cell to the right if it exists and is empty, and will stay still if it does not exist or is not empty.
>
> In this problem, the contestant needs to construct an operating sequence of at most $5 \times 10^4$ steps consisting of U, D, L, R only. If after operating these steps in order there are still two kangaroos standing in different cells, the contestant will be given a `Wrong Answer` verdict.

Our dear friend, Kotori, also took part in the contest and submitted a code of randomized algorithm. To her surprise, this simple solution is judged as a correct answer. We now present her solution as follows:

```cpp
#include <bits/stdc++.h>
using namespace std;
string s = "UDLR";
int main()
{
  srand(time(NULL));
  for (int i = 1; i <= 50000; i++) putchar(s[rand() % 4]);
  return 0;
}
```

For contestants who are not familiar with C and C++: the above code will output a random string of length $5 \times 10^4$ consisting only of characters `U`, `D`, `L` and `R`, where each character has equal probability to appear in each position in the string.

Kotori suspects that things might not be that simple for this problem, so right now, in this $\textit{2020 ICPC Nanjing Regional}$ contest, you need to construct an input data to hack her solution. Due to the randomness, your input data only needs to satisfy a successful hacking rate of at least $25\%$. 

Formally speaking, we've prepared $500$ randomly generated strings that each character has equal probability to appear in each position and will use them as the controlling sequence against your answer. For your answer to be accepted, there should be at least $125$ times that after using your answer as the map of cells and the whole controlling sequence is executed, there are still kangaroos in different cells.

Note that your input data should be completely legal. That is to say:

- The map in your answer should not be larger than $20 \times 20$;
- Your answer should contain at least two empty cells;
- All empty cells in your answer should be reachable starting from any empty cell;
- No cycles consisting of empty cells are allowed.

## 输入格式
There is no input for this problem. You're on your own!

## 输出格式
You should first output one line containing two integers $n$ and $m$ ($1 \le n, m \le 20$) separated by a space, indicating the number of rows and columns of the map in your answer.

You should then output $n$ lines where the $i$-th line contains a binary string $s_{i,1}s_{i,2}\cdots s_{i,m}$ ($s_{i,j} \in \{\text{`0'}, \text{`1'}\}$) of length $m$. If $s_{i,j} = \text{`1'}$ then the cell in the $i$-th row and the $j$-th column is empty; Otherwise that corresponding cell contains a wall and cannot be entered.

Note again that your answer only need to achieve a successful hacking rate of at least $25\%$. Not that hard isn't it?

## 题目大意
### 题目描述
2018 年，由南京航空航天大学主办的 $\textit{国际大学生程序设计竞赛}$（ICPC）地区赛时隔数年再次在南京举行。来自清华大学的 $\textit{Power of Two}$ 队获得了冠军。

两年过去了，在 2018 年和 2019 年取得巨大成功后，南京航空航天大学继续在 2020 年举办 ICPC 南京赛区的比赛。虽然这次由于疫情的影响，我们不能齐聚南京，但我们仍然应该感谢所有工作人员和志愿者为这次比赛付出的辛勤劳动。感谢你们为本次比赛做出的巨大贡献！

![](https://cdn.luogu.com.cn/upload/image_hosting/z82ge8hi.png)

在 2018 年的竞赛中 K 题 $\textit{Kangaroo Puzzle}$ 中，要求参赛者为游戏构建一个操作序列。让我们先回顾一下该问题的内容：

> The puzzle is a grid with $n$ rows and $m$ columns ($1 \le n, m \le 20$) and there are some (at least $2$) kangaroos standing in the puzzle. The player's goal is to control them to get together. There are some walls in some cells and the kangaroos cannot enter the cells with walls. The other cells are empty. The kangaroos can move from an empty cell to an adjacent empty cell in four directions: up, down, left, and right. It's guaranteed that kangaroos can reach from any empty cell to any other empty cells by going through adjacent empty cells. It is also guaranteed that there is no cycle in the puzzle -- that is, it's impossible that one kangaroo can move from an empty cell, pass by several distinct empty cells, and then back to the original cell.
>
> There is exactly one kangaroo in every empty cell in the beginning and the player can control the kangaroos by pressing the button U, D, L, R on the keyboard. The kangaroos will move simultaneously according to the button you press. For instance, if you press the button R, a kangaroo would move one cell to the right if it exists and is empty, and will stay still if it does not exist or is not empty.
>
> In this problem, the contestant needs to construct an operating sequence of at most $5 \times 10^4$ steps consisting of U, D, L, R only. If after operating these steps in order there are still two kangaroos standing in different cells, the contestant will be given a ``Wrong Answer'' verdict.

我们的好友 Kotori 也参加了比赛，并提交了随机算法代码。令她惊讶的是，这个简单的解决方案竟然被评为正确答案。现将她的解决方案介绍如下：

```cpp
#include <bits/stdc++.h>
using namespace std;
string s = "UDLR";
int main()
{
  srand(time(NULL));
  for (int i = 1; i <= 50000; i++) putchar(s[rand() % 4]);
  return 0;
}
```

对于不熟悉 C 和 C++ 的参赛者：上述代码将输出一个长度为 $5 \times 10^4$ 的随机字符串，该字符串仅由字符 `U`、`D`、`L` 和 `R` 组成，其中每个字符在字符串中每个位置出现的概率相等。

Kotori 怀疑这个问题可能没那么简单，所以现在，在这个 $\textit{2020 ICPC 南京赛区}$ 竞赛中，你需要构建一个输入数据来破解她的解决方案。由于随机性，你的输入数据只需满足至少 $25\%$ 的 hack 成功率即可。 

从形式上讲，我们准备了 $500$ 个随机生成的字符串，每个字符在每个位置出现的概率相等，并将它们用作对您的答案的控制序列。为了使您的答案被接受，在使用您的答案作为单元格映射并执行整个控制序列后，至少应该有 $125$ 个的不同单元格中有袋鼠。

请注意，您的输入数据必须完全合法。也就是说:

- 答案中的地图不应大于 $20 × 20$；
- 您的答案应至少包含两个空单元格；
- 答案中的所有空单元格都应可以从任意空单元格出发到达；
- 不允许包含空单元格的环（也就是说，空单元格组成一棵树）。

```input1
(No input)
```

```output1
3 4
1111
1010
1100

```

## 提示
### Note
The sample output we provide you is (obviously) incorrect. It only serves the purpose of showing you the output format. This is a $3 \times 4$ map with $4$ walls, so there will be $8$ kangaroos in the empty cells at the beginning.

