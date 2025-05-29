## Description

<div><p>You are given two rooted trees, consisting of $n$ vertices each. The vertices in the trees are numbered from $1$ to $n$, and the root is the vertex $1$.</p><p>You can perform the following operation: choose the tree and the vertex $v$ (except the root of the tree) in it; connect the child nodes of $v$ to the parent of $v$ and remove $v$ from the tree.</p><p>Let's say that two trees are equal if both of the following conditions hold: </p><ul> <li> the sets of remaining vertices in both trees are the same; </li><li> for every vertex $v$ which is not deleted, its parent in the first tree is the same as its parent in the second tree. </li></ul><p>Your task is to calculate the minimum number of aforementioned operation in order to make the trees equal.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 40$)&nbsp;！ the number of vertices in the trees.</p><p>The second line contains $n-1$ integers $a_2, a_3, \dots, a_n$ ($1 \le a_i \le n$), where $a_i$ the parent of the $i$-th vertex in the first tree. Vertex $1$ is the root.</p><p>The third line contains $n-1$ integers $b_2, b_3, \dots, b_n$ ($1 \le b_i \le n$), where $b_i$ the parent of the $i$-th vertex in the second tree. Vertex $1$ is the root.</p></div><div class="output-specification"><p>Print a single integer&nbsp;！ the minimum number of aforementioned operation in order to make the trees equal.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 40$)&nbsp;！ the number of vertices in the trees.</p><p>The second line contains $n-1$ integers $a_2, a_3, \dots, a_n$ ($1 \le a_i \le n$), where $a_i$ the parent of the $i$-th vertex in the first tree. Vertex $1$ is the root.</p><p>The third line contains $n-1$ integers $b_2, b_3, \dots, b_n$ ($1 \le b_i \le n$), where $b_i$ the parent of the $i$-th vertex in the second tree. Vertex $1$ is the root.</p>

## Output

<p>Print a single integer&nbsp;！ the minimum number of aforementioned operation in order to make the trees equal.</p>





```input1|
5
1 5 5 1
1 4 1 2
```




```input2|
2
1
1
```




```input3|
10
4 7 10 6 2 9 7 1 1
1 2 10 3 4 6 6 5 5
```




```output1
4
```




```output2
0
```




```output3
10
```


