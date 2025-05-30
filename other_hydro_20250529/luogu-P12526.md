## 题目描述
CuteWhite 最近迷上了一款多人纸牌游戏。

这个游戏的规则为：每人抽取三张牌，将三张牌的牌面数字加起来作为本轮得分，得分大者获胜。特别地，如果三张牌牌面数字一致，则称为「炸弹」，得分在原基础上额外加 $100$ 分。

但 CuteWhite 计算不太好。因此，他希望你编写一个程序，能快速计算他抽到的三张牌的得分。

## 输入格式
输入共一行三个整数 $a_1$, $a_2$ 和 $a_3$ ($1\le a_1, a_2, a_3\le 13$) ，用一个空格分隔，表示本轮游戏 CuteWhite 抓到的三张牌的牌面数字。

## 输出格式
输出一行，仅一个整数，表示 CuteWhite 的得分。

```input1
6 6 6
```

```output1
118
```

```input2
1 1 4
```

```output2
6
```

## 提示
对于第一组样例，由于三张牌牌面数字一致，得分应在原基础上额外加 $100$ 分，即总得分为 $6+6+6+100=118$。

对于第二组样例，三张牌牌面数字并不一致，故总得分为 $1+1+4=6$。

