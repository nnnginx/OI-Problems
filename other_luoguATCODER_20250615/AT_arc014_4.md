# AT_arc014_4 [ARC014D] grepマスター

## 题目描述

高桥君对使用 `grep` 命令很在行。然而，由于很多人也擅长 `grep`，这已不足以证明他的特别之处。为了掌握新的技能，他正在研究 `grep` 命令的手册。

在 `grep` 命令中，有 `-B` 和 `-A` 选项。使用这些选项时，例如：

```sh
grep -B x -A y "needle" kakikomi.txt
```

这行命令会在文件 `kakikomi.txt` 中，不仅显示符合模式 `"needle"` 的行，还会显示该行前面的 `x` 行和后面的 `y` 行。如果文件没有足够的前后行数，就仅显示实际存在的行数。而且，每一行只会被显示一次，即使它被多个命中行所覆盖。关于这个行为，可以参考输出示例。

现在，已知道在某个模式下对文件 `kakikomi.txt` 执行 `grep` 命令后，得到了匹配的行号列表 $L_1, L_2, \ldots, L_n$。现在有 $m$ 个查询，每个查询给定 `x` 和 `y`。对每个查询，求出使用 `-B x -A y` 选项时，将会显示多少行。

### 输入格式

1. 输入的第一行包含三个整数：文件 `kakikomi.txt` 的总行数 $all (1 \leq all \leq 10^9)$，命中行数 $N (1 \leq N \leq \min(all, 10^5))$，以及查询数量 $M (1 \leq M \leq 10^5)$。
2. 接下来有 $N$ 行，每行包含一个整数 $L_i (1 \leq L_i \leq all)$，表示每个命中行的行号。
3. 接下来是 $M$ 行，每行包含两个整数 $x_i, y_i (0 \leq x_i, y_i \leq 10^9)$，表示查询中的 `x` 和 `y`。

### 输出格式

对于每一个查询 $(x, y)$，输出一行，表示使用 `-B x -A y` 选项时，将会显示的行数。在输出的最后要有一个换行符。

### 示例
#### 输入
```
7 2 3
2
4
1 1
3 0
3 4
```

#### 输出
```
5
4
7
```

#### 解释
- 匹配的行是第 2 行和第 4 行。
- 对于第一个查询 $x = 1, y = 1$，命中范围为第 1 到 3 行和第 3 到 5 行，加起来共 5 行。
- 对于第二个查询 $x = 3, y = 0$，命中范围为第 1 到 2 行和第 1 到 4 行，加起来共 4 行。
- 对于第三个查询 $x = 3, y = 4$，命中范围为第 1 到 6 行和第 1 到 7 行，加起来共 7 行。

#### 输入
```
100 5 5
3
18
24
57
90
1 8
27 0
15 16
22 3
2 2
```

#### 输出
```
46
80
98
79
25
```

通过这样的调整和润色，题目描述变得更加简明和易于理解，增强了中文阅读的流畅性。

 **本翻译由 AI 自动生成**

## 输入格式

无

## 输出格式

无