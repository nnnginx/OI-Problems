# AT_ttpc2019_b okyoech

## 题目描述

东京工业大学的全称是 `Tokyo Institute of Technology`，简称为 `Tokyo Tech`。正在该校就读的 rina 想把 AtCoder 比赛排名表过滤，只显示属于东京工业大学的人。然而，由于不同人的机构名称可能是全称、简称或有些微不同，rina 决定采用 `*okyo*ech*` 这一模式进行过滤。由于 rina 正忙于 TTPC2200 的准备工作，她请求路人帮忙编写一个过滤程序。

你需要编写一个程序：给定一个整数 $N$，随后有 $N$ 行，每行是一个表示所属机构的字符串 $S_i$。对于每个字符串 $S_i$，如果它符合 `*okyo*ech*` 模式，输出 `Yes`；否则，输出 `No`。

满足 `*okyo*ech*` 模式的字符串 `T` 指的是，有可能找出字符串 `A`, `B`, `C`，使得 `T` 能被表示为 `A + "okyo" + B + "ech" + C`。这里，`+` 表示字符串连接，且 `A`, `B`, `C` 可以是空字符串。

## 输入格式

输入以下格式提供：

> $ N $  
> $ S_1 $  
> $ \vdots $  
> $ S_N $

## 输出格式

针对每个字符串 $S_i$，在单独的一行中输出相应判断结果，结果之间用换行符分隔。

## 输入输出样例 #1

### 输入 #1

```
1
tokyoinstituteoftechnology
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
8
okyoech
tokyotech
titech
tokyotokyotechtech
tokyotecg
tttoookkkyyyooottteeeccchhh
tokyokogyodaigaku
tokyouniversityofagricultureandtechnology
```

### 输出 #2

```
Yes
Yes
No
Yes
No
No
No
Yes
```

## 说明/提示

### 约束条件

- $ N $ 为满足 $ 1 \leq N \leq 50 $ 的整数。
- $ S_i $ 由小写字母组成。
- $ 1 \leq |S_i| \leq 50 $。

### 示例解释 2

- 请注意，即使所属机构不是东京工业大学，结果也可能为 `Yes`。

 **本翻译由 AI 自动生成**