## Statement

A scourge of frogs destroying all the crop has started in Byteotia. A farmer named Byteasar has decided to fight the vermin with peculiar "scarefrogs", that he has set up at certain points of his field. While moving from one place to another, every frog tries to keep as far of them as possible, i.e. maximizes the distance to the closest scarefrog.

The field that belongs to Byteasar has rectangular shape. The frogs leap in directions parallel to the field's sides and their leaps are unitary (of length 1). The scarefrogs-distance, for a given frog's route, is the minimum of all distances from all scarefrogs at all inter-leap-points of the route.

Byteasar already knows the most common starting and destination points of the frogs' routes, therefore he experiments with various deployments of the scarefrogs. He asks you for help, namely he would like you to write a programme that calculates the maximum (over all routes) scarefrogs-distance for a given deployment of scarefrogs - which we call in short the frogshold distance.

TaskWrite a programme that:

reads from the standard input the size of the field, the coordinates of the screfrogs and the source and target position of a frog,determines the frogshold distance (the maximum scarefrogs-distance a frog may achieve while still being able to reach the target point) writes the square of this number to the standard output.

![](./1064/file/pic1.jpg)

## Input Format

The first line of the input contains two integers: $w_x$ and $w_y$ separated by a single space - the breadth and length of the field. The second line of the input contains four integers: $p_x$, $p_y$, $k_x$ and $k_y$ separated by single spaces; $(p_x, p_y)$ is the initial position of the frog, $(k_x, k_y)$ is the target (final) position of the frog ($1 \le p_x, k_x \le w_x$, $1 \le p_y, k_y \le w_y$). The third line of the standard input contains one integer $n$ - these are the coordinates of the ith scarefrog $(1 \le n \le w_x \cdot w_y)$. No two scarefrogs occupy the same position and none of them is at the point $(p_x, p_y)$ nor $(k_x, k_y)$.

## Output Format

In the first and only line of the standard output one integer should be written, namely the square of the frogshold distance. If the frog cannot avoid leaping directly on some scarefrog the result is 0.

```input1
5 5
1 1 5 5
2
3 3
4 2
```
```output1
4
```

## Constraints

$2 \le w_x, w_y \le 10^3$
