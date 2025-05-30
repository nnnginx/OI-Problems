### 题目描述

你有一个 $N \times M$ 大的长方形菜园，每个格子代表一块田地。现在你想要检查一下菜园内的田地，于是你决定从右上角出发，在菜园里走一圈回到右上角。最后，所有在你走过的这个环内的田地都被认为检查过了。为了保护植物，你的路径只能在田地边界的小路上走，不能走到田地里面。并且你走过的路径不能自交，小路保证足够宽，你可以多次沿着一条小路走，并且这些路径都不相交。

先在给你菜园的地图，其中有的田地标记为 $I$ ，表示这些田地是你想要检查的；有的田地被标记为 $X$ ，表示这些田地是你不想检查的；有的田地被标记为 $.$ ，表示这些田地你不关心。

假设菜园中有 $K$ 个 $I$ ，那么你要输出 $K$ 个数字，其中第 $i$ 个数为：恰好检查任意 $i$ 个标记为”$I$”的田地，并且没有检查任何一个标记为”$X$”的田地的最短路。

### 输入格式

输入的第一行为 $N$，$M$ 表示田地大小。

接下来 $N$ 行，每行 $M$ 个字母（$I$ ，$X$ 或 $.$ ）描述菜园。

### 输出格式

输出一行，$K$ 个数字用空格隔开，如题目描述中所述。

```input1
2 2
XX
XI
```

```output1
8
```

### 提示

$30\%$ 满足 $K$ = $1$；

$100\%$ 数据满足 $N , M \leq 50$，除了”.”之外的字符最多 $10$ 个。

### 题目来源

2010福建集训

