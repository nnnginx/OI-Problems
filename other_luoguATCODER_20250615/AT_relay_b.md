# AT_relay_b 鏡文

## 题目描述

给出由b、d、p、q四种字符组成的字符串$S$。请判断$S$是不是“镜像字符串”。

这里的“镜像字符串”是指对字符串S进行以下操作后，可得到与原字符串相同的字符串。
1. 反转S。（例："bdpq"=>"qpdb"）
2. 改b为d，改d为b，改p为q，改q为p（不要搞错对应关系）

## 输入格式

标准输入，格式如下：

	S

## 输出格式

如果$S$是镜像字符串，输入"Yes"，否则输出"No"。（不要输出引号）
# 输入输出样例（略）

## 输入输出样例 #1

### 输入 #1

```
pdbq
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
ppqb
```

### 输出 #2

```
No
```

## 说明/提示

## 条件：
- $1≤|S|≤10^5$（$|S|$表示$S$的长度）
- $S$由且仅由b、d、p、q四种字符构成

感谢@std_cpp 提供的翻译