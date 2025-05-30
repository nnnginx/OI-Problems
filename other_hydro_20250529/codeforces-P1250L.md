## Description

<div><p>A group of students has recently been admitted to the Faculty of Computer Sciences at the Berland State University. Now the programming teacher wants to divide them into three subgroups for practice sessions.</p><p>The teacher knows that a lot of programmers argue which language is the best. The teacher doesn't want to hear any arguments in the subgroups, so she wants to divide the students into three subgroups so that no pair of students belonging to the same subgroup want to argue.</p><p>To perform this division, the teacher asked each student which programming language he likes. There are $a$ students who answered that they enjoy Assembler, $b$ students stated that their favourite language is Basic, and $c$ remaining students claimed that C++ is the best programming language ！ and there was a large argument between Assembler fans and C++ fans.</p><p>Now, knowing that Assembler programmers and C++ programmers can start an argument every minute, the teacher wants to divide the students into three subgroups so that every student belongs to exactly one subgroup, and there is no subgroup that contains at least one Assembler fan and at least one C++ fan. Since teaching a lot of students can be difficult, the teacher wants the size of the largest subgroup to be minimum possible.</p><p>Please help the teacher to calculate the minimum possible size of the largest subgroup!</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 5$) ！ the number of test cases in the input. Then test cases follow.</p><p>Each test case consists of one line containing three integers $a$, $b$ and $c$ ($1 \le a, b, c \le 1000$) ！ the number of Assembler fans, Basic fans and C++ fans, respectively.</p></div><div class="output-specification"><p>For each test case print one integer ！ the minimum size of the largest subgroup if the students are divided in such a way that there is no subgroup that contains at least one Assembler fan and at least one C++ fan simultaneously.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 5$) ！ the number of test cases in the input. Then test cases follow.</p><p>Each test case consists of one line containing three integers $a$, $b$ and $c$ ($1 \le a, b, c \le 1000$) ！ the number of Assembler fans, Basic fans and C++ fans, respectively.</p>

## Output

<p>For each test case print one integer ！ the minimum size of the largest subgroup if the students are divided in such a way that there is no subgroup that contains at least one Assembler fan and at least one C++ fan simultaneously.</p>

## Samples

```input1
5
3 5 7
4 8 4
13 10 13
1000 1000 1000
13 22 7
```

```output1
5
6
13
1000
14
```






```input2
5
1 3 4
1000 1000 1
4 1 2
325 226 999
939 861 505
```

```output2
3
667
3
517
769
```




## Note

<p>Explanation of the answers for the example $1$:</p><ol><li> The first subgroup contains $3$ Assembler fans and $2$ Basic fans, the second subgroup ！ $5$ C++ fans, the third subgroup ！ $2$ C++ fans and $3$ Basic fans. </li><li> The first subgroup contains $4$ Assembler fans, the second subgroup ！ $6$ Basic fans, the third subgroup ！ $2$ Basic fans and $4$ C++ fans. </li><li> The first subgroup contains all Assembler fans, the second subgroup ！ all Basic fans, the third subgroup ！ all C++ fans. </li><li> The first subgroup contains all Assembler fans, the second subgroup ！ all Basic fans, the third subgroup ！ all C++ fans. </li><li> The first subgroup contains $12$ Assembler fans and $2$ Basic fans, the second subgroup ！ $1$ Assembler fan and $13$ Basic fans, the third subgroup ！ $7$ Basic fans and $7$ C++ fans. </li></ol>
