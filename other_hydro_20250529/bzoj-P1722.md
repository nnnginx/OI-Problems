## 题目描述
Farmer John's $n \ (1 \le  n \le  500)$ cows are trying to select the milking team for the world-famous Multistate Milking Match-up (MMM) competition. As you probably know, any team that produces at least $x \ (1 \le  x \le  10^6)$ gallons of milk is a winner. Each cow has the potential of contributing between $-10^4$ and $10^4$ gallons of milk.(Sadly, some cows have a tendency to knock over jugs containing milk produced by other cows.) The MMM prides itself on promoting family values. FJ's cows have no doubt that they can produce $x$ gallons of milk and win the contest, but to support the contest's spirit, they want to send a team with as many parent-child relationships as possible (while still producing at least $x$ gallons of milk). Not surprisingly, all the cows on FJ's farm are female. Given the family tree of FJ's cows and the amount of milk that each would contribute, compute the maximum number of parent-child relationships that can exist in a winning team. Note that a set of cows with a grandmother-mother-daughter combination has two parent-child relationships (grandmother-mother, mother-daughter).


约翰的 $n$ 头奶牛打算组队去参加一个世界级的产奶比赛 MultistateMilking Match-up，（缩写为 MMM）。她们很清楚其他队的实力，也就是说，她们派出的队只要能产出至少 $x$ 加仑牛奶，就能赢得这场比赛。每头牛都能为集体贡献一定量的牛奶，数值在 $-10^4$ 到 $10^4$ 之间（有些奶牛总是想弄翻装着其他奶牛产的奶的瓶子）。MMM 的举办目的之一，是通过竞赛中的合作来增进家庭成员之间的默契。奶牛们认为她们总是能赢得这场比赛，但为了表示对比赛精神的支持，她们希望在选出的队伍里能有尽可能多的牛来自同一个家庭，也就是说，有尽可能多对的牛有直系血缘关系（当然，这支队伍必须能产出至少 $x$ 加仑牛奶）。当然了，所有的奶牛都是女性，所以队伍里所有直系血亲都是母女关系。约翰熟知所有奶牛之间的血缘关系。现在他想知道，如果在保证一支队伍能赢得比赛的情况下，队伍中最多能存在多少对血缘关系。注意，如果一支队伍由某头奶牛和她的母亲、她的外祖母组成，那这支队伍里一共有 $2$ 对血缘关系（这头奶牛外祖母与她的母亲，以及她与她的母亲）。
## 输入格式
* Line $1$: Two space-separated integers,$n$ and $x$.
* Lines $2\dots n+1$: Line $i+1$ contains two space-separated integers describing cow $i$. The first integer is the number of gallons of milk cow $i$ would contribute. The second integer (range $1\dots n$) is the index of the cow's mother. If the cow's mother is unknown, the second number is $0$. The family information has no cycles: no cow is her own mother, grandmother, etc.

- 第一行：两个用空格隔开的整数 $n$ 和 $x$。
- 第二到 $n+1$ 行：每行包括两个用空格隔开的整数，第一个数为一只奶牛能贡献出的牛奶的加仑数，第二个数表示她的母亲的编号。如果她的母亲不在整个牛群里，那第二个数为 $0$。并且，血缘信息不会出现循环，也就是说一头奶牛不会是自己的母亲或祖母，或者更高代的祖先。

## 输出格式
* Line $1$: The maximum number of parent-child relationships possible on a winning team. Print `-1` if no team can win.

* 输出在一个能获胜的队伍中，最多可能存在的有血缘关系的牛的对数。如果任何一支队伍都不可能获胜，输出 `-1`。
```input1
5 8
-1 0
3 1
5 1
-3 3
2 0
```
```output1
2
```
## 样例说明

INPUT DETAILS：  
There are $5$ cows. Cow $1$ can produce $-1$ gallons and has two daughters, cow $2$ and $3$, who can produce $3$ and $5$ gallons, respectively. Cow $3$ has a daughter (cow $4$) who can produce $-3$ gallons. Then there's cow $5$, who can produce $2$ gallons.

约翰一共有 $5$ 头奶牛。第 $1$ 头奶牛能提供 $-1$ 加仑的牛奶，且她是第 $2$、第 $3$ 头奶牛的母亲。第 $2$、第 $3$ 头奶牛的产奶量务别为 $3$ 加仑和 $5$ 加仑。第 $4$ 头奶牛是第 $3$ 头奶牛的女儿，她能提供 $-3$ 加仑牛奶。还有与其他牛都没有关系的第 $5$ 头奶牛，她的产奶量是 $2$ 加仑。最好的一支队伍包括第 $1,2,3,5$ 头奶牛。她们一共能产出 $\ (-1)+3+5+2=9≥8$ 加仑牛奶，并且这支队伍里有 $2$ 对牛有血缘关系（$1—2$ 和 $1-3$）。如果只选第 $2,3,5$ 头奶牛，虽然总产奶量会更高（$10$ 加仑），但这支队伍里包含的血缘关系的对数比上一种组合少（队伍里没有血缘关系对）。

## 数据规模与约定
对于 $100\%$ 的数据，$1 \leq n \leq 500$，$1 \leq x \leq 10^6$。
## 题目来源
Gold