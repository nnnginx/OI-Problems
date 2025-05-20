Farmer John has a brilliant idea for the next great spectator sport: Cow
Steeplechase! As everyone knows, regular steeplechase involves a group of
horses that race around a course filled with obstacles they must jump over.
FJ figures the same contest should work with highly-trained cows, as long
as the obstacles are made short enough.

In order to design his course, FJ makes a diagram of all the $N$ possible obstacles he could potentially build. Each one is represented
by a line segment in the 2D plane that is parallel to the horizontal or
vertical axis. Obstacle $i$ has distinct endpoints $(X1_i, Y1_i)$ and $(X2_i,
Y2_i)$. An example is as follows:

```plain
   --+-------   
-----+-----
  ---+---     |
     |     |  |
   --+-----+--+-   |
     |     |  |  | |
     |   --+--+--+-+-
           |  |  | |
              |
```

FJ would like to build as many of these obstacles as possible, subject to
the constraint that no two of them intersect. Starting with the diagram
above, FJ can build $7$ obstacles:

```plain
   ----------   
-----------
  -------     |
           |  |
           |  |    |
           |  |  | |
           |  |  | |
           |  |  | |
              |
```

Two segments are said to intersect if they share any point in common, even an endpoint of one or both of the segments.  FJ is certain that no two horizontal segments in the original input diagram will intersect, and that similarly no two vertical segments in the input diagram will intersect.

Please help FJ determine the maximum number of obstacles he can build.

> - $1 \leqslant N \leqslant 250$
> - $1 \leqslant X1_i, Y1_i, X2_i, Y2_i \leqslant 1,000,000,000$

## Input Format

* Line 1: A single integer: $N$.

* Lines $2..N+1$: Line $i+1$ contains four space-separated integers representing an obstacle: $X1_i$, $Y1_i$, $X2_i$, and $Y2_i$.

## Output Format

* Line 1: The maximum number of non-crossing segments FJ can choose.

```input1
3
4 5 10 5
6 2 6 12
8 3 8 5
```
```output1
2
```
>

> **Input Details**
> 
> There are three potential obstacles. The first is a horizontal segment connecting $(4, 5)$ to $(10, 5)$; the second and third are vertical segments connecting $(6, 2)$ to $(6, 12)$ and $(8, 3)$ to $(8, 5)$.
>

> **Output Details**
>

> The optimal solution is to choose both vertical segments.