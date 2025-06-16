## 题目描述

Farmer John's cows would like to host a dance party in their barn, complete with a laser light show. Unfortunately, the only working laser they have found is located far away from the barn and too heavy to move, so they plan to re-direct the laser light to the barn using a series of mirrors.

The layout of the farm has the laser at position $(0,0)$ pointing north (in the positive $y$ direction), and the barn at $(B_x, B_y)$; we can think of both the laser and the barn as points in the 2D plane. There are already $n$ cows scattered throughout the farm holding mirrors that are aligned at angles of $45$ degrees to the axes. For example, a mirror aligned like `\` will take a beam of light entering from below and reflect it to the left. We can also think of the mirrors as being located at points in the 2D plane.

Just before pressing the big red button to activate the laser, Bessie noticed a major flaw in the plan: the laser cannot hit the barn with the mirrors in their current configuration! As a result, she plans to run out onto the field, and hold up one more mirror (placed once again at a $45$ degree angle) in order to redirect the laser onto the barn. Please count the number of locations in the field where Bessie can stand to accomplish this goal.

All coordinates are integers between $-10^9$ and $10^9$. It is guaranteed that any mirrors to be placed will be in this range as well. The cows running the laser insist that the beam should never come back to $(0,0)$ after leaving this location (and with the mirrors in their initial configuration, it is guaranteed that this will not happen). No two cows occupy the same point in space, and Bessie cannot locate herself at the same position as an existing cow.

## 输入格式

Line $1$: The integers $n$, $B_x$, and $B_y$.

Lines $2 \dots n + 1$: Line $i + 1$ describes the $i$-th mirror with $3$ elements: its $(x,y)$ location, and its orientation (either `\` or `/`).

## 输出格式

A single integer giving the number of locations where Bessie can stand to redirect the laser to the barn.

```input1
4 1 2
-2 1 \
2 1 /
2 2 \
-2 2 /
```
```output1
2
```

OUTPUT DETAILS: A mirror at $(0,1)$ or $(0,2)$ placed in either direction would do the trick. 

## 提示

$1 \le n \le 10^5$
