## 题目描述
立方填词是一种特殊的填词游戏。填词之前，你需要选择立方体的边长 $a$ ，然后你就可以建立一个有 $a^3$ 个单位立方体的立方体了。这个大立方体有 $12$ 条边。然后，你去掉所有没有接触大立方体边的单位立方体。下图展示了当 $a=6$ 时建立的最终立方体。

![](https://cdn.luogu.com.cn/upload/image_hosting/zzs7dshw.png)

最后，你需要给剩下的每个单位立方体填上一个字母。对于这个立方体，填词之后，每条边上的单词都应该是有意义的。每条边都可以双向阅读，只要从一个方向读起来有意义即可。

下图展示了当 $a=6$ 时的一个立方体。一些单位立方体已经填上了字母。你已经可以沿这个大立方体的三条边读到 **SUBMIT**，**ACCEPT** 和 **TURING** 三个单词了。

![](https://cdn.luogu.com.cn/upload/image_hosting/jzpyzoeu.png)

给定一系列有意义的单词，每个单词可以在合法的立方体的任意一条边上出现。求可以构造多少种不同的立方体对 $998244353$ 取模。

即使一个立方体可以通过旋转和镜像操作变成另一个立方体，也认为这两个立方体**是不同的**。

## 输入格式
第一行一个整数 $n$ ，表示单词的个数。

接下来 $n$ 行，每行一个单词，表示可以在大立方体的边上出现的单词。单词长度大于等于 $3$ ，并且小于等于 $10$ 。

保证所有单词都不同。

## 输出格式
输出一个整数，表示可以构造的不同立方体数对 $998244353$ 取模后的结果。

```input1
1
radar
```

```output1
1
```

```input2
1
robot
```

```output2
2
```

```input3
2
FLOW
WOLF
```

```output3
2
```

```input4
2
baobab
bob
```

```output4
4097
```

```input5
3
TURING
SUBMIT
ACCEPT
```

```output5
162
```

```input6
3
MAN1LA
MAN6OS
AN4NAS
```

```output6
114
```

## 提示
#### 样例解释#1

第一个样例中，唯一一种可能是立方体的所有边上的单词均为 **radar**。

#### 样例解释#2

第二个样例中，有两种立方体，其中一个旋转后可以得到另一个立方体。立方体所有边上的单词都是 **robot**，两个立方体的不同之处在于左下角的字母是 **r** 还是 **t**。

#### 样例解释#3

第三个样例与第二个类似，注意阅读方向不会影响答案。

#### 样例解释#4

第四个样例中，如果把 **bob** 填在立方体的每条边上，有一种立方体。还有 $2^
{12} = 4096$ 种立方体，每条边都填 **baobab**（对于 $12$ 条边中的一条，我们有两种可能的阅读顺序）。

#### 数据范围

对于全部数据， $1 \le n \le 10^5$  。      

详细子任务限制及分值如下表：

| 子任务编号 | 限制 | 分值 |
| :----------: | :----------: | :----------: |
| 1 | 单词中只包含小写的 `a` 到 `f` | $21$ |
| 2 | 单词中只包含小写的 `a` 到 `p` | $29$ |
| 3 | 单词中包含小写的 `a` 到 `p` 和大写的 `A` 到 `P` | $34$ |
| 4 | 单词中包含小写的 `a` 到 `z`，大写的 `A` 到 `Z` 和数字 `0` 到 `9`  | $16$ |

