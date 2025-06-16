# AT_tricky_4 高橋くんレーシング

## 题目描述

高桥是一位赛车手，使用「Takahashi」的名字参加了一场共 $N$ 人参与的比赛。作为忠实支持者的青木，正在通过广播收听这场比赛。

广播首先公布了比赛开始时所有参赛者的初始排名。青木没能听到每个人的排名，但他成功地记录了高桥的名次。接下来，广播每次播报某个选手超越另一个选手的消息，青木也一一记录下来。

根据青木的记录，你需要计算高桥的最终排名。如果记录中存在逻辑矛盾，请指出这一点。注意，所有参赛者的名字都是独一无二的，且区分大小写。此外，除了在超越的一瞬间，不会有两名或更多的选手同时占据同样的名次。

输入的第一行给出测试用例的数量 $T$。接下来是 $T$ 个测试用例。

每个测试用例的第一行包括参赛者的数量 $N$ 和青木记录的超越事件数量 $R$。下一行提供的信息格式为 `Takahashi is the 順位`，表示高桥在比赛开始时的名次。其中，「順位」由第 $1$ 位依次为 `1st place`、`2nd place`、`3rd place`，直到不超过第 $N$ 位。在后续的 $R$ 行中，每一行记录一条格式为 `名前1 overtakes 名前2` 的信息，表示选手「名前1」超越了「名前2」。

- $0 \leq T \leq 10^4$
- $1 \leq N$
- $0 \leq R \leq 4 \times 10^5$
- `Takahashi is the 順位` 中的「順位」范围为第 $1$ 位到第 $N$ 位
- `名前1` 和 `名前2` 是由长度 $1$ 到 $20$ 之间的半角字母构成的字符串
- 单个测试用例中所有 $R$ 的总和不超过 $4 \times 10^5$

若测试用例中的记录存在矛盾，输出 `The memo must be wrong`。若记录没有矛盾，输出 `Takahashi might get the 順位`，其中「順位」与输入格式中的相同，表示在记录无误的情况下高桥的最终名次。

输入示例：
```
2
3 2
Takahashi is the 2nd place
Takahashi overtakes Aoki
HechoSamurai overtakes Aoki
2 1
Takahashi is the 1st place
Takahashi overtakes Aoki
```

输出示例：
```
Takahashi might get the 1st place
The memo must be wrong
```

输入格式不会出现无效情况，例如：
```
1
3 0
Takahashikun starts with the 2nd place
```

或
```
1
3 1
Takahashi is the 2nd place
Takahashi kicks Aoki
```

请注意，题目并未明确保证 `名前1` 和 `名前2` 是不同的名字。

 **本翻译由 AI 自动生成**

## 输入格式

无

## 输出格式

无