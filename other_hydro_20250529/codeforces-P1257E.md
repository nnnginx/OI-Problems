## Description

<div><p>A team of three programmers is going to play a contest. The contest consists of $n$ problems, numbered from $1$ to $n$. Each problem is printed on a separate sheet of paper. The participants have decided to divide the problem statements into three parts: the first programmer took some prefix of the statements (some number of first paper sheets), the third contestant took some suffix of the statements (some number of last paper sheets), and the second contestant took all remaining problems. But something went wrong ！ the statements were printed in the wrong order, so the contestants have received the problems in some random order.</p><p>The first contestant has received problems $a_{1, 1}, a_{1, 2}, \dots, a_{1, k_1}$. The second one has received problems $a_{2, 1}, a_{2, 2}, \dots, a_{2, k_2}$. The third one has received all remaining problems ($a_{3, 1}, a_{3, 2}, \dots, a_{3, k_3}$).</p><p>The contestants don't want to play the contest before they redistribute the statements. They want to redistribute them so that the first contestant receives some prefix of the problemset, the third contestant receives some suffix of the problemset, and the second contestant receives all the remaining problems.</p><p>During one move, some contestant may give one of their problems to other contestant. What is the minimum number of moves required to redistribute the problems?</p><p><span class="tex-font-style-bf">It is possible that after redistribution some participant (or even two of them) will not have any problems</span>.</p></div><div class="input-specification"><p>The first line contains three integers $k_1, k_2$ and $k_3$ ($1 \le k_1, k_2, k_3 \le 2 \cdot 10^5, k_1 + k_2 + k_3 \le 2 \cdot 10^5$) ！ the number of problems initially taken by the first, the second and the third participant, respectively.</p><p>The second line contains $k_1$ integers $a_{1, 1}, a_{1, 2}, \dots, a_{1, k_1}$ ！ the problems initially taken by the first participant.</p><p>The third line contains $k_2$ integers $a_{2, 1}, a_{2, 2}, \dots, a_{2, k_2}$ ！ the problems initially taken by the second participant.</p><p>The fourth line contains $k_3$ integers $a_{3, 1}, a_{3, 2}, \dots, a_{3, k_3}$ ！ the problems initially taken by the third participant.</p><p>It is guaranteed that no problem has been taken by two (or three) participants, and each integer $a_{i, j}$ meets the condition $1 \le a_{i, j} \le n$, where $n = k_1 + k_2 + k_3$.</p></div><div class="output-specification"><p>Print one integer ！ the minimum number of moves required to redistribute the problems so that the first participant gets the prefix of the problemset, the third participant gets the suffix of the problemset, and the second participant gets all of the remaining problems.</p></div>

## Input

<p>The first line contains three integers $k_1, k_2$ and $k_3$ ($1 \le k_1, k_2, k_3 \le 2 \cdot 10^5, k_1 + k_2 + k_3 \le 2 \cdot 10^5$) ！ the number of problems initially taken by the first, the second and the third participant, respectively.</p><p>The second line contains $k_1$ integers $a_{1, 1}, a_{1, 2}, \dots, a_{1, k_1}$ ！ the problems initially taken by the first participant.</p><p>The third line contains $k_2$ integers $a_{2, 1}, a_{2, 2}, \dots, a_{2, k_2}$ ！ the problems initially taken by the second participant.</p><p>The fourth line contains $k_3$ integers $a_{3, 1}, a_{3, 2}, \dots, a_{3, k_3}$ ！ the problems initially taken by the third participant.</p><p>It is guaranteed that no problem has been taken by two (or three) participants, and each integer $a_{i, j}$ meets the condition $1 \le a_{i, j} \le n$, where $n = k_1 + k_2 + k_3$.</p>

## Output

<p>Print one integer ！ the minimum number of moves required to redistribute the problems so that the first participant gets the prefix of the problemset, the third participant gets the suffix of the problemset, and the second participant gets all of the remaining problems.</p>

## Samples

```input1
2 1 2
3 1
4
2 5
```

```output1
1
```






```input2
3 2 1
3 2 1
5 4
6
```

```output2
0
```






```input3
2 1 3
5 6
4
1 2 3
```

```output3
3
```






```input4
1 5 1
6
5 1 2 4 7
3
```

```output4
2
```




## Note

<p>In the first example the third contestant should give the problem $2$ to the first contestant, so the first contestant has $3$ first problems, the third contestant has $1$ last problem, and the second contestant has $1$ remaining problem.</p><p>In the second example the distribution of problems is already valid: the first contestant has $3$ first problems, the third contestant has $1$ last problem, and the second contestant has $2$ remaining problems.</p><p>The best course of action in the third example is to give all problems to the third contestant.</p><p>The best course of action in the fourth example is to give all problems to the second contestant.</p>
