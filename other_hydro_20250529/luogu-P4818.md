## 题目描述
After eating too much fruit in Farmer John's kitchen, Bessie the cow is getting some very strange dreams! In her most recent dream, she is trapped in a maze in the shape of an $N×M$ grid of tiles $(1≤N,M≤1,000)$. She starts on the top-left tile and wants to get to the bottom-right tile. When she is standing on a tile, she can potentially move to the adjacent tiles in any of the four cardinal directions.

But wait! Each tile has a color, and each color has a different property! Bessie's head hurts just thinking about it:

- If a tile is **red**, then it is impassable.

- If a tile is **pink**, then it can be walked on normally.

- If a tile is **orange**, then it can be walked on normally, but will make Bessie smell like oranges.

- If a tile is **blue**, then it contains piranhas that will only let Bessie pass if she smells like oranges.

- If a tile is **purple**, then Bessie will slide to the next tile in that direction (unless she is unable to cross it). If this tile is also a purple tile, then Bessie will continue to slide until she lands on a non-purple tile or hits an impassable tile. Sliding through a tile counts as a move. **Purple tiles will also remove Bessie's smell.**

(If you're confused about purple tiles, the example will illustrate their use.)

Please help Bessie get from the top-left to the bottom-right in as few moves as possible. 

## 输入格式
 The first line has two integers $N$ and $M$, representing the number of rows and columns of the maze.

The next $N$ lines have $M$ integers each, representing the maze:

- The integer '0' is a red tile

- The integer '1' is a pink tile

- The integer '2' is an orange tile

- The integer '3' is a blue tile

- The integer '4' is a purple tile 

The top-left and bottom-right integers will always be '1'. 

## 输出格式
A single integer, representing the minimum number of moves Bessie must use to cross the maze, or -1 if it is impossible to do so. 

## 题目大意
### 题目描述

Bessie 在 Farmer John 的厨房暴食水果后，开始做奇怪的梦！在最近的梦境中，她被困在一个 $N \times M$ 的网格迷宫（$1 \leq N,M \leq 1,000$）中。她需要从左上角的格子移动到右下角的格子。当站在某个格子时，她可以向四个基本方向移动至相邻格子。

但请注意！每个格子有不同的颜色和特殊属性：

- **红色（0）**：不可通行  
- **粉色（1）**：可正常通行  
- **橙色（2）**：可正常通行，且会使 Bessie 带有橙子气味  
- **蓝色（3）**：仅当 Bessie 带有橙子气味时方可通行  
- **紫色（4）**：Bessie 将沿该方向滑动到下一个格子（除非无法通过）。若下一个格子仍是紫色，则继续滑动直至遇到非紫色格子或不可通行格子。**每次滑动均计为一步移动**，且**紫色格子会消除 Bessie 的气味**

（若对紫色格子机制有疑问，样例将帮助理解）

请帮助 Bessie 找到从左上角到右下角的最短路径步数。

### 输入格式

第一行包含两个整数 $N$ 和 $M$，表示迷宫的行数和列数。  
接下来 $N$ 行每行包含 $M$ 个整数描述迷宫：  
- 0 表示红色  
- 1 表示粉色  
- 2 表示橙色  
- 3 表示蓝色  
- 4 表示紫色  

保证左上角和右下角的格子始终为 1。

### 输出格式

输出一个整数，表示 Bessie 穿越迷宫所需的最少步数，若无法到达则输出 -1。

### 说明/提示

样例中，Bessie 的移动路径为：向下 1 步，向右 2 步（滑动再向右 1 步），向上 1 步，向左 1 步，向下 1 步（滑动再向下 2 步），最后向右 1 步。总计 10 步（路径表示为 DRRRULDDDR）。

题目提供者：Nathan Pinsker，灵感来自游戏《Undertale》  

```input1
4 4
1 0 2 1
1 1 4 1
1 0 4 0
1 3 1 1
```

```output1
10
```

## 提示
In this example, Bessie walks one square down and two squares to the right (and then slides one more square to the right). She walks one square up, one square left, and one square down (sliding two more squares down) and finishes by walking one more square right. This is a total of 10 moves (DRRRULDDDR).

Problem credits: Nathan Pinsker, inspired by the game "Undertale". 

