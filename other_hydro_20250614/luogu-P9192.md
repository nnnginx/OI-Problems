## 题目描述
Pareidolia is the phenomenon where your eyes tend to see familiar patterns in images where none really exist -- for example seeing a face in a cloud. As you might imagine, with Farmer John's constant proximity to cows, he often sees cow-related patterns in everyday objects. For example, if he looks at the string `bqessiyexbesszieb`, Farmer John's eyes ignore some of the letters and all he sees is `bessiebessie`.

Given a string $s$, let $B(s)$ represent the maximum number of repeated copies of `bessie` one can form by deleting zero or more of the characters from $s$. In the example above, $B(bqessiyexbesszieb)=2$. Furthermore, given a string $t$, let $A(t)$ represent the sum of $B(s)$ over all contiguous substrings $s$ of $t$.

Farmer John has a string t of length at most $2\times10^5$ consisting only of characters a-z. Please compute A(t), and how A(t) would change after $U (1\le U\le2\times10^5)$ updates, each changing a character of t. Updates are cumulative.

## 输入格式
The first line of input contains $t$.

The next line contains $U$, followed by $U$ lines each containing a position $p$ $(1\le p\le N)$ and a character $c$ in the range a-z, meaning that the pth character of $t$ is changed to $c$.

## 输出格式
Output $U+1$ lines, the total number of bessies that can be made across all substrings of $t$ before any updates and after each update.

## 题目大意
### 题目描述

Pareidolia 是一种现象，指的是人们倾向于在并不真正存在的地方看到熟悉的图案——例如在云中看到一张脸。可以想象，由于农夫 John 经常与奶牛接触，他常常在日常物品中看到与奶牛相关的图案。例如，如果他看到字符串 `bqessiyexbesszieb`，农夫 John 的眼睛会忽略其中的一些字母，而他看到的只是 `bessiebessie`。

给定一个字符串 $s$，令 $B(s)$ 表示通过删除 $s$ 中的零个或多个字符后，能够形成的 `bessie` 的最大重复次数。在上面的例子中，$B(bqessiyexbesszieb)=2$。此外，给定一个字符串 $t$，令 $A(t)$ 表示所有连续子串 $s$ 的 $B(s)$ 之和。

农夫 John 有一个长度不超过 $2 \times 10^5$ 的字符串 $t$，且仅由字符 a-z 组成。请计算 $A(t)$，以及在 $U (1 \le U \le 2 \times 10^5)$ 次更新后 $A(t)$ 的变化情况，每次更新会修改 $t$ 中的一个字符。更新是累积的。

### 输入格式

第一行输入包含 $t$。

接下来的一行包含 $U$，随后是 $U$ 行，每行包含一个位置 $p$ $(1 \le p \le N)$ 和一个字符 $c$（范围为 a-z），表示将 $t$ 的第 $p$ 个字符修改为 $c$。

### 输出格式

输出 $U+1$ 行，分别表示在没有任何更新之前以及每次更新后，$t$ 的所有子串中能够形成的 `bessie` 的总数。

### 提示

在没有任何更新之前，有 12 个子串恰好包含 $1$ 个 `bessie`，有 $1$ 个子串恰好包含 $2$ 个 `bessie`，因此 `bessie` 的总数为 $12 \cdot 1 + 1 \cdot 2 = 14$。

第一次更新后，$t$ 变为 `belsiebessie`。有 7 个子串恰好包含一个 `bessie`。

第二次更新后，$t$ 变为 `belsiesessie`。只有整个字符串包含 `bessie`。

输入 $2$：$|t|, U \le 300$；

输入 $3-5$：$U \le 10$；

输入 $6-13$：$|t|, U \le 10^5$；

输入 $14-21$：没有额外限制。

```input1
bessiebessie
3
3 l
7 s
3 s
```

```output1
14
7
1
7
```

## 提示
Before any updates, twelve substrings contain exactly $1$ `bessie` and $1$ string contains exactly $2$ `bessie`s, so the total number of bessies is $12⋅1+1⋅2=14$.

After one update, $t$ is `belsiebessie`. Seven substrings contain exactly one `bessie`.

After two updates, $t$ is `belsiesessie`. Only the entire string contains `bessie`.


Input $2$: $|t|,U\le300$;

Inputs $3-5$: $U\le10$;

Inputs $6-13$: $|t|,U\le10^5$;

Inputs $14-21$: No additional constraints.

