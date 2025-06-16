# AT_rco_contest_2018_final_b くるくる寿司

## 题目描述

这是一道交互题。当给出整数 $N$ 时，你需要选择一个长度为 $N$ 的字符串 $S$ 和一个实数 $D$。裁判根据 $S$ 和 $D$ 生成 $Q$ 个查询 $q_i$。对于每个查询，裁判会在 $0$ 到 $N-1$ 的整数中随机选择一个起始点 $start_i$。字符串 $q_i$ 根据如下伪代码生成：

> $ q_i\ =\ "" $  
for (pos = $ start_i $; $ q_i $.length < M; pos++)  
以概率 $ 1.0\ /\ D $ 将 $ S[pos\ \%\ N] $ 添加到 $ q_i $ 的末尾  
return $ q_i $

你需要估计每个 $start_i$。

每个测试用例的得分以及本问题的总得分按以下方式计算：

- 对于每个 $i$，估计值 $guess_i$ 和实际值 $start_i$ 的距离定义为：
  \[
  distance_i = \min\left(\left| guess_i - start_i \right|, N - \left| guess_i - start_i \right|\right)
  \]
- 得分使用以下公式计算：
  \[
  score_i = \sqrt{D} \times \exp(-distance_i^2 / 25.0)
  \]
- 函数 $ y = \exp(-x^2 / 25) $ 产生的图形如下：
  ![y=exp(-x^2/25)](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_rco_contest_2018_final_b/efdd44afc41673f26dfaed4842e288d6dcbceccb.png)
- 每个测试用例的得分为所有 $i$ 的分数总和，并向上取整。
- 一共包含10个测试用例，得分为各测试用例得分之和。
- 请注意，评分计算使用64位浮点数，因此可能存在微小的误差。

### 输入格式

输入将以如下格式从标准输入提供：

首先，输入以下内容：

> $ N $ $ M $ $ Q $

- $ N $ 为字符串 $ S $ 的长度，$ N = 3000 $。
- $ M $ 为 $ q_i $ 的长度，$ M = 7 $。
- $ Q $ 是查询的数量，$ Q = 30000 $。

基于该输入，你需要输出 $ S $ 和 $ D$，格式如下：

> $ S $ $ D $

- $ S $ 为长度为 $ N $ 的字符串，由小写字母组成。
- $ D $ 是一个在 $ 1.0 $ 至 $ 10.0 $ 之间的实数。

接收以下输入：

> $ q_0 $ $ q_1 $ ... $ q_{Q-1} $

- 每个 $ q_i $ 是长度为 $ M $ 的字符串。

针对每个 $ q_i $，输出 $ guess_i$，格式如下：

> $ guess_0 $ $ guess_1 $ ... $ guess_{Q-1} $

- $ guess_i $ 是一个在 $ 0 \leq guess_i < N $ 范围内的整数。

- 完成输出后，立即结束程序。
- 每次输出后请确保换行并刷新输出缓冲区。
- 因判题程序要求，必须在读取完所有 $ q_i $ 后再开始输出 $ guess_i $。

### 示例

**输入：**
```
13 7 2
```

通知：此处提供的 $ N = 13, M = 7, Q = 2 $ 仅为示例，不符合题目中实际测试用例的约束条件。

**输出：**
```
nosushinolife
1.8
```

输出表示选取的 $ S=\text{"nosushinolife"} $ 和 $ D=1.8 $，其中 $ S $ 长��为 $ N=13 $。

**输入：**
```
osushin
nolifos
```

系统生成并提供的 $ q_0, q_1 $，每个长度为 $ M=7 $。

**输出：**
```
1
7
```

对于给定 $ start_0=1 $ 和 $ start_1=0 $，计算分数如下：

- $ distance_0 = \min(\left| 1 - 1 \right|, 13 - \left| 1 - 1 \right|) = 0 $，
- $ score_0 = \sqrt{1.8} \times \exp(-0^2 / 25.0) \approx 1.341641 $，
- $ distance_1 = \min(\left| 7 - 0 \right|, 13 - \left| 7 - 0 \right|) = 6 $，
- $ score_1 = \sqrt{1.8} \times \exp(-6^2 / 25.0) \approx 0.317872 $。

因此，本示例中的总得分是 $ score_0 + score_1 \approx 1.659513 $，向上取整后结果为 $ 2 $ 分。

### 测试器

测试器可以通过以下链接获取：

[测试器](https://github.com/recruit-communications/rco-contest-2018/tree/master/final_B/tester)

 **本翻译由 AI 自动生成**

## 输入格式

无

## 输出格式

无