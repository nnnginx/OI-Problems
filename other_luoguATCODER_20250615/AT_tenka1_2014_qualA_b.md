# AT_tenka1_2014_qualA_b かぶりん！

## 题目描述

“ぶん投げRPG『かぶりん！』”是一款靠投掷包裹的神秘生物かぶりん来击败敌人的动作角色扮演游戏。

国民ダイキ君对かぶりん游戏非常着迷，于是决定写一个程序来计算对敌人造成的伤害。

游戏规则如下：

- 游戏开始时，玩家手中有 $5$ 袋かぶりん。
- 玩家可以投掷手中的かぶりん，造成一定的伤害；投掷后，かぶりん会在一段时间后返回。
- 共有两种投掷方式：「普通投掷」和「蓄力投掷」，每次成功造成伤害后，连击数会增加。

### 普通投掷

- 投掷 $1$ 袋かぶりん。
- 至少需要 $1$ 袋かぶりん。
- 投掷时间 $0.5$ 秒。
- 投掷后 $1$ 秒造成伤害。
- 基础伤害为 $10$，与投掷时的连击数有关。
- 造成伤害后 $5$ 秒かぶりん返回手中。

### 蓄力投掷

- 投掷 $3$ 袋かぶりん。
- 至少需要 $3$ 袋かぶりん。
- 投掷时间 $2.5$ 秒，期间无法进行其他操作。
- 投掷后 $1$ 秒造成伤害。
- 基础伤害为 $50$，与投掷时的连击数有关。
- 造成伤害后 $5$ 秒かぶりん返回手中。

### 连击机制

- 游戏开始时连击数为 $0$。
- 每成功一次投掷攻击，连击数加 $1$。
- 每 $10$ 连击，造成的伤害增加基础伤害的 $10\%$。
- 伤害计算公式为：$A \times (1 + \text{floor}(C / 10) \times 0.1)$，其中 $A$ 是基础伤害，$C$ 是当前连击数。
- 伤害增幅从达成连击后的第一投生效。

### 用户输入

- 每秒钟，用户可以输入一次「普通投掷」、「蓄力投掷」或「无动作」。
- 如果投掷指令时手中没有足够的かぶりん，该指令被忽略。
- 在蓄力期间所有输入被忽略。

根据用户输入，计算对敌人造成的总伤害。注意，包括用户输入结束后，未返回的かぶりん的伤害。

## 输入格式

标准输入包含一行，表示用户输入序列：

> $ S_1\ S_2\ \ldots\ S_n $

- 输入时长为 $n$ 的字符串 ($1 \leq n \leq 1000000$)
- 第 $i$ 个字符 $S_i$ 表示第 $i$ 秒的用户输入
- $S_i$ 可以为：
  - `-` 无动作
  - `N` 普通投掷
  - `C` 蓄力投掷

## 输出格式

输出对敌人造成的总伤害，以一行整数形式给出。需注意，输出需以一个换行结束，确保总伤害不会超过 $10^{11}$。请注意，一般的 32 位整数类型无法存储这么大的数据。

## 输入输出样例 #1

### 输入 #1

```
NNNNNNNN
```

### 输出 #1

```
60
```

## 输入输出样例 #2

### 输入 #2

```
CCCCC
```

### 输出 #2

```
50
```

## 输入输出样例 #3

### 输入 #3

```
NNC------NNC------NNC------NNC------NNC------NNC
```

### 输出 #3

```
439
```

## 说明/提示

### 样例解释 1

尝试进行 $8$ 次普通投掷，其中第 $6$ 和第 $7$ 秒因かぶりん不足未成功，到第 $8$ 秒才因第 $1$ 秒的投掷返还かぶりん，故成功投掷 $6$ 次，造成 $60$ 点伤害。

### 样例解释 2

在第 $1$ 秒开始蓄力投掷，第 $2$ 和第 $3$ 秒的输入因处于蓄力状态被忽略，第 $4$ 和第 $5$ 秒因かぶりん不足而被忽略。

### 样例解释 3

连击导致的伤害增益是在开始投掷前生效的。注意，当连击数达到 $10$ 时，之后的投掷立即享受伤害增益。

 **本翻译由 AI 自动生成**