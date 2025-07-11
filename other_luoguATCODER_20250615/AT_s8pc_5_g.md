# AT_s8pc_5_g Snake Escaping 2

## 题目描述

在 22XX 年，AtCoder 王国遭遇了大量毒蛇的侵袭。国王 chokudai 为了清除这些毒蛇，将所有发现的毒蛇都关进了仓库。然而，三年后，毒蛇又在王国中四处出现。  
在王国的 square 公园，地面上铺有涂着颜色的瓷砖，可以看作是一个 $H$ 行 $W$ 列的网格。毒蛇为了避免再次被捉进仓库，决定通过模仿瓷砖的颜色来逃脱。

今天，有一条毒蛇闯入了公园。它由 $|S|$ 个节段组成，每个节段的颜色可以通过字符串 $S$ 的对应字符获得。$S$ 仅由 `R`、`G` 和 `B` 这些字符组成，分别代表红色、绿色和蓝色。  
毒蛇的相邻节段必须位于网格的上下左右相邻的格子中。

为了帮助毒蛇确保它的「伪装」不被识破，希望你找出瓷砖颜色和毒蛇位置的组合，使得毒蛇能够完美拟态，即每个节段的颜色都与所在格子的瓷砖颜色一致。  
请根据给定的毒蛇颜色，输出可能的瓷砖颜色和毒蛇的位置组合。

## 输入格式

输入由标准输入给出，格式如下：

> $ S $

## 输出格式

输出请遵循以下格式：

> $ H $ $ W $ $ a_{1,1} $ $ a_{1,2} $ ... $ a_{1,W} $ $ a_{2,1} $ $ a_{2,2} $ ... $ a_{2,W} $ : : : $ a_{H,1} $ $ a_{H,2} $ ... $ a_{H,W} $ $ sx $ $ sy $ $ V $

- 第 1 行输出公园网格的高度 $H$ 和宽度 $W$。
- 从第 2 行到第 $H$ 行，输出公园网格的每个位置 $a_{i,j}$ 的颜色。该颜色必须是 `R`、`G` 或 `B`。
- 第 $H+2$ 行输出毒蛇头部的位置 $(sx, sy)$，满足 $1 \leq sx \leq H$ 和 $1 \leq sy \leq W$。
- 第 $H+3$ 行输出毒蛇从第二个节段开始至最后一个节段的移动路径。如果第 $i$ 节段相对第 $i-1$ 节段在左边，则输出 `L`；右边则输出 `R`；下边则输出 `D`；上边则输出 `U`。
- **$H$ 和 $W$ 必须不大于 100。**

## 输入输出样例 #1

### 输入 #1

```
RGB
```

### 输出 #1

```
3 3
RGB
RGB
RGB
1 1
RR
```

## 输入输出样例 #2

### 输入 #2

```
GBRBGBR
```

### 输出 #2

```
4 3
GBR
RGR
RBR
RRR
1 1
RRLDDD
```

## 输入输出样例 #3

### 输入 #3

```
RGBGRGRBRR
```

### 输出 #3

```
3 4
RGBG
BRGR
RRRR
1 1
RRRDLLLRD
```

## 说明/提示

### 制约

- $S$ 由 `R`, `G`, `B` 组成，字符串长度在 1 到 1,000,000 之间。
- **$S$ 是一个随机生成的字符串，其中 `R`, `G`, `B` 出现的概率相等。**

### 子任务

子任务 1 [80 分]

- 满足 $|S| \leq 10,000$。（10 个测试用例）

子任务 2 [320 分]

- 满足 $|S| \leq 15,000$。（20 个测试用例）

子任务 3 [800 分]

- 满足 $|S| = 1,000,000$。（20 个测试用例）

对于子任务 3，得分计算如下：

- 在所有测试中取得的最大值 $max(H, W)$ 记为 $L$。依据 $L$ 值得分：
  - 当 $L \leq 30$ 时，800 分。
  - 当 $31 \leq L \leq 40$ 时，得分为 $1470 - 24L$。
  - 当 $41 \leq L \leq 50$ 时，得分为 $1270 - 19L$。
  - 当 $51 \leq L \leq 100$ 时，得分为 $\lfloor 620 \times 3^{1 - \frac{L}{30}} + 20 \rfloor$。

此外，所有 $30 \leq L \leq 100$ 的得分，可以在 [这个链接](https://drive.google.com/file/d/1Ycjp29PZ0EdbxKb4tVo2uf58jhBGwGF1/view?usp=sharing) 查看。

### 样例解释 1

例如，可以通过下图进行拟态：![ ](https://img.atcoder.jp/s8pc-5/a3a4600450c246a638c6d391c88825e8.png)

### 样例解释 2

例如，可以通过下图进行拟态：![ ](https://img.atcoder.jp/s8pc-5/ef60b421a9ec73374398dfd4c9f04350.png)

 **本翻译由 AI 自动生成**