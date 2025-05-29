## Description

<div><p>You are given an integer $n$. You choose $n$ cells $(x_1,y_1), (x_2,y_2),\dots,(x_n,y_n)$ in the grid $n\times n$ where $1\le x_i\le n$ and $1\le y_i\le n$.</p><p>Let $\mathcal{H}$ be the set of <span class="tex-font-style-bf">distinct</span> Manhattan distances between any pair of cells. Your task is to maximize the size of $\mathcal{H}$. Examples of sets and their construction are given in the notes.</p><p><span class="tex-font-style-bf">If there exists more than one solution, you are allowed to output any.</span></p><p>Manhattan distance between cells $(x_1,y_1)$ and $(x_2,y_2)$ equals $|x_1-x_2|+|y_1-y_2|$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 50$)&nbsp;¡ª the number of test cases.</p><p>Each of the following $t$ lines contains a single integer $n$ ($2\le n\le 10^3$).</p></div><div class="output-specification"><p>For each test case, output $n$ points which maximize the size of $\mathcal{H}$. It is not necessary to output an empty line at the end of the answer for each test case.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 50$)&nbsp;¡ª the number of test cases.</p><p>Each of the following $t$ lines contains a single integer $n$ ($2\le n\le 10^3$).</p>

## Output

<p>For each test case, output $n$ points which maximize the size of $\mathcal{H}$. It is not necessary to output an empty line at the end of the answer for each test case.</p>





```input1|2,4,6
5
2
3
4
5
6
```




```output1
1 1
1 2

2 1
2 3
3 1

1 1
1 3
4 3
4 4

1 1
1 3
1 4
2 1
5 5

1 4
1 5
1 6
5 2
5 5
6 1
```



## Note

<p>In the first testcase we have $n=2$. One of the possible arrangements is: </p><center> <img class="tex-graphics" src="./34621/file/iTwA10Bs.png" style="max-width: 100.0%;max-height: 100.0%;">  <span class="tex-font-size-small">The arrangement with cells located in $(1,1)$ and $(1,2)$.</span> </center> In this case $\mathcal{H}=\{|1-1|+|1-1|,|1-1|+|2-2|,|1-1|+|1-2|\}=\{0,0,1\}=\{0,1\}$. Hence, the size of $\mathcal{H}$ is $2$. It can be shown that it is the greatest possible answer.<p>In the second testcase we have $n=3$. The optimal arrangement is: </p><center> <img class="tex-graphics" src="./34621/file/BdtBL95e.png" style="max-width: 100.0%;max-height: 100.0%;">  <span class="tex-font-size-small">The arrangement with cells located in $(2,1)$, $(2,3)$ and $(3,1)$.</span> </center><p>$\mathcal{H}$=$\{|2-2|+|1-1|,|2-2|+|3-3|,|3-3|+|1-1|,|2-2|+|1-3|,|2-3|+|1-1|,|2-3|+|3-1|\}$=$\{0,0,0,2,1,3\}$=$\{0,1,2,3\}$.</p><p>For $n=4$ a possible arrangement is: </p><center> <img class="tex-graphics" src="./34621/file/5yxYm8ua.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For $n=5$ a possible arrangement is: </p><center> <img class="tex-graphics" src="./34621/file/bhp8pYsw.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For $n=6$ a possible arrangement is: </p><center> <img class="tex-graphics" src="./34621/file/u4DBby95.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
