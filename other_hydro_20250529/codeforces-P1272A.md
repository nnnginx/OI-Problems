## Description

<div><p>Three friends are going to meet each other. Initially, the first friend stays at the position $x = a$, the second friend stays at the position $x = b$ and the third friend stays at the position $x = c$ on the coordinate axis $Ox$.</p><p>In one minute <span class="tex-font-style-bf">each friend independently</span> from other friends can change the position $x$ by $1$ to the left or by $1$ to the right (i.e. set $x := x - 1$ or $x := x + 1$) or even don't change it.</p><p>Let's introduce the total pairwise distance ！ the sum of distances between each pair of friends. Let $a'$, $b'$ and $c'$ be the final positions of the first, the second and the third friend, correspondingly. Then the total pairwise distance is $|a' - b'| + |a' - c'| + |b' - c'|$, where $|x|$ is the absolute value of $x$.</p><p>Friends are interested in the minimum total pairwise distance they can reach if they will move optimally. <span class="tex-font-style-bf">Each friend will move no more than once</span>. So, more formally, they want to know the minimum total pairwise distance they can reach after one minute.</p><p>You have to answer $q$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 1000$) ！ the number of test cases.</p><p>The next $q$ lines describe test cases. The $i$-th test case is given as three integers $a, b$ and $c$ ($1 \le a, b, c \le 10^9$) ！ initial positions of the first, second and third friend correspondingly. The positions of friends can be equal.</p></div><div class="output-specification"><p>For each test case print the answer on it ！ the minimum total pairwise distance (the minimum sum of distances between each pair of friends) if friends change their positions optimally. <span class="tex-font-style-bf">Each friend will move no more than once</span>. So, more formally, you have to find the minimum total pairwise distance they can reach after one minute.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 1000$) ！ the number of test cases.</p><p>The next $q$ lines describe test cases. The $i$-th test case is given as three integers $a, b$ and $c$ ($1 \le a, b, c \le 10^9$) ！ initial positions of the first, second and third friend correspondingly. The positions of friends can be equal.</p>

## Output

<p>For each test case print the answer on it ！ the minimum total pairwise distance (the minimum sum of distances between each pair of friends) if friends change their positions optimally. <span class="tex-font-style-bf">Each friend will move no more than once</span>. So, more formally, you have to find the minimum total pairwise distance they can reach after one minute.</p>

## Samples

```input1
8
3 3 4
10 20 30
5 5 5
2 4 3
1 1000000000 1000000000
1 1000000000 999999999
3 2 5
3 2 6
```

```output1
0
36
0
0
1999999994
1999999994
2
4
```



