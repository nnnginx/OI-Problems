## Description

<div><p>Little Petya very much likes rectangles and especially squares. Recently he has received 8 points on the plane as a gift from his mother. The points are pairwise distinct. Petya decided to split them into two sets each containing 4 points so that the points from the first set lay at the vertexes of some square and the points from the second set lay at the vertexes of a rectangle. Each point of initial 8 should belong to exactly one set. It is acceptable for a rectangle from the second set was also a square. If there are several partitions, Petya will be satisfied by any of them. Help him find such partition. Note that the rectangle and the square from the partition should have non-zero areas. The sides of the figures <span class="tex-font-style-bf">do not have</span> to be parallel to the coordinate axes, though it might be the case.</p></div><div class="input-specification"><p>You are given 8 pairs of integers, a pair per line �� the coordinates of the points Petya has. The absolute value of all coordinates does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. It is guaranteed that no two points coincide.</p></div><div class="output-specification"><p>Print in the first output line "<span class="tex-font-style-tt">YES</span>" (without the quotes), if the desired partition exists. In the second line output 4 space-separated numbers �� point indexes from the input, which lie at the vertexes of the square. The points are numbered starting from 1. The numbers can be printed in any order. In the third line print the indexes of points lying at the vertexes of a rectangle in the similar format. All printed numbers should be pairwise distinct.</p><p>If the required partition does not exist, the first line should contain the word "<span class="tex-font-style-tt">NO</span>" (without the quotes), after which no output is needed.</p></div>


## Input

<p>You are given 8 pairs of integers, a pair per line �� the coordinates of the points Petya has. The absolute value of all coordinates does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>. It is guaranteed that no two points coincide.</p>


## Output

<p>Print in the first output line "<span class="tex-font-style-tt">YES</span>" (without the quotes), if the desired partition exists. In the second line output 4 space-separated numbers �� point indexes from the input, which lie at the vertexes of the square. The points are numbered starting from 1. The numbers can be printed in any order. In the third line print the indexes of points lying at the vertexes of a rectangle in the similar format. All printed numbers should be pairwise distinct.</p><p>If the required partition does not exist, the first line should contain the word "<span class="tex-font-style-tt">NO</span>" (without the quotes), after which no output is needed.</p>


## Samples

```input1
0 0
10 11
10 0
0 11
1 1
2 2
2 1
1 2

```

```output1
YES
5 6 7 8
1 2 3 4

```






```input2
0 0
1 1
2 2
3 3
4 4
5 5
6 6
7 7

```

```output2
NO

```






```input3
0 0
4 4
4 0
0 4
1 2
2 3
3 2
2 1

```

```output3
YES
1 2 3 4
5 6 7 8

```




## Note

<p>Pay attention to the third example: the figures do not necessarily have to be parallel to the coordinate axes.</p>

