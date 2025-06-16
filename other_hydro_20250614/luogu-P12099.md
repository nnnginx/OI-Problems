## 题目描述
This is an interactive problem.

Harry and Hermione are trying to hunt down $\emph{hoglins}$ which are haunting Hogwarts. There is a long hallway in Hogwarts, consisting of $n$ individual $\emph{cells}$, numbered from $1$ to $n$ from the left to the right.

Hermione can cast a spell that would $\emph{block}$ any cell of the hallway of her choosing. After the spell is cast, the blocked cell will remain blocked while she casts other spells.

Hoglins are simple creatures; all they do is randomly move around and bump into stuff. To be more precise, every hoglin has a range which it considers to be $\emph{accessible}$. Initially, when the hoglin appears, it is a range from the cell $1$ to the cell $n$.

Initially, a single hoglin appears in a cell of the hallway chosen uniformly at random. Then, until this hoglin is caught, the following happens on every $\emph{round}$ of the hunt:

- Hermione can cast a spell to block any single cell of her choosing, or do nothing.
- If the cell she is trying to block is the cell with a hoglin in it, the hoglin is caught. After that, all the blocked cells become free again, and, if there are more hoglins to be caught, a new hoglin immediately appears in a random location, and the hunt begins again.
- Otherwise, the hoglin chooses a cell uniformly at random from its accessible range and tries to move to that cell, moving one cell at a time towards a chosen cell. Regardless of the distance, all the steps of the movement, as described below, happen in the same round.
- If the chosen cell is to the right of the hoglin, it moves to the right; if the chosen cell is to the left of the hoglin, it moves to the left. If the chosen cell is the same as where the hoglin is now, it does nothing.
- If at any point during the movement towards the chosen cell a hoglin is trying to move to the right or to the left from an unblocked cell at position $i$ to the neighbouring blocked cell at position $i \pm 1$, the hoglin updates the right or left boundary of its accessible range correspondingly to be $i$.
- If on the way to the chosen cell, the hoglin tries to move to a blocked cell, Harry and Hermione hear a loud sound, as the hoglin $\emph{bumps}$ into the blocked cell. In this case, the hoglin returns to the position it has originally started from at the beginning of this round. 
- Otherwise, if the hoglin does not bump into any blocked cells on its way, it does not change its accessible range and stays at the new position. In that case, Harry and Hermione hear nothing.

To free Hogwarts from hoglins, Harry and Hermione should catch $k$ of them, but they don't have much time. They can only afford to hunt hoglins for at most $200\,000$ rounds. Please help them find an efficient strategy to do that.

**Interaction Protocol**

First, the testing system will write two integers $n$ and $k$ ($1 \le n \le 10^{18}; 1 \le k \le 800)$ --- the number of cells in Hogwarts' hallway and the number of hoglins that should be caught. Then the catching process begins.

The following interaction proceeds in rounds as described in the problem statement.

At the start of each round, your program should output Hermione's action --- an integer $p$ ($0 \le p \le n$) representing the position of the cell Hermione is going to block. If $p = 0$ or the cell at position $p$ is already blocked, she does nothing in this round.

Then, if the current position of the hoglin is at the newly blocked cell $p$, the hoglin is caught; the testing system outputs $\texttt{2}$, all the blocked cells become free, and interaction rounds start again. In case you caught the $k$-th hoglin, the testing system outputs $\texttt{3}$ instead of $\texttt{2}$, and your program should immediately stop execution.

Otherwise, the hoglin attempts to move according to the rules described in the problem statement. If in the process it bumps into any blocked cell, the testing system outputs $\texttt{1}$; otherwise, it outputs $\texttt{0}$.

If your $200\,000$-th action does not catch the $k$-th hoglin, the testing system outputs $\texttt{-1}$ instead of its usual answer, and your program should immediately stop execution to guarantee the `Wrong Answer` verdict.

The interactor in this problem is not adaptive. It is guaranteed that the hoglins follow the rules described in the problem statement. The starting cell for each hoglin is chosen uniformly at random and their moves are chosen uniformly at random from the range of cells that they consider accessible.

The problem has at most $15$ tests.

Here is the summary of all possible interactor answers:
- $\texttt{-1}$ --- too many actions;
- $\texttt{0}$ --- hoglin moved successfully, did not bump;
- $\texttt{1}$ --- hoglin attempted to move, bumped into blocked cell;
- $\texttt{2}$ --- hoglin is caught, interaction starts again;
- $\texttt{3}$ --- hoglin is caught, stop.

## 输入格式
See also **Interaction Protocol**.

## 输出格式
See also **Interaction Protocol**.

```input1
9 2

0

1

1

0

1

2

1

0

0

3
```

```output1

3

7

5

1

9

4

5

7

0

2
```

## 提示
![](https://cdn.luogu.com.cn/upload/image_hosting/h3gyhxo6.png)

We show the sample from the point of view of the hoglins.

The black dot shows the current position of the hoglin.

Crosses mark blocked cells.

White cells mark the range which the hoglin considers to be accessible; other cells are marked gray.

On the right is the action that was performed by either Hermione or the hoglin to get to this state from the previous one.

