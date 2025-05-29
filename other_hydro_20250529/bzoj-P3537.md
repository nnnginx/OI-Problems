## Statement

The cows keep getting in trouble by taking rides on Farmer John's tractor, so he has hidden the keys to the tractor in a fancy new safe in his office. Undeterred, the cows have vowed to try and break into this safe.

The safe is protected by a rather complicated passcode system. The passcode entry system is arranged as a rooted tree of $n$ nodes, each of which requires a digit between $0$ and $9$. The nodes are indexed $0 \dots n - 1$.

The only information that the cows have is that certain sequences of length $5$ do not occur along particular paths upwards through the tree.

For instance, suppose the tree is the following (rooted at `A`):

```plain
A <- B <- C <- D <- E
               ^
               |
               F
```

The cows might know that the sequence $01234$ does not occur starting at `F`, and that the sequence $91234$ does not occur starting at `E`. This information rules out $19$ possible passcodes: all those of the form

```plain
4 <- 3 <- 2 <- 1 <- *
               ^
               |
               0
```

or

```plain
4 <- 3 <- 2 <- 1 <- 9
               ^
               |
               *
```

which gives $19$ once we account for the fact that

```plain
4 <- 3 <- 2 <- 1 <- 9
               ^
               |
               0
```

appears twice.

Given $m$ length-$5$ sequences, together with their starting nodes in the tree, help the cows figure out how many passcodes have been ruled out. You should compute your answer modulo $1234567$.

## Input Format

Line $1$: Two space-separated integers, $n$ and $m$.

Lines $2 \dots n$: Line $i + 1$ contains a single integer $p_i$, denoting the parent of node $i$ in the tree.

Lines $n + 1 \dots n + m$: Line $n + i$ describes the $i$-th sequence known not to occur in the code. The line will contain $v_i$ and $s_i$ separated by a space, where $v_i$ is the starting node of the sequence, and $s_i$ is a $5$-digit string known not to occur starting at $v_i$ and proceeding upward in the tree. It is guaranteed that the root is at least $4$ steps upward from $v_i$.

## Output Format

Line $1$: A single integer giving the number of ruled-out configurations, modulo $1234567$.

```input1
6 2
0
1
2
3
3
4 01234
5 91234
```
```output1
19 
```

## Constraints

$1 \le n \le 2 \times 10^4,~1 \le m \le 5 \times 10^4,~0 \le p_i < i$
