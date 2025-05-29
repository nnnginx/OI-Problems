## Description

<div><p>Monocarp plays a fantasy RPG. His character is a mage, so he casts spells. There are two types of spells he knows ！ basic spells and composite spells.</p><p>There are $n$ basic spells in Monocarp's spell book, numbered from $1$ to $n$. Each basic spell simply changes the health of the target: either decreases it or increases it. The $i$-th basic spell changes the target's health value by $b_i$ (increases by $b_i$ if $b_i$ is non-negative, or decreases by $|b_i|$ if $b_i$ is negative). If the target's health value goes to $0$ or below, it dies, and all next spells cast at it do nothing.</p><p>There are also $m$ composite spells in the spell book, numbered from $n+1$ to $n+m$. Each composite spell is a sequence of other spells, cast in specific order. A composite spell can consist both of basic spells and composite spells; the $i$-th spell consists of $s_i$ other spells, and each of those spells has index strictly less than $i$ (so there is no situation that composite spells infinitely cast each other). So, actually, each composite spell can be considered a finite sequence of basic spells, although its length might be huge. Note that the same spell can appear in a composite spell multiple times.</p><p>Monocarp has decided to cast the $(n+m)$-th spell from his spell book. The target of this spell is a monster with an initial health value of $hp$. Monocarp wants to know whether the monster will be killed or not, and if it will be killed, which basic spell will kill it.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>Each test case is given as follows:</p><ul> <li> the first line contains two integers $n$ and $hp$ ($1 \le n \le 5000$; $1 \le hp \le 10^{9}$) ！ the number of basic spells and the initial health value of the monster; </li><li> the second line contains $n$ integers $b_1, b_2, \dots, b_n$ ($-10^9 \le b_i \le 10^9$) ！ the descriptions of basic spells; </li><li> the third line contains one integer $m$ ($1 \le m \le 5000$) ！ the number of composite spells; </li><li> then $m$ lines follow, the $i$-th of these lines describes the $(n+i)$-th spell: it begins with an integer $s_{n+i}$ ($1 \le s_{n+i} \le 5000$) denoting the length of the spell (the number of spells it consists of); then a sequence of integers from $1$ to $(n+i-1)$ follows, denoting the sequence of spells. </li></ul><p>Additional constraints on the input: </p><ul> <li> the sum of $n$ over all test cases does not exceed $5000$; </li><li> the sum of $m$ over all test cases does not exceed $5000$; </li><li> the total length of all composite spells over all test cases does not exceed $5000$. </li></ul></div><div class="output-specification"><p>For each test case, print one integer:</p><ul> <li> if the monster dies, print the index of the basic spell that kills the monster; </li><li> otherwise, print $-1$. </li></ul></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>Each test case is given as follows:</p><ul> <li> the first line contains two integers $n$ and $hp$ ($1 \le n \le 5000$; $1 \le hp \le 10^{9}$) ！ the number of basic spells and the initial health value of the monster; </li><li> the second line contains $n$ integers $b_1, b_2, \dots, b_n$ ($-10^9 \le b_i \le 10^9$) ！ the descriptions of basic spells; </li><li> the third line contains one integer $m$ ($1 \le m \le 5000$) ！ the number of composite spells; </li><li> then $m$ lines follow, the $i$-th of these lines describes the $(n+i)$-th spell: it begins with an integer $s_{n+i}$ ($1 \le s_{n+i} \le 5000$) denoting the length of the spell (the number of spells it consists of); then a sequence of integers from $1$ to $(n+i-1)$ follows, denoting the sequence of spells. </li></ul><p>Additional constraints on the input: </p><ul> <li> the sum of $n$ over all test cases does not exceed $5000$; </li><li> the sum of $m$ over all test cases does not exceed $5000$; </li><li> the total length of all composite spells over all test cases does not exceed $5000$. </li></ul>

## Output

<p>For each test case, print one integer:</p><ul> <li> if the monster dies, print the index of the basic spell that kills the monster; </li><li> otherwise, print $-1$. </li></ul>





```input1|2,3,4,5,6,7,14,15,16,17
4
4 9
1 -2 3 -4
3
3 1 4 3
4 1 2 1 2
6 6 5 6 5 6 5
4 9
1 -2 3 -4
3
3 1 4 3
4 1 2 1 2
7 6 5 6 5 6 6 5
3 31
-10 -20 30
1
6 1 2 3 1 2 3
6 20
-1 -5 -9 -7 -1 -1
4
3 6 5 2
4 3 3 7 6
6 4 8 4 4 6 7
3 6 5 7
```




```output1
4
4
-1
-1
```


