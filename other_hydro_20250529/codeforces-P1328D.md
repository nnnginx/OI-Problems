## Description

<div><p>The round carousel consists of $n$ figures of animals. Figures are numbered from $1$ to $n$ in order of the carousel moving. Thus, after the $n$-th figure the figure with the number $1$ follows. Each figure has its own type ！ the type of the animal corresponding to this figure (the horse, the tiger and so on). The type of animal of the $i$-th figure equals $t_i$.</p><center> <img class="tex-graphics" src="./31002/file/YeCpYSTW.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The example of the carousel for $n=9$ and $t=[5, 5, 1, 15, 1, 5, 5, 1, 1]$</span>. </center><p>You want to color each figure in one of the colors. You think that it's boring if the carousel contains two different figures (with the distinct types of animals) going one right after another and colored in the same color.</p><p>Your task is to color the figures in such a way that the number of distinct colors used is the minimum possible and there are no figures of the different types going one right after another and colored in the same color. If you use exactly $k$ distinct colors, then the colors of figures should be denoted with integers from $1$ to $k$.</p></div><div class="input-specification"><p>The input contains one or more test cases.</p><p>The first line contains one integer $q$ ($1 \le q \le 10^4$) ！ the number of test cases in the test. Then $q$ test cases follow. One test case is given on two lines.</p><p>The first line of the test case contains one integer $n$ ($3 \le n \le 2 \cdot 10^5$) ！ the number of figures in the carousel. Figures are numbered from $1$ to $n$ in order of carousel moving. Assume that after the $n$-th figure the figure $1$ goes.</p><p>The second line of the test case contains $n$ integers $t_1, t_2, \dots, t_n$ ($1 \le t_i \le 2 \cdot 10^5$), where $t_i$ is the type of the animal of the $i$-th figure.</p><p>The sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>Print $q$ answers, for each test case print two lines.</p><p>In the first line print one integer $k$ ！ the minimum possible number of distinct colors of figures.</p><p>In the second line print $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le k$), where $c_i$ is the color of the $i$-th figure. If there are several answers, you can print any.</p></div>

## Input

<p>The input contains one or more test cases.</p><p>The first line contains one integer $q$ ($1 \le q \le 10^4$) ！ the number of test cases in the test. Then $q$ test cases follow. One test case is given on two lines.</p><p>The first line of the test case contains one integer $n$ ($3 \le n \le 2 \cdot 10^5$) ！ the number of figures in the carousel. Figures are numbered from $1$ to $n$ in order of carousel moving. Assume that after the $n$-th figure the figure $1$ goes.</p><p>The second line of the test case contains $n$ integers $t_1, t_2, \dots, t_n$ ($1 \le t_i \le 2 \cdot 10^5$), where $t_i$ is the type of the animal of the $i$-th figure.</p><p>The sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>Print $q$ answers, for each test case print two lines.</p><p>In the first line print one integer $k$ ！ the minimum possible number of distinct colors of figures.</p><p>In the second line print $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le k$), where $c_i$ is the color of the $i$-th figure. If there are several answers, you can print any.</p>

## Samples

```input1
4
5
1 2 1 2 2
6
1 2 2 1 2 2
5
1 2 1 2 3
3
10 10 10
```

```output1
2
1 2 1 2 2
2
2 1 2 1 2 1
3
2 3 2 3 1
1
1 1 1
```



