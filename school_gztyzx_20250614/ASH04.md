## 题目背景

（这是废话可以跳过

火光熄灭，黑暗落幕

滴答滴答……黑暗中见一抹红光

玻璃容器中盛满红色液体，金发女孩永葆青春，沉睡其中。

你说她是古代长生不老的神仙，可谁又知道，她是不是西方无恶不作的吸血鬼呢……

“你终于来了……$MY$ $BELIEVER$……嘻嘻嘻……”

## 题目描述

你来到了 $ASH$ 的里世界——一个 $N×N$ 的正方形数字迷宫。

现在你位于迷宫的左上角。迷宫的终点位于右下角。

每一格有一个非负整数，表示该格的信仰值 $a_i$ 。当你走到该格时，你的血徒值将乘上该信仰值。

初始血徒值为 $1$。

你只能向下和向右走。

当然，$ASH$ 不希望你顺利离开这里。她认为血徒值末尾的 $0$ 过多是不好的，因为 $0$ 代表万物毁灭。所以如果当你到达终点时血徒值末尾的 $0$ 多于 $x$ 个，她将让你永远留在 $ASH$ 中，成为她的血徒。

你希望能安全离开 $ASH$ 。如果能安全离开，请寻找一条路径使血徒值末尾的 $0$ 尽可能少。否则输出 `ASH BELIEVER!`。

## 输入格式

第一行一个正整数 $N$，表示该正方形迷宫的规模。

第二行一个非负整数 $x$，含义如题目描述。

接下来 $N$ 行，每行有 $N$ 个非负整数，表示每格的信仰值 $a_i$ 。

## 输出格式

第一行一个整数，表示血徒值结尾最少的 $0$ 的个数。

第二行一行字符串，如果可以逃离，输出相应的路径（ $D$  为向下，$R$ 为向右），否则输出 `ASH BELIEVER!`。

## 输入数据1

```
3
0
1 2 3
4 5 6
7 8 9
```

## 输出数据1

```
0
DDRR
```

## 数据范围

对于$30％$的数据，$x=0$。

对于$100％$的数据，$0≤x≤1000，2≤N≤1000，0≤a_i≤10^9$。

