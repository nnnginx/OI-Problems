## 题目背景
小 L 很喜欢树，很喜欢 $ \operatorname{LCA} $，很喜欢有序元组，于是有了这样一道题。

## 题目描述
对于一棵 $ n $ 点有根树（根为 $ 1 $），定义有序 $ p $ 元组 $ (a_1,a_2,......,a_p) $ 为 $ k $ 级 $ \operatorname{LCA} $ $ p $ 元组当且仅当：

* $ 1 \le a_1<a_2<......<a_p \le n $

* 存在 $ x $ 使得对于任意有序严格递增 $ k $ 元组 $ b \subseteq a $ 均满足 $ \operatorname{LCA}_{i=1}^{k}\{b_i\} = x $。

注意，$ \operatorname{LCA}(x,y) $ 指树上 $ x $ 点和 $ y $ 点的最近公共祖先，且 $ \operatorname{LCA}_{i=1}^{k}\{b_i\} $ 指的是所有的 $ b_i $ 的 $ \operatorname{LCA} $。

求出 $ k $ 级 $ \operatorname{LCA} $ $ p $ 元组的个数，对 $ 10^9+7 $ 取模。

## 输入格式
第一行一个整数 $ n,p,k $。

接下来 $ n-1 $ 行，每行两个整数代表一条边的两个端点的编号。

## 输出格式
输出一个整数代表要求的答案。

```input1
6 4 3
1 2
2 3
3 4
3 5
3 6
```

```output1
1
```

```input2
6 3 2
1 2
1 3
1 4
1 5
1 6
```

```output2
20
```

```input3
6 4 2
1 2
1 3
2 4
2 5
3 6
```

```output3
0
```

## 提示
**【样例 1 解释】**

对于样例 $ 1 $，我们发现符合要求的 $ 4 $ 元组只有 $ (3,4,5,6) $。

**【数据规模与约定】**

对于 $ 100\% $ 的数据，$ 2 \le n \le 5000 $，$ 2 \le k \le p \le n $。

**提示：本题开启捆绑测试。**

* Subtask 1（10 pts）：$ n \le 10 $。
* Subtask 2（20 pts）：$ n \le 20 $。
* Subtask 3（30 pts）：$ n \le 500 $。
* Subtask 4（10 pts）：$ 1 $ 和所有点存在直接连边。
* Subtask 5（30 pts）：无特殊限制。

**【贡献名单】**

data&check：EstasTonne。（主题库里这个题下一个题号的出题人）

