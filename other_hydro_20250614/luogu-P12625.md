## 题目描述
In a certain popular sandbox video game, one can build a structure called a *mob grinder*.

A mob grinder consists of an $N\times M$ rectangular grid of tiles. Monsters, also known as "mobs", appear continuously at random places on the grid. The goal of a mob grinder is to move all of the monsters to the top-right tile in the grid, no matter where they originally appear. To accomplish this goal, each tile (except for the top-right tile) has a conveyor belt on it with a specified direction (up, right, down, or left). A monster on a conveyor belt gets moved to the orthogonally adjacent tile in the direction specified by the conveyor belt orientation.

Your job is to place a conveyor belt on each tile (other than the top-right corner) so that no matter where a monster appears on the grid, it will get moved to the top-right corner after a finite amount of time, without ever leaving the bounds of the grid. However, there is a limit on how many conveyor belts you can use of each orientation: your final design must have exactly $U$ conveyor belts going up, $R$ going right, $D$ going down, and $L$ going left.

You are asked to design multiple mob grinders, each with a specification of how many conveyor belts of each type you are allowed to use. Design a valid mob grinder that meets each specification, if possible.

## 输入格式
The first line of input contains an integer $T$ ($1 \leq T \leq 10^5$): the number of mob grinders you need to design.

Each of the next $T$ lines of input contains six space-separated integers that describe one mob grinder specification. The first two integers, $N$ and $M$, ($1\leq N,M$ and $N\cdot M \leq 10^5)$ are the number of rows and columns in the grid, respectively. The last four, $U$, $R$, $D$, $L$ $(0 \leq U, R, D, L$ and $U+R+D+L = (N \cdot M)-1)$, are the number of times you must use each conveyor belt orientation in your design.

It is guaranteed that the sum of $N\cdot M$ over all $T$ mob grinders does not exceed $10^5$.

## 输出格式
Print $T$ mob grinder designs, one for each specification. Separate consecutive designs with a single empty line.

If it is impossible to construct a valid mob grinder respecting the given constraints for the given specification, print $\texttt{impossible}$. Otherwise, print an $N\times M$ grid of ASCII characters. The top-right tile must be a $\texttt{*}$. 
Every other character in the grid must be either $\texttt{U}$, $\texttt{R}$, $\texttt{D}$, or $\texttt{L}$, representing the orientation of the conveyor belt on that grid tile.

**This problem is whitespace-sensitive.** You *must* separate each mob grinder design with exactly one empty line (containing just a newline character). You *must not* print an empty line, or any other extraneous output, after the last mob grinder design (though the last line of output must be terminated with a newline). Please see the Sample Output for examples of how to correctly format your mob grinder designs.

```input1
2
4 3 5 3 1 2
1 2 0 1 0 0
```

```output1
RR*
URU
UDU
ULL

R*
```

```input2
3
3 3 0 0 0 8
2 2 0 2 0 1
1 1 0 0 0 0
```

```output2
impossible

impossible

*
```

