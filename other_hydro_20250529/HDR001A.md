## 题目背景
因为在群里发出“铃有 $114514^{1919810}$ 个金牌”的时候，你没有在 1ms 内赞同，你要用钻石赎罪。

## 题目描述
你没有那么多钻石，所以你用纸糊了一些钻石块准备蒙混过关。

现在你有 $n$ 行的钻石块，第 $i$ 行的钻石块有 $a_i$ 个。

你交差的时候，他说：

“你要赎掉你的 $k$ 个罪！”

因此他拿出了 $k$ 根木棍，代表着你的 $k$ 个罪，你可以将木棍放置到任意一个 $1 \times 1$ 的用纸糊的钻石块上。在你放置的时候，他又说话了：

“你不能让任意两根木棍在同一行或者同一列！”

加了一个要求，你还得硬着头皮干。

所以，你想知道，一共有多少种放置方案？

答案对 $998244353$ 取模。

## 输入格式
第一行一个整数 $n$ 代表有多少行的钻石块。

接下来 $n$ 行每行两个整数 $a_i$ 代表第 $i$ 行的钻石块数量。

第 $n+2$ 行一个整数 $k$ 代表你要放置的木棍数量。

## 输出格式
一行一个整数代表答案对 $998244353$ 取模的结果。

```input1
3
4
3
5
3
```

```output1
27
```

## 说明/提示
#### 样例 1 解释

如下图所示，一共有 $27$ 种方式：

![](./176/file/4o8e1vwj.png)

![](./176/file/gfwmnszi.png)

![](./176/file/n5wut7qs.png)

#### 数据规模与约定

**本题采用捆绑测试。**

- Subtask 1（1 pts）：$k=1$。
- Subtask 2（10 pts）：$n,k \le 5$。
- Subtask 3（25 pts）：$a_i \le a_{i+1}$。
- Subtask 4（10 pts）：$a_i$ 都相等。
- Subtask 5（54 pts）：无特殊限制。

对于 $100\%$ 的数据，$1 \le n,k \le 10^3$，$1 \le a_i \le 10^5$。