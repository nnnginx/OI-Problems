## Description

<div><p>In some social network, there are $n$ users communicating with each other in $m$ groups of friends. Let's analyze the process of distributing some news between users.</p><p>Initially, some user $x$ receives the news from some source. Then he or she sends the news to his or her friends (two users are friends if there is at least one group such that both of them belong to this group). Friends continue sending the news to their friends, and so on. The process ends when there is no pair of friends such that one of them knows the news, and another one doesn't know.</p><p>For each user $x$ you have to determine what is the number of users that will know the news if initially only user $x$ starts distributing it. </p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 5 \cdot 10^5$) �� the number of users and the number of groups of friends, respectively.</p><p>Then $m$ lines follow, each describing a group of friends. The $i$-th line begins with integer $k_i$ ($0 \le k_i \le n$) �� the number of users in the $i$-th group. Then $k_i$ <span class="tex-font-style-bf">distinct</span> integers follow, denoting the users belonging to the $i$-th group.</p><p>It is guaranteed that $\sum \limits_{i = 1}^{m} k_i \le 5 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $n$ integers. The $i$-th integer should be equal to the number of users that will know the news if user $i$ starts distributing it.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 5 \cdot 10^5$) �� the number of users and the number of groups of friends, respectively.</p><p>Then $m$ lines follow, each describing a group of friends. The $i$-th line begins with integer $k_i$ ($0 \le k_i \le n$) �� the number of users in the $i$-th group. Then $k_i$ <span class="tex-font-style-bf">distinct</span> integers follow, denoting the users belonging to the $i$-th group.</p><p>It is guaranteed that $\sum \limits_{i = 1}^{m} k_i \le 5 \cdot 10^5$.</p>

## Output

<p>Print $n$ integers. The $i$-th integer should be equal to the number of users that will know the news if user $i$ starts distributing it.</p>

## Samples

```input1
7 5
3 2 5 4
0
2 1 2
1 1
2 6 7
```

```output1
4 4 1 4 4 2 2
```



