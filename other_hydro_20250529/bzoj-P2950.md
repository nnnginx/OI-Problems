## 题目描述
Byteland 一直以奇妙的跳舞蝇而闻名于世。驯养的苍蝇能和着音乐的节奏精确地做每一次飞跃。

通常，训练者会在桌上放一排硬币，这些硬币的排列并不按照特定的顺序。每枚硬币上都有一行题字：$i\to j$，$i$ 是这枚硬币的编号，$j$ 是站在硬币 $i$ 上的苍蝇下一步应该飞往的硬币编号。训练者在每个硬币上放一只苍蝇，然后开始放音乐。那些苍蝇就跟着音乐的节拍开始跳舞，在每一拍中苍蝇都会直接跳到编号为 $j$ 的硬币上。在舞蹈中，可能会出现多只苍蝇在同一硬币上的情况。这样，跳舞蝇就会一起继续表演。假定有 $n$ 只苍蝇，$n$ 枚硬币。则一旦确定了 $n$ 枚硬币上的题字，那么这场表演也就确定了。然而，对硬币不同的设置也可能导致相同的表演，只要我们把硬币按适当的顺序排列。

让我们先来看 $3$ 枚硬币上的表演。如果表演是这样进行：从第一个硬币到第二个，第二个到第三个，第三个又回到第一个硬币（表示为 $1\to 2$，$2\to 3$，$3\to 1$）。具体表演是 $3$ 只苍蝇绕圈跳跃，从不相遇。那么表演 $1\to 2$，$2\to 3$，$3\to 3$，则是与其不同的。因为该表演为：两拍后，所有的苍蝇在第3枚硬币上相遇，然后一直在原地跳跃。

但是，设置 $1\to 2$，$2\to 3$，$3\to 2$，$4\to 4$ 和 $1\to 1$，$2\to 3$，$3\to 2$，$4\to 3$ 就是同样的类型。如果你把前者的硬币从左到右排列，而把后者从右到左排列，就会看到相同的表演。

如果跳舞蝇的两次表演是相同的，就会使观众不满，请编写一个程序，读入两组硬币设置，验证是否能把硬币按一定顺序排列，使跳舞蝇给出相同的表演。
## 输入格式
本题有多组测试数据。

第一行读入一个整数 $d$，表示数据组数。

接下来依次输入 $3d$ 组数据，每组数据 $3$ 行。

每组数据中，第一行输入一个整数 $n$，表示硬币个数。

第二行和第三行每行输入 $n$ 个整数，描述一套硬币。第 $i$ 个整数表示硬币 $i$ 上的苍蝇应该飞向的硬币的编号。
## 输出格式
对每个任务，输出一行，仅包含一个字母。如果可以按一定顺序排硬币使表演相同则输出 ``T``，否则输出 ``N``。
## 样例输入
```plain
2
3
2 3 1
2 3 3
4
2 3 2 4
1 3 2 3
```
## 样例输出
```plain
N
T
```
## 数据规模与约定
对于所有数据，$1\leq d\leq 100$，$1\leq n\leq 2000$。