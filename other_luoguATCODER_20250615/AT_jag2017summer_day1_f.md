# AT_jag2017summer_day1_f 極小部分列

## 题目描述

给出字符串 $s$ 和 $q$ 个查询，每个查询给出一个字符串 $t_i$。

你需要求出：在 $s$ 的最短的包含 $t_i$ 的子串中，最靠左边的那段的左右端点。

## 输入格式

第一行：字符串 $s$，长度不超过 $10^5$。

第二行：询问次数 $q$，不超过 $10^5$。

第三行开始的 $q$ 行：每行一个字符串 $t_i$。

保证：$s$ 和每个 $t_i$ 均由小写英文字母组成，且 $\sum |t_i|\le 10^5$ 。

## 输出格式

对于每个询问，输出一行。

- 若不存在此种子串，输出`-1`；
- 否则，输出两个以单个空格隔开的两个正整数 $l$ 和 $r$，为题目所求。

## 输入输出样例 #1

### 输入 #1

```
aaxbab
12
ab
da
subsequence
aaxbab
a
aa
aaa
aaaa
ba
x
xb
xb
```

### 输出 #1

```
2 4
-1
-1
1 6
1 1
1 2
1 5
-1
4 5
3 3
3 4
3 4
```