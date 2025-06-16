# AT_ahc047_a 可爱语言模型

## 题目描述

高桥有 $N$ 个喜欢的字符串。将第 $i$ 个字符串记为 $S_i$，其偏好度为 $P_i$。每个 $S_i$ 仅由 `a` 到 `f` 的小写英文字母组成。

最近，高桥对可以生成字符串的概率模型产生了兴趣。他想设计一个能以高概率生成他喜欢的字符串的**可爱语言模型（LLM）**。

该模型由 $M$ 个状态组成。为每个状态 $i$（$0 \le i \le M$）分配一个由 `a` 到 `f` 中的一个小写字母组成的 $C_i$。此外，对于每对状态 $(i,j)$，定义从状态 $i$ 到状态 $j$ 的转移概率为整数 $A_{i,j}$，表示百分比值。这些值必须满足以下条件：
$$
\sum_{j = 0}^{M - 1}A_{i,j} = 100
$$
模型从状态 $0$ 开始，并在生成长度为 $L$ 的字符串后停止。生成的字符串的第一个字符是分配给状态 $0$ 的字符 $C_0$。然后，模型根据转换概率进行状态转换，依次输出分配给每个新转移状态的字符。

对于每个字符串 $S_i$，如果它在生成的字符串中作为连续子串**出现至少一次**，高桥将获得其对应的偏好度 $P_i$。你的任务是设计字符分配 $C_0,C_1,\ldots,C_{M-1}$ 和转移矩阵 $A$，使得期望总偏好度最大化。

## 输入格式

第一行包含三个整数 $N,M,L$。其中：
* $N$ 是字符串数量，固定 $N = 36$。
* $M$ 是模型中的状态数，固定 $M = 12$。
* $L$ 是生成的字符串的长度，固定 $L = 10^6$。

接下来的输入有 $N$ 行。对于第 $i$（$0 \le i \le N - 1$）行由两个整数 $S_i$ 和 $P_i$ 组成。其中：
* 每个 $S_i$ 是由 `a` 到 `f` 的小写英文字母组成的字符串，且保证其长度满足 $6 \le |S_i| \le 12$。
* 每个偏好度 $P_i$ 是正整数且 $1 \le P_i \le 17000$。
* 所有 $S_i$ 互不相同。

## 输出格式

如果 $C_i$ 是分配给状态 $i$ 的字符，$A_{i,j}$ 是状态 $i$ 到状态 $j$ 的转移概率，则输出由 $M$ 行组成。对于第 $i$（$0 \le i \le M - 1$）行，第一个数为 $C_i$，随后 $M$ 个数为 $A_{i,j}$（$0 \le j \le M - 1$）。其中：

* 每个 $C_i$ 都必须是从 `a` 到 `f` 的小写字母之一。
* 每个 $A_{i,j}$ 必须是满足 $0 \le A_{i,j} \le 100$ 的整数，并且每个 $i$ 必须满足以下条件：

$$
 \sum_{j=0}^{M-1} A_{i,j} = 100 
$$
您的程序可能会输出多个解。如果输出多个解，则只使用最后一个解进行评分。您可以使用网络版的可视化工具比较多个解决方案。

[显示示例](https://img.atcoder.jp/ahc047/cHmFekjC.html?lang=ja&seed=0&output=sample)

## 输入输出样例 #1

### 输入 #1

```
36 12 1000000
acafbafdb 166
baeebdacd 86
baaffdcf 76
cfddcba 251
acdecbbfddaf 12423
ebcebe 107
feddecdb 373
acadbc 40
dcfaabebefcd 15639
fcebaade 438
cbefcedaaf 2468
efcfafcbcaac 4414
dbddcfa 96
cabacbdb 219
cbdeadcbad 3110
bbdeacbbe 894
deafadebdad 7067
dceedaacfefa 6453
deffecdee 280
cfffaaeca 651
aeffcbcfec 1021
ccefdcddadfd 6189
ffcdcb 91
afddebceadc 2283
ffebaff 258
aeceafebd 1235
fbbfec 83
fcdeceffbaf 1787
ddfffeb 188
bebffddaa 238
eedbfbaed 500
cacbccdbd 1346
cafbfbedcff 393
eccbdecdfefa 4423
fdfaddae 522
befebddfe 507
```

### 输出 #1

```
e 66 0 0 0 0 12 0 0 0 0 9 13
e 36 12 0 0 0 0 0 0 0 11 0 41
d 0 20 0 56 0 0 0 0 5 0 19 0
a 0 8 12 79 1 0 0 0 0 0 0 0
f 0 0 0 0 0 0 41 0 0 10 37 12
c 0 0 0 31 0 0 0 53 15 0 1 0
b 0 0 0 0 23 0 65 1 0 0 0 11
f 34 0 8 0 0 0 0 0 0 14 0 44
e 21 0 0 0 10 57 0 0 0 12 0 0
f 0 41 18 0 0 22 0 0 0 0 19 0
a 6 0 0 46 0 0 16 0 0 0 32 0
b 12 0 0 21 24 43 0 0 0 0 0 0
```

## 说明/提示

### 得分

设使用设计的模型生成长度为 $L$ 的字符串时，各字符串 $S_i$ 作为连续子串**出现至少一次**的概率为 $Q_i$。此时得分计算如下：

$\mathrm{round}\left(\sum_{i=0}^{N-1} P_i \cdot Q_i\right)$

共计 150 个测试用例，各测试用例得分之和即为最终得分。若在一个或多个测试用例中出现非法输出或超时，则整个提交将被判定为 `WA` 或 `TLE`。比赛期间获得的最高分将决定最终排名，比赛结束后不进行系统测试。若多名参赛者得分相同，则不论提交时间均视为同一排名。

### 输入生成方法

$ \mathrm{rand}(L,\ U) $：在 $L$ 到 $U$ 范围内均匀随机生成整数值。

#### 字符串 $S_i$ 的生成

各 $S_i$ 的长度 $\ell_i$ 通过 $\ell_i\ =\ \mathrm{rand}(6,\ 12)$ 确定，并按以下步骤生成长度为 $\ell_i$ 的字符串：

- 从字母`a`~`f`中随机选取 $\ell_i$ 次并连接
- 允许同一字母多次出现

若生成的字符串 $S_i$ 与已生成字符串重复，则重新生成长度为 $\ell_i$ 的字符串。

#### 偏好度 $P_i$ 的生成

为每个字符串 $S_i$ 生成对应偏好度 $P_i$：

- 计算最大值 $U_i\ =\ \left\lfloor\ 1.5^{2\ \cdot\ \ell_i}\ \right\rfloor$
- 通过 $P_i\ =\ \mathrm{rand}(1,\ U_i)$ 均匀随机生成

如此独立生成 $N\ =\ 36$ 组 $(S_i,\ P_i)$ 数据。

### 工具（输入生成器/可视化工具）

- [网页版](https://img.atcoder.jp/ahc047/cHmFekjC.html?lang=ja)：比本地版性能更强，支持动画显示
- [本地版](https://img.atcoder.jp/ahc047/cHmFekjC.zip)：需准备[Rust语言](https://www.rust-lang.org/ja)编译环境
  - [Windows预编译二进制文件](https://img.atcoder.jp/ahc047/cHmFekjC_windows.zip)：若配置Rust环境困难可使用此版本

比赛期间禁止共享可视化结果或讨论解法思路，请注意。

By@[shigengxin](https://www.luogu.com.cn/user/1114046)