## 题目描述
Farmer John wants to remodel the floor of his barn using a collection of square tiles he recently purchased from the local square mart store (which of course, only sells square objects).  Unfortunately, he didn't measure the size of the barn properly before making his purchase, so now he needs to exchange some of his tiles for new square tiles of different sizes.

The N square tiles previously purchased by FJ have side lengths A\_1...A\_N. He would like to exchange some of these with new square tiles so that the total sum of the areas of the his tiles is exactly M.  Square mart is currently offering a special deal: a tile of side length A\_i can be exchanged for a new tile of side length B\_i for a cost of

|A\_i-B\_i|\*|A\_i-B\_i| units. However, this deal only applies to 
previously-purchased tiles -- FJ is not allowed to exchange a tile that he has already obtained via exchanging some other tile (i.e., a size-3 tile cannot be exchanged for a size-2 tile, which is then exchanged for a size-1 tile).

Please determine the minimum amount of money required to exchange tiles so that the sum of the areas of the tiles becomes M.  Output -1 if it is impossible to obtain an area of M.



## 输入格式
\* Line 1: Two space-separated integers, N (1<=N<=10) and M 

(1<=M<=10,000). 

\* Lines 2..1+N: Each line contains one of the integers A\_1 through A\_N, describing the side length of an input square

(1<=A\_i<=100). 



## 输出格式
\* Line 1: The minimum cost of exchanging tiles to obtain M units of total area, or -1 if this is impossible.


## 题目大意
有 $N$ 个正方形，依次给出它们的边长，要求可以换掉一些正方形：如果边长为 $A_i$ 的正方形换成边长为 $B_i$ 的正方形所需代价为：$|A_i-B_i| \times |A_i-B_i|$。问至少花费多少代价使得这 $N$ 个正方形面积总和为 $M$？若无论如何也不可能使这 $N$ 个正方形面积总和为 $M$ 则输出 $-1$。

```input1
3 6 
3 
3 
1 

```

```output1
5 

```

## 提示
There are 3 tiles.  Two are squares of side length 3, and one is a square with side length 1.  We would like to exchange these to make a total area of 6.


Exchange one of the side-3 squares for a side-2 square, and another side-3 square for a side-1 square.  This gives the desired area of 4+1+1=6 and costs 4+1=5 units.

感谢 wjcwinmt 提供翻译


