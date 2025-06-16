## 题目背景
本题翻译自 [2021년도 국제정보올림피아드 대표학생 선발고사](https://www.ioikorea.or.kr/archives/ioitst/2021/) 1차 선발고사 [#1 카드 뒤집기 게임](https://assets.ioikorea.or.kr/ioitst/2021/1/card/card_statement.pdf)。

**请注意，你不需要也不应该实现 `main` 函数。具体实现方式见【实现细节】部分。**

## 题目描述
翻牌游戏是一种单人卡牌游戏，使用两种类型的卡牌 A 和 B。卡牌 A 上写有游戏规则的相关信息。具体来说，如图 1 所示，卡牌 A 上写有两个整数 $N$ 和 $M$（$M \leq N$），以及一个大小为 $N \times N$ 的由字符 `O` 和 `X` 组成的图案 $P$。

![图 1](https://cdn.luogu.com.cn/upload/image_hosting/mzniv9wh.png)

卡牌 B 的正面写有字符 `O`，背面写有字符 `X`。每张卡牌 B 代表卡牌 A 上的图案中的一个字符，为此准备了足够多的卡牌 B。

游戏开始时，首先选择一张卡牌 A，并根据其上的 $N$ 值将卡牌 B 排列成 $N \times N$ 的网格。初始时所有卡牌都显示 `X`。每个卡牌的位置用行号和列号标记，如图 2 所示。

![图 2](https://cdn.luogu.com.cn/upload/image_hosting/pxh8ehfd.png)

初始排列完成后，玩家可以重复进行如下**翻牌**操作。每次翻牌由两个步骤组成：

- **步骤 1**：在 $N \times N$ 网格中选择任意一行或一列，并根据卡牌 A 上的整数 $M$ 选择一个任意的整数 $k$（$0 \leq k < M$）。
- **步骤 2**：
   - 如果选择的是行 $i$，则对于所有满足 $j \equiv k \pmod M$ 的列 $j$，翻转位置 $(i, j)$ 上的卡牌。
   - 如果选择的是列 $j$，则对于所有满足 $i \equiv k \pmod M$ 的行 $i$，翻转位置 $(i, j)$ 上的卡牌。

玩家的目标是通过重复翻牌操作，使网格中的卡牌图案与卡牌 A 上的图案 $P$ 完全一致。请判断这是否可能实现。

### 实现细节

你需要实现以下函数：

```cpp
bool reversal(int N, int M, vector<string> P)
```

- 该函数仅被调用一次。
- 参数 $N$ 表示网格的大小。
- 参数 $M$ 表示翻牌操作中卡牌的间隔。
- 参数 $P$ 是一个包含 $N$ 个字符串的数组，每个字符串长度为 $N$，$P[i]$ 表示目标图案的第 $i$ 行。
- 如果通过翻牌操作可以从初始排列得到图案 $P$，则返回 `true`，否则返回 `false`。


## 输入格式
示例评测程序的输入格式如下：

- 第 $1$ 行：$N \ M$
- 第 $2$ 行到第 $2 + i$ 行：$P[i]$

注意：示例评测程序可能与实际评测程序不同。


## 输出格式
示例评测程序的输出格式如下：

- 第 $1$ 行：一个字符 `0` 或 `1`，分别表示 `false` 或者 `true`

```input1
5 2
XXXOX
XXXOX
OOOXO
XOXXX
XOXXX
```

```output1
1
```

## 提示
### 约束条件

- $1 \leq M \leq N \leq 1\,000$
- $P$ 中的所有字符为 `O` 或 `X`。

### 子任务

1. （$11$ 分）
   - $N \times M \leq 10$
2. （$50$ 分）
   - $M = 1$
3. （$39$ 分）
   - 无额外约束。

### 评分标准

每个子任务的得分是该子任务所有测试点得分的最小值。

### 示例

- $N = 5$, $M = 2$，图案 $P = [\texttt{XXXXX}, \texttt{XXXXX}, \texttt{OOOXO}, \texttt{XOXXX}, \texttt{XOXXX}]$ 时，评测程序将调用：

  ```cpp
  reversal(5, 2, ["XXXXX", "XXXXX", "OOOXO", "XOXXX", "XOXXX"])
  ```

  下图展示了从初始状态开始，通过翻牌操作，根据选择的行或列号和 $k$ 值，卡牌图案的变化过程。最终形成了图案 $P$。因此，调用的 `reversal` 函数应返回 `true`。

  ![](https://cdn.luogu.com.cn/upload/image_hosting/mzniv9wh.png)

