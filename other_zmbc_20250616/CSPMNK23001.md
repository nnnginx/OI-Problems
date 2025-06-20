# 【题目描述】

芝麻同学暑假在老家放羊，放羊时需要经过一座铁索桥，于是他就将他的羊群赶到前方的铁索桥上，而他自己则留在羊群后方。羊群十分慌张，因为这座铁索桥十分狭窄，只能容纳一只羊通过。假如有 2 只羊相向而行在桥上相遇，那么它们 2只羊将无法绕过对方，只能有 1 只羊回头下桥，让另一只羊先通过。但是，可以有多只羊同时呆在同一个位置。

突然，芝麻同学看到了天上盘旋的雄鹰，它正朝着羊群所在的铁索桥飞来! 为了安全，芝麻同学的羊群必须全部撤离铁索桥。铁索桥的长度为 L，羊群只能呆在坐标为整数的地方。所有羊的速度都为 1，但一只羊某一时刻来到了坐标为 0或 L+1 的位置，它就离开了独木桥。

每只羊都有一个初始面对的方向，它们会以匀速朝着这个方向行走，中途不会自己改变方向。但是，如果两个只羊面对面相遇，它们无法彼此通过对方，于是就分别转身，继续行走。转身不需要任何的时间。

由于雄鹰的惊吓，芝麻同学已不能控制他的羊群。甚至，他连每只羊初始面对的方向都不知道。因此，他想要知道他的羊群最少需要多少时间就可能全部撤离铁索桥。另外，芝麻同学的爷爷也带着猎枪在赶来的路上了，因此他还需要知道他的羊群最多需要多少时间才能全部撤离铁索桥。

## 【输入格式】

从文件bridge.in中读入数据

第一行共一个整数 L，表示铁索桥的长度。桥上的坐标为 1, 2, ……, L。

第二行共一个整数 N，表示初始时留在桥上的羊群数目。

第三行共有 N 个整数，分别表示每只羊的初始坐标。

## 【输出格式】

输出到文件bridge.out中

共一行，输出 2个整数，分别表示羊群撤离铁索桥的最小时间和最大时间。2个整数由一个空格符分开。

# 【样例1输入输出】

```input1
4
2
1 3
```

```output1
2 4
```

# 【数据范围】

对于 100%的数据，满足初始时，没有两只羊同在一个坐标，1≤L≤5 * 10^3，0≤​*N*​≤5 * 10^3，且数据保证​*N*​≤​*L*​。

