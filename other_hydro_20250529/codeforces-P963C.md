## Description

<div><p>A rectangle with sides $A$ and $B$ is cut into rectangles with cuts parallel to its sides. For example, if $p$ horizontal and $q$ vertical cuts were made, $(p + 1) \cdot (q + 1)$ rectangles were left after the cutting. After the cutting, rectangles were of $n$ different types. Two rectangles are different if at least one side of one rectangle isn't equal to the corresponding side of the other. Note that the rectangle can't be rotated, this means that rectangles $a \times b$ and $b \times a$ are considered different if $a \neq b$.</p><p>For each type of rectangles, lengths of the sides of rectangles are given along with the amount of the rectangles of this type that were left after cutting the initial rectangle.</p><p>Calculate the amount of pairs $(A; B)$ such as the given rectangles could be created by cutting the rectangle with sides of lengths $A$ and $B$. Note that pairs $(A; B)$ and $(B; A)$ are considered different when $A \neq B$.</p></div><div class="input-specification"><p>The first line consists of a single integer $n$ ($1 \leq n \leq 2 \cdot 10^{5}$)&nbsp;！ amount of different types of rectangles left after cutting the initial rectangle.</p><p>The next $n$ lines each consist of three integers $w_{i}, h_{i}, c_{i}$ $(1 \leq w_{i}, h_{i}, c_{i} \leq 10^{12})$&nbsp;！ the lengths of the sides of the rectangles of this type and the amount of the rectangles of this type.</p><p>It is guaranteed that the rectangles of the different types are different.</p></div><div class="output-specification"><p>Output one integer&nbsp;！ the answer to the problem.</p></div>

## Input

<p>The first line consists of a single integer $n$ ($1 \leq n \leq 2 \cdot 10^{5}$)&nbsp;！ amount of different types of rectangles left after cutting the initial rectangle.</p><p>The next $n$ lines each consist of three integers $w_{i}, h_{i}, c_{i}$ $(1 \leq w_{i}, h_{i}, c_{i} \leq 10^{12})$&nbsp;！ the lengths of the sides of the rectangles of this type and the amount of the rectangles of this type.</p><p>It is guaranteed that the rectangles of the different types are different.</p>

## Output

<p>Output one integer&nbsp;！ the answer to the problem.</p>

## Samples

```input1
1
1 1 9

```

```output1
3

```






```input2
2
2 3 20
2 4 40

```

```output2
6

```






```input3
2
1 2 5
2 3 5

```

```output3
0

```




## Note

<p>In the first sample there are three suitable pairs: $(1; 9)$, $(3; 3)$ and $(9; 1)$.</p><p>In the second sample case there are 6 suitable pairs: $(2; 220)$, $(4; 110)$, $(8; 55)$, $(10; 44)$, $(20; 22)$ and $(40; 11)$.</p><p>Here the sample of cut for $(20; 22)$.</p><center> <img class="tex-graphics" src="./29216/file/KxmxAvnP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The third sample has no suitable pairs.</p>
