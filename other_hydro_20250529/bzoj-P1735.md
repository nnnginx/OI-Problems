## 题目描述

Rain has pummeled the cows' field, a rectangular grid of $r$ rows and $c$ columns $(1 \le r, c \le  50)$. While good for the grass, the rain makes some patches of bare earth quite muddy. The cows, being meticulous grazers, don't want to get their hooves dirty while they eat. To prevent those muddy hooves, Farmer John will place a number of wooden boards over the muddy parts of the cows'field. Each of the boards is $1$ unit wide, and can be any length long. Each board must be aligned parallel to one of the sides of the field. Farmer John wishes to minimize the number of boards needed to cover the muddy spots, some of which might require more than one board to cover. The boards may not cover any grass and deprive the cows of grazing area but they can overlap each other. Compute the minimum number of boards FJ requires to cover all the mud in the field.

大雨侵袭了奶牛们的牧场。牧场是一个 $r \times c$ 的矩形。大雨将没有长草的土地弄得泥泞不堪，可是小心的奶牛们不想在吃草的时候弄脏她们的蹄子。为了防止她们的蹄子被弄脏，约翰决定在泥泞的牧场里放置一些木板。每一块木板的宽度为 $1$ 个单位，长度任意。每一个板必须放置在平行于牧场的泥地里。约翰想使用最少的木板覆盖所有的泥地。一个木板可以重叠在另一个木板上，但是不能放在草地上。

## 输入格式
* Line $1$: Two space-separated integers: $r$ and $c$.
* Lines $2\dots r+1$: Each line contains a string of $c$ characters, with `*` representing a muddy patch, and `.` representing a grassy patch. No spaces are present.
* 第一行：两个整数 $r$ 和 $c$。
* 第二到 $r+1$ 行：每行 $c$ 个字符，其中 `*` 代表泥地，`.` 代表草地。
## 输出格式
* Line $1$：A single integer representing the number of boards FJ needs.
* 最少需要多少木板。
```input1
4 4
*.*.
.***
***.
..*.
```
```output1
4
```
## 样例说明
Boards $1,2,3$ and $4$ are placed as follows：
```
|1|.|2|.|
|.|3|3|3|
|4|4|4|.|
|.|.|2|.|
```
Board $2$ overlaps boards $3$ and $4$.
## 数据规模与约定
对于 $100\%$ 的数据，$1 \leq r,c \leq 50$。
## 题目来源
Gold