## 题目描述

Linköping 有一个相当复杂的水资源运输系统。在 Linköping 周围的出水点有一些水井。这些水通过管道输送到其它地点。每条管道是从某一个水井到城市的某个位置的直线管道。  

所有管道在地下的深度相同。因此，无论何时，两个管道相交时，它们会形成交点。幸运的是，管道系统正好是以满足两个管道有交点的方式建造。井不计入交点。任何数量的管道（包括零个与超过两个）都可以来源于每一个水井。  

这些交点导致了一个问题，因为污垢（石灰和其它东西的混合物）往往会卡住交点，导致管道崩溃和坍塌，导致大型水槽孔的形成。这样的水槽孔对 Linköping 的学生有吸引的效果，使他们荒废学业，不受教育，这从长远来看将不只是导致管道系统的崩溃，还有社会的结构。因此，当务之急是管道定期清理。北欧提水再分配公司（NWERC）——负责 Linköping 的水管的——拥有充足的机器人车队才可以完成此任务。一个机器人可以在一条管道的开始位置被插入。然后，机器人通过管道一直到结束，并清除沿途所有交点。到达终点后，机器人转身并返回它开始的井。为了防止机器人互相碰撞，政府法规规定每当两个管相交，它们中的至多一个可以包含一个机器人。  
由于整个水系统在被清洁时必须关闭（另一政府法规），则 NWERC 想迅速完成清洗，使用一批次清洁机器人，都必须在同一时间开始。  

你的任务是验证是否可以做到这一点——即，是否能够把机器人同时插入管道中的一些，在不会有两个机器人相撞的危险下清洁所有交点。

## 输入格式
 
第一行两个整数 $w$ 和 $p$，分别表示井的数量和管道的数量。

接下来 $w$ 行，每行两个整数 $x_i$ 和 $y_i$，表示 $i$ 号井的位置（井从 $1$ 到 $w$ 编号）。

接下来 $p$ 行，每行 $3$ 个整数 $s$ 表示管道从 $s$ 号井开始，$x$ 和 $y$ 表示管道在位置为 $x$，$y$ 的点结束。  

每条管道都有一个井，就是它开始的那个。被两个或多个管道共享的点是一口井。任两条管道至多会有一个交点。两条管道的公共点可以是他们其中之一或两者的端点。所有管道的长度为正数。

## 输出格式

如果在上述情况下可以清理所有交点，输出「possible」，否则输出「impossible」。

```input1
3 3
0 0
0 2
2 0
1 2 3
2 2 2
3 0 3
```

```output1
impossible
```

```input2
2 3
0 0
0 10
1 5 15
1 2 15
2 10 10
```

```output2
possible
```

## 数据范围与约定

对于 $100 \%$ 的数据，$1 \le w \le 1000$，$1 \le p \le 1000$，$-10000 \le x, y \le 10000$，$1 \le s \le w$，$-10000 \le x, y \le 10000$。