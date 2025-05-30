## 题目描述
A little-known fact about cows is that they love puzzles! For Bessie's birthday, Farmer John gives her an interesting mechanical puzzle for her to solve.  The puzzle consists of three solid objects, each of which is built from 1x1 unit squares glued together.  Each of these objects is a "connected" shape,  in the sense that you can get from one square on the object to any other square on the object by stepping north, south, east, or west, through squares on the object.

An object can be moved by repeatedly sliding it either north, south, east, or west one unit.  The goal of the puzzle is to move the objects so that they are separated -- where their bounding boxes no longer share any positive overlap with each-other.  Given the shapes and locations of the three objects, your task is to help Bessie decide what is the minimum number of individual slides required to separate the objects.

![](https://cdn.luogu.com.cn/upload/image_hosting/flelqdzu.png)



## 输入格式
\* Line 1: Three space-separated integers: N1, N2, and N3, describing respectively the number of unit squares making up objects 1, 2, and 3.

\* Lines 2..1+N1: Each of these lines describes the (x,y) location of the south-west corner of single square that is part of object 1.  All coordinates lie in the range 0..9.

\* Lines 2+N1..1+N1+N2: Each of these lines describes the (x,y) location of the south-west corner of single square that is part of object 2.  All coordinates lie in the range 0..9.

\* Lines 2+N1+N2..1+N1+N2+N3: Each of these lines describes the (x,y) location of the south-west corner of single square that is part of object 3.  All coordinates lie in the range 0..9.


第1行：三个整数N1,N2,N3，表示组成模块1,2,3的小正方体数目。


第2行到第N1+1行：读入一对坐标（x，y），每对坐标表示组成模块1的一个小正方体西南角落的位置。所有坐标在0..9之间。


第N1+2行到第N1+N2+1行：读入一对坐标（x，y），每对坐标表示组成模块2的一个小正方体西南角落的位置。所有坐标在0..9之间。


第N1+N2+2行到第N1+N2+N3+…


## 输出格式
\* Line 1: The minimum number of moves necessary to separate the three objects, or -1 if the objects cannot be separated.


## 题目大意

奶牛们一个鲜为人知的事实是它们爱解谜！Bessie生日时农夫约翰给了她一个有趣的机械锁给她解决。锁由三个模块构成，每一个模块都由1x1的小立方体粘连而成。每一个模块都是一个“连通”的模型，那么，你就可以通过在模型上的小正方体间向北、南、东或西走而从模型的一个小正方形到达模型上的任何其他小正方形。


一个模块可以多次向东西南北滑动一个单位。拼图的目标是滑动模块使其分离——即使它们的边界框不再有任何重叠。给定三个模块的形状与位置，请你帮助Bessie找到达到目标需要的最小滑动次数。

```input1
12 3 5 
0 0 
1 0 
2 0 
3 0 
3 1 
0 1 
0 2 
0 3 
0 4 
1 4 
2 4 
3 4 
2 1 
2 2 
1 2 
2 3 
3 3 
4 3 
4 4 
4 2 

```

```output1
5 

```

## 提示
Object 1 is made from 12 squares, object 2 is made from 3 squares, and object 3 is made from 5 squares.  The shapes of the objects are those in the figure above.


If we slide object 3 to the east by one position, then slide object 2 north by one position, then slide object 1 west by three positions, then the bounding boxes of the three objects will no longer share any overlap in common.

模块1由12块小正方体制造，模块2由3块小正方体制造，模块3由5块小正方体制造。最后的图像在如上。（吃图？！）

```cpp
A：模块1方块 B：模块2方块 C：模块3方块 *：啥都木有
A A A A C
A * C C C
A B B * C
A * B A *
A A A A *
```
假如我们把模块3向东移一个单位，然后把模块2向北移一个单位，然后把模块1向西移三个单位，就满足了条件。

感谢 @姚起龙 提供翻译


