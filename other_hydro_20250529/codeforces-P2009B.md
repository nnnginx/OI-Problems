## Description

<div><p>You are playing your favorite rhythm game, osu!mania. The layout of your beatmap consists of $n$ rows and $4$ columns. Because notes at the bottom are closer, you will process the bottommost row first and the topmost row last. Each row will contain exactly one note, represented as a '#'.</p><p>For each note $1, 2, \dots, n$, in the order of processing, output the column in which the note appears.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 100$) ！ the number of test cases.</p><p>For each test case, the first line contains $n$ ($1 \leq n \leq 500$) ！ the number of rows of the beatmap.</p><p>The following $n$ lines contain $4$ characters. The $i$-th line represents the $i$-th row of the beatmap from the top. It is guaranteed that the characters are either '.' or '#', and exactly one of the characters is '#'. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $500$.</p></div><div class="output-specification"><p>For each test case, output $n$ integers on a new line, the column that the $i$-th note appears in for all $i$ from $1$ to $n$.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 100$) ！ the number of test cases.</p><p>For each test case, the first line contains $n$ ($1 \leq n \leq 500$) ！ the number of rows of the beatmap.</p><p>The following $n$ lines contain $4$ characters. The $i$-th line represents the $i$-th row of the beatmap from the top. It is guaranteed that the characters are either '.' or '#', and exactly one of the characters is '#'. </p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $500$.</p>

## Output

<p>For each test case, output $n$ integers on a new line, the column that the $i$-th note appears in for all $i$ from $1$ to $n$.</p>





```input1|2,3,4,5,6,10,11
3
4
#...
.#..
..#.
...#
2
.#..
.#..
1
...#
```




```output1
4 3 2 1 
2 2 
4
```


