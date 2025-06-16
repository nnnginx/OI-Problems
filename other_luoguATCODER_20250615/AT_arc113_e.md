# AT_arc113_e [ARC113E] Rvom and Rsrev

## 题目描述

给定只由$a$,$b$组成的一个字符串$S$，你可以做以下操作任意次，使最终的字符串字典序最大。

- 选择$S$的两个相同的字符，将它们之间的字符串翻转，并删掉所选择的两个字符。

比如在$S$中选择两个位置$i,j(s_i=s_j,i<j)$，你可以将字符串$S$替换为$s_1\dots s_{i-1}s_{j-1}s_{j-2}\dots s_{i+2}s_{i+1}s_{j+1}s_{j+2}\dots s_{|S|}$

有$T$组数据

## 输入格式

第一行一个整数$T$.
接下来$T$行，每行一个字符串$S$.

## 输出格式

$T$行，一行一个字符串，对每一组测试数据，输出字典序最大的字符串。

## 输入输出样例 #1

### 输入 #1

```
20
abbaa
babbb
aabbabaa
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbabaaaaabbaababaaabbabbbbbaaaaa
babbbaaaabaababbbabaabaaaaababaa
bbaababababbbaaabaabababaabbabab
abaabbabaabaaaaabaaaabbaabaaaaab
aabababbabbabbabbaaaabbabbbabaab
aabababbabbbbaaaabbaaaaabbaaaabb
abbbbaabaaabababaaaababababbaabb
aaaaaaaaaaaaaaaaaaaaaaabbbbbbbbb
aaaaaaaaaabbbbbbbbbbbbbbbbbbbbbb
abababaaababaaabbbbbaaaaaaabbbbb
aabbaaaaababaabbbbbbbbbaabaaabbb
babababbababbbababbbbbababbbabbb
bbbbababbababbbabababbabbabbbbbb
aaaaaaaaaaaaaaaaababababbbabbbbb
aabababbabbabababababababbbbabbb
```

### 输出 #1

```
bba
bba
bbba
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbaaaaaaaa
bbbbbbbbbbbbbaaaaaaa
bbbbbbbbbbbbbbbb
bbbbbbbbbb
bbbbbbbbbbbbbbbbab
bbbbbbbbbbbbbb
bbbbbbbbbbbbbabb
abbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbaaaaaaaaa
bbbbbbbbbbbbbbbaaaaa
bbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbba
bbbbbbbbbaaaaaaaaaaaaaaa
bbbbbbbbbbbbbbbbba
```

## 说明/提示

$
1\le T\le 2\times 10^5\\
1\le |S_i|(i=1,2\dots ,T)\\
1\le |S_1|+|S_2|+\dots +|S_T|\le 2\times 10^5
$