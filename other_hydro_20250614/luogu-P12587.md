## 题目背景
**请使用 C++17 或 C++20 提交本题**

你需要在程序开头加入如下代码：

```cpp
#include <vector>

void init(std::vector<int> H);

long long query(int S, int E);
```

题目译自 [2019년도 국제정보올림피아드 대표학생 선발고사 - 2차 선발고사](https://www.ioikorea.kr/archives/ioitst/2019/) T3「[외계 선인장](https://assets.ioikorea.kr/ioitst/2019/1/cactus/cactus_statement.pdf)」



## 题目描述
某个外星行星的大部分地表是沙漠，因此降雨非常少。这个星球上的植物都是仙人掌。由于降雨量极少，仙人掌们进化出了互相协作储存水的方法。

行星的某个区域是一个只有上下和左右方向的二维平面。在这个区域内，有 $N$ 棵仙人掌排成一行。每棵仙人掌的宽度都是 $1$ 米，但高度可能不同。为了美化环境，只保留从第 $S$ 棵仙人掌到第 $E$ 棵仙人掌，当降雨量充足时，仙人掌上方的空隙中会积水。如下图所示，下图中箭头指示的范围外的仙人掌可以忽略。

![](https://cdn.luogu.com.cn/upload/image_hosting/3oqf6q0m.png)

你需要根据仙人掌的高度和保留下来的仙人掌范围来计算积水的面积。给定的范围最多有 Q 次。范围始终适用于所有存在的初始仙人掌状态。

你需要实现以下函数：

- `void init(int H[]);`

这个函数只会在程序开始时被调用一次。$H$ 是大小为 $N$ 的数组（向量），按从左到右的顺序存储仙人掌的高度。$N$ 是仙人掌的数量。

- `long long query(int S, int E);`

给定第 $S$ 棵仙人掌到第 $E$ 棵仙人掌的范围 $(1 \leq S \leq E \leq N)$，当降雨量充足时，返回积水的面积。这个函数最多会被调用 $Q$ 次。所有调用都是独立的，即一次调用中移除的仙人掌与其他调用无关。

这些函数必须按照上述描述工作。当然，你可以创建和使用其他函数，但不得进行任何输入输出操作或访问其他文件。

## 输入格式
示例评测程序按以下格式读取输入：

- 第 1 行：$N\, Q$
- 下一行：$N$ 个自然数，按从左到右的顺序表示仙人掌的高度。
- 接下来的 $Q$ 行：每行两个自然数 $S, E (1 \leq S \leq E \leq N)$，表示只保留从第 $S$ 棵仙人掌到第 $E$ 棵仙人掌且下了充足的雨。

## 输出格式
示例评测程序会按行输出你在 `query()` 函数中返回的值。

```input1
10 3
1 3 2 5 1 4 6 2 1 3
2 8
2 4
7 9
```

```output1
6
1
0
```

## 提示
### 样例说明 #1
在上述输入中，你的代码运行方式如下：

| 调用 | 结果 |
| :----------: | :----------: |
|`init({1, 3, 2, 5, 1, 4, 6, 2, 1, 3})`|初始调用|
|`query(2, 8)`|`Query` 调用，返回值 `6`|
|`query(2, 4)`|`Query` 调用，返回值 `1`|
|`query(7, 9)`|`Query` 调用，返回值 `0`|

### 数据范围
对于所有输入数据，满足：

- $1 \leq N \leq 5\cdot 10^5$，$1 \leq Q \leq 5\cdot 10^5$
- 仙人掌的高度在 $1$ 到 $10^{9}$ 之间

详细子任务附加限制及分值如下表所示。

| 子任务 | 分值 | 附加限制 |
| :----------: | :----------: | :----------: |
|$1$|$13$|$1 \leq N \leq 5000$，$1 \leq Q \leq 5000$|
|$2$|$12$|$1 \leq N \leq 5000$|
|$3$|$22$|仙人掌的高度不超过 $20$|
|$4$|$34$|$1 \leq N \leq 10^5$，$1 \leq Q \leq 10^5$|
|$5$|$69$|无附加限制|

