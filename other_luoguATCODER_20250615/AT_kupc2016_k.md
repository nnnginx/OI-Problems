# AT_kupc2016_k 百目おばけ

## 题目描述

- 你是一个使用召唤术的魔法师，能够将画在素描本上的怪物实体化。
- 京都大学灵长类研究所请求你召唤一个“百目妖怪”。
- 你决定使用你的魔法技能来创造一个高质量的“百目妖怪”。

**问题**：
- 在二维平面上有两个圆A和B。
- 圆A的中心坐标是\( (x_A, y_A) \)，半径是\( r_A \)。
- 圆B的中心坐标是\( (x_B, y_B) \)，半径是\( r_B \)。
- 这两个圆没有重叠的部分。
- 需要考虑一个圆的集合S，满足以下条件：
  - 集合S中的任意圆与A和B相切，且内部没有共同部分。
  - 集合S中的任意两个不同的圆C1和C2，内部没有共同部分。
- 需要求出集合S的最大元素数量。

## 输入格式

- 首先输入一个整数T，表示测试案例的数量。
- 每个测试案例包含六个整数，分别代表圆A和B的中心坐标和半径。

## 输出格式

- 对于每个测试案例，输出一个整数，表示该测试案例中集合S的最大元素数量。

**输入输出样例**：
- 输入：4个测试案例，每个案例包含两个圆的中心坐标和半径。
- 输出：每个测试案例的集合S的最大元素数量。

## 输入输出样例 #1

### 输入 #1

```
4
0 -3 2 0 3 2
0 0 9 8 8 2
0 0 9 10 10 5
0 0 707 1000 1000 707
```

### 输出 #1

```
3
10
21
180
```

## 说明/提示

- 描述了魔法师如何使用魔法来创造“百目妖怪”，以及如何考虑在两个圆之间放置尽可能多的眼睛。

**制約**：
- T的值在1到50000之间。
- 圆A和B的中心坐标和半径的值在-10^5到10^5之间。
- 圆A和B的半径平方和小于它们中心点之间的距离的平方。

**Sample Explanation**：
- 对于第一个和第二个测试案例，给出了如何放置圆的示例图片。