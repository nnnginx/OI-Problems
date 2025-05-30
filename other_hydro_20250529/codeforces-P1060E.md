## Description

<div><p>Sergey Semyonovich is a mayor of a county city N and he used to spend his days and nights in thoughts of further improvements of Nkers' lives. Unfortunately for him, anything and everything has been done already, and there are no more possible improvements he can think of during the day (he now prefers to sleep at night). However, his assistants have found a solution and they now draw an imaginary city on a paper sheet and suggest the mayor can propose its improvements.</p><p>Right now he has a map of some imaginary city with $n$ subway stations. Some stations are directly connected with tunnels in such a way that the whole map is a tree (assistants were short on time and enthusiasm). It means that there exists exactly one simple path between each pair of station. We call a path simple if it uses each tunnel no more than once.</p><p>One of Sergey Semyonovich's favorite quality objectives is the sum of all pairwise distances between every pair of stations. The distance between two stations is the minimum possible number of tunnels on a path between them.</p><p>Sergey Semyonovich decided to add new tunnels to the subway map. In particular, he connected any two stations $u$ and $v$ that were not connected with a direct tunnel but share a common neighbor, i.e. there exists such a station $w$ that the original map has a tunnel between $u$ and $w$ and a tunnel between $w$ and $v$. You are given a task to compute the sum of pairwise distances between all pairs of stations in the new map.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($2 \leq n \leq 200\,000$)&nbsp;�� the number of subway stations in the imaginary city drawn by mayor's assistants. Each of the following $n - 1$ lines contains two integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$, $u_i \ne v_i$), meaning the station with these indices are connected with a direct tunnel.</p><p>It is guaranteed that these $n$ stations and $n - 1$ tunnels form a tree.</p></div><div class="output-specification"><p>Print one integer that is equal to the sum of distances between all pairs of stations after Sergey Semyonovich draws new tunnels between all pairs of stations that share a common neighbor in the original map.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($2 \leq n \leq 200\,000$)&nbsp;�� the number of subway stations in the imaginary city drawn by mayor's assistants. Each of the following $n - 1$ lines contains two integers $u_i$ and $v_i$ ($1 \leq u_i, v_i \leq n$, $u_i \ne v_i$), meaning the station with these indices are connected with a direct tunnel.</p><p>It is guaranteed that these $n$ stations and $n - 1$ tunnels form a tree.</p>

## Output

<p>Print one integer that is equal to the sum of distances between all pairs of stations after Sergey Semyonovich draws new tunnels between all pairs of stations that share a common neighbor in the original map.</p>

## Samples

```input1
4
1 2
1 3
1 4

```

```output1
6

```






```input2
4
1 2
2 3
3 4

```

```output2
7

```




## Note

<p>In the first sample, in the new map all pairs of stations share a direct connection, so the sum of distances is $6$.</p><p>In the second sample, the new map has a direct tunnel between all pairs of stations except for the pair $(1, 4)$. For these two stations the distance is $2$.</p>
