## 题目描述
Farmer John has decided his home needs more decoration. Visiting the local china shop, he finds a delicate glass cow figurine that he decides to purchase, knowing that it will fit perfectly on the mantel above his fireplace.

The shape of the cow figurine is described by an $N \times M$ grid of haracters like the one below ($3 \leq N, M \leq 500$), where lowercase letter characters are each part of the figurine (indicating different colors) and '.' characters are not.

```
...............
...............
x..x...........
xxxx...........
xxxxaaaaaaa...
.xx.aaaaaaaaa..
....aaaaaaa.aa.
....ll...ll....
....vv...vv....
...............
```

Unfortunately, right before FJ can make his purchase, a bull runs through the shop  and breaks not only FJ's figurine, but many of the other glass objects on the shelves as well!  FJ's figurine breaks into 3 pieces, which quickly becomelost  among $K$ total pieces lying on the ground ($4 \leq K \leq 100$).  Each ofthe $K$ pieces is described by a grid of characters, just like the originalfigurine.

Please help FJ determine how many sets of 3 pieces (out of the $K$ on the floor)could be glued back together to mend his broken figurine.

The pieces on the ground might have been flipped vertically or horizontally, orrotated by some multiple of 90 degrees. Therefore, given the original grid aswell as $K$ grids describing pieces, you want to find sets of 3 pieces that canbe joined together to form the original picture, allowing the pieces to betranslated, flipped, or rotated multiples of 90 degrees.  When thensuperimposed, the 3 pieces should exactly form the original picture, with eachcolored square in the original picture represented in exactly one of the pieces.

## 输入格式
The first line contains a single integer $K$. Following that will be $K + 1$ piece descriptions.  The first description will describe the original glass cow,the following $K$ descriptions will be of the broken pieces.

Each description begins with a line containing two integers $R$ and $C$ ($1 \le R, C \le 100$).  The following $R$ lines contain $C$ lowercase alphabet characters describing the color of each cell.  Each piece will be horizontally/vertically connected and have at least one non-empty cell.


## 输出格式
Output the number of triples $i, j, k$ ($i < j < k$) such that pieces $i$, $j$, and $k$ can be arranged to form the original glass cow.

## 题目大意
### 题目描述

Farmer John 决定给他的家增添一些装饰。在当地的瓷器店里，他发现了一尊精致的玻璃牛雕像，决定购买它，因为它完美地适合放在壁炉上方的壁炉架上。

牛雕像的形状由一个 $N \times M$ 的字符网格描述（$3 \leq N, M \leq 500$），其中小写字母字符代表雕像的各个部分（表示不同的颜色），而 '.' 字符则不代表雕像部分。

```cpp
...............
...............
x..x...........
xxxx...........
xxxxaaaaaaa...
.xx.aaaaaaaaa..
....aaaaaaa.aa.
....ll...ll....
....vv...vv....
...............
```

不幸的是，就在 FJ 准备购买之前，一头公牛冲进了商店，不仅撞碎了 FJ 的雕像，还撞碎了许多其他货架上的玻璃制品！FJ 的雕像碎成了 3 块，并迅速混入了地上的 $K$ 块碎片中（$4 \leq K \leq 100$）。每一块碎片都由一个字符网格描述，就像原来的雕像一样。

请帮助 FJ 确定有多少组 3 块碎片（地上的 $K$ 块中）可以粘合在一起修复他破碎的雕像。

地上的碎片可能被垂直或水平翻转，或者旋转了 90 度的倍数。因此，给定原始网格以及描述碎片的 $K$ 个网格，你需要找到可以组合成原始图片的 3 块碎片，允许碎片被平移、翻转或旋转 90 度的倍数。当这 3 块碎片叠加在一起时，它们应该准确地形成原始图片，且原始图片中的每个彩色方块都恰好出现在一块碎片中。

### 输入格式

第一行包含一个整数 $K$。接下来是 $K + 1$ 个碎片的描述。第一个描述是原始玻璃牛的描述，接下来的 $K$ 个描述是破碎的碎片。

每个描述以两个整数 $R$ 和 $C$（$1 \le R, C \le 100$）开始。接下来的 $R$ 行包含 $C$ 个小写字母字符，描述每个单元格的颜色。每块碎片在水平/垂直方向上都是连通的，并且至少有一个非空单元格。

### 输出格式

输出满足条件的三元组 $i, j, k$（$i < j < k$）的数量，使得碎片 $i$、$j$ 和 $k$ 可以排列成原始玻璃牛。

### 说明/提示

三个解决方案使用了碎片 $(0, 1, 2)$、$(0, 2, 4)$ 和 $(1, 3, 4)$。

请注意，这个问题每个测试用例的时间限制为 6 秒（Java 和 Python 提交的时间限制为 12 秒）。

```input1
5
5 5
aaaaa
..a..
bbabb
..a..
aaaaa
3 5
..abb
..a..
aaaaa
5 2
a.
a.
aa
a.
a.
1 2
bb
1 5
bbabb
2 5
aaaaa
..a..
```

```output1
3
```

## 提示
The three solutions use pieces $(0, 1, 2)$, $(0, 2, 4)$, $(1, 3, 4)$.

Note that this problem has a time limit of 6 seconds per test case (and twice that  for Java and Python submissions).

