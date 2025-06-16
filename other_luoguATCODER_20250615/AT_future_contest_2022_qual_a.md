# AT_future_contest_2022_qual_a Project Leader

## 题目描述

有 $N$ 个任务需要分配给 $M$ 名团队成员。每个任务最多分配给一名成员，并且成员在一个任务完成前不能接新任务。共有 $K$ 种技能，每个成员 $j$ 的技能水平是一个非负整数向量 $\bm{s_j} = (s_{j,1}, \cdots, s_{j,K})$，每个任务 $i$ 的要求是另一个非负整数向量 $\bm{d_i} = (d_{i,1}, \cdots, d_{i,K})$。成员技能水平 $\bm{s_1}, \cdots, \bm{s_M}$ 不会作为输入给出。

定义 $w_{i,j} := \sum_{k=1}^K \max(0, d_{i,k} - s_{j,k})$。如果成员 $j$ 被分配了任务 $i$，则任务完成时间 $t_{i,j}$ 计算如下：

1. 若 $w_{i,j} = 0$，则 $t_{i,j} = 1$。
2. 若 $w_{i,j} > 0$，则 $t_{i,j} = \max(1, w_{i,j} + r_i)$，其中 $r_i$ 是 -3 到 3 的随机整数。

任务如果在第 $d$ 天启动，预计用时 $t$ 天，则在第 $d + t - 1$ 天结束。任务间的依赖要求某任务必须完成后，依赖于该任务的任务才能开始。目标是在最短的时间内完成所有任务。

### 输入格式

标准输入提供任务数 $N$、成员数 $M$、技能种类 $K$、依赖数 $R$、每个任务的技能需求 $\bm{d_1}, \cdots, \bm{d_N}$ 及依赖关系 $(u_1, v_1), \cdots, (u_R, v_R)：

> $N$ $M$ $K$ $R$  
> $d_{1,1} \cdots d_{1,K}$  
> $\vdots$  
> $d_{N,1} \cdots d_{N,K}$  
> $u_1$ $v_1$  
> $\vdots$  
> $u_R$ $v_R$

依赖关系 $(u_i, v_i)$ 代表任务 $v_i$ 在任务 $u_i$ 完成前无法启动。保证 $u_i < v_i$，且每对 $(u_i, v_i)$ 在输入中独立出现。

每天需完成以下步骤：

1. 提供当天分配的任务：输出在第 $a_i$ 名成员负责第 $b_i$ 个任务的列表 $(a_1, b_1), \cdots, (a_m, b_m)$，格式为：

> $m$ $a_1$ $b_1$ $\cdots$ $a_m$ $b_m$

**注意：输出后必须刷新标准输出**，否则可能超时。

2. 当天的结束时，会输入任务完成的成员列表 $f_1, \cdots, f_n$：

> $n$ $f_1$ $\cdots$ $f_n$

当所有任务完成或到达第 2000 天时，输入 `-1` 表示程序应终止。

### 输出格式

根据描述逐日输出各成员及其任务列表。

### 数据范围与提示

#### 得分
- 在第 $D$ 天结束（$1 \leq D \leq 2000$）完成所有任务，得分为 $N + 2000 - D$。
- 若在 2000 天内未完成任务，得分为完成的任务数 $T$（$T < N$）。

#### 测试用例
- 暂定测试数：50 个
- 系统测试数：3000 个，比赛后公开 [seeds.txt](https://img.atcoder.jp/future-contest-2022-qual/seeds.txt) 

提交的最终得分是所有测试用例得分之和。暂定测试中，如有错误输出或超时，整体提交判定为失败。系统测试中错误仅影响该测试用例。注意程序异常退出可能记为错误判定。

#### 运行时间
运行时间有浮动，系统测试中会稍长。临界运行时间的程序可能在系统测试中超时，建议程序计时并提前终止或性能优化。

#### 输入生成方法
随机生成函数如下：
- $\mathrm{randint}(L, U)$：生成 $L$ 到 $U$ 的整数。
- $\mathrm{randdouble}(L, U)$：生成 $L$ 到 $U$ 的浮点数。
- $\mathrm{randnormal}()$：从标准正态分布生成数值。

#### $N$、$M$、$K$、$R$ 的生成
- 固定 $N = 1000$
- 固定 $M = 20$
- 随机 $K = \mathrm{randint}(10, 20)$
- 随机 $R = \mathrm{randint}(1000, 3000)$

#### $d_{i,j}$ 的生成
针对每个 $i = 1, \cdots, N$，生成 $\bm{d_i} = (d_{i,1}, \cdots, d_{i,K})$：

1. 生成 $(d'_{i,1}, \cdots, d'_{i,K})$，其中 $d'_{i,j} = |\mathrm{randnormal}()|$。
2. 计算 $p_i = \frac{\mathrm{randdouble}(10, 40)}{\sqrt{\sum_{j=1}^K d'_{i,j}^2}}$。
3. 生成 $d_{i,j} = \mathrm{round}(p_i \cdot d'_{i,j})$。

#### $s_{i,j}$ 的生成
对每个 $i = 1, \cdots, M$，生成 $\bm{s_i} = (s_{i,1}, \cdots, s_{i,K})$：

1. 生成 $(s'_{i,1}, \cdots, s'_{i,K})$，其中 $s'_{i,j} = |\mathrm{randnormal}()|$。
2. 计算 $q_i = \frac{\mathrm{randdouble}(20, 60)}{\sqrt{\sum_{j=1}^K s'_{i,j}^2}}$。
3. 生成 $s_{i,j} = \mathrm{round}(q_i \cdot s'_{i,j})$。

#### $(u_i, v_i)$ 的生成
从空集合 $E = \emptyset$ 开始，直到 $|E| = R$，循环以下步骤生成：

1. 生成 $h = \mathrm{randint}(1, 100)$ 和 $v = \mathrm{randint}(h+1, N)$，设 $u = v - h$。
2. 将 $(u, v)$ 添加到 $E$。

### 工具

- [本地测试器](https://img.atcoder.jp/future-contest-2022-qual/f4ca7c3336de23e5c8d1338981e38375.zip)：需 [Rust 语言](https://www.rust-lang.org/ja) 编译环境。
- [网页可视化工具](https://img.atcoder.jp/future-contest-2022-qual/f4ca7c3336de23e5c8d1338981e38375.html)

工具中使用的输入输出文件包含隐藏信息：技能水平 $\bm{s_i}$ 和各任务实际完成时间 $t_{i,j}$。文件格式如下：

> $N$ $M$ $K$ $R$  
> $d_{1,1} \cdots d_{1,K}$  
> $\vdots$  
> $d_{N,1} \cdots d_{N,K}$  
> $u_1$ $v_1$  
> $\vdots$  
> $u_R$ $v_R$  
> $s_{1,1} \cdots s_{1,K}$  
> $\vdots$  
> $s_{M,1} \cdots $s_{M,K}$  
> $t_{1,1} \cdots t_{1,M}$  
> $\vdots$  
> $t_{N,1} \cdots t_{N,M}$

有这些信息即可自行实现等效测试器。而程序输出的 `#` 开头行视为注释。特别是以 `#s` 开头的行被解释为技能水平预测用于可视化：

> #s $i$ $s_{i,1} \cdots s_{i,K}$

预测值可多次输出，相同 $i$ 的值被更新。通过插入以下注释行可调整示例输出中的预测值变化：

```
2 1 1 2 2
#s 1 0 1
0
#s 2 1 0
1 1 3
0
0
```

这类注释在实际提交中被忽略，因此原样提交也无妨。

### 示例程序 (Python)

```python
# 为团队成员 1 随机分配任务。
import sys
import random

# 读取输入信息
n, m, d, r = list(map(int, input().split()))
task_difficulty = []
for i in range(n):
    task_difficulty.append(list(map(int, input().split())))
task_dependency = [[] for _ in range(n)]
for i in range(r):
    temp = list(map(int, input().split()))
    task_dependency[temp[1] - 1].append(temp[0] - 1)

# -1: 未开始
#  0: 进行中
#  1: 已完成
task_status = [-1] * n

# -1: 未分配
#  k: 被分配的任务 k (1 <= k <= N)
member_status = -1
day = 0

while True:
    day += 1
    output = [0]
    # 随机查找任务
    if member_status < 0:
        tasklist = list(range(n))
        random.shuffle(tasklist)
        for task in tasklist:
            if task_status[task] != -1:
                continue
            ok = True
            for necessary in task_dependency[task]:
                if task_status[necessary] != 1:
                    ok = False
                    break
            if ok:
                task_status[task] = 0
                member_status = task
                output = [1, 1, task + 1]
                break
    str_output = map(str, output)
    print(" ".join(str_output))
    # 输出后刷新标准输出
    sys.stdout.flush()
    temp = list(map(int, input().split()))
    if len(temp) == 1:
        if temp[0] == -1:
            # 天数已达 2000 或所有任务已完成
            exit()
        else:
            # 状态无变化
            pass
    else:
        # 一个任务已完成
        task = member_status
        task_status[task] = 1
        member_status = -1
```


 **本翻译由 AI 自动生成**

## 输入格式

无

## 输出格式

无