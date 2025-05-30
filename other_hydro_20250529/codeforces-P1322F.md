## Description

<div><p>Mayor of city M. decided to launch several new metro lines during 2020. Since the city has a very limited budget, it was decided not to dig new tunnels but to use the existing underground network.</p><p>The tunnel system of the city M. consists of $n$ metro stations. The stations are connected with $n - 1$ bidirectional tunnels. Between every two stations $v$ and $u$ there is exactly one simple path. Each metro line the mayor wants to create is a simple path between stations $a_i$ and $b_i$. Metro lines can intersects freely, that is, they can share common stations or even common tunnels. However, it's not yet decided which of two directions each line will go. More precisely, between the stations $a_i$ and $b_i$ the trains will go either from $a_i$ to $b_i$, or from $b_i$ to $a_i$, but not simultaneously.</p><p>The city $M$ uses complicated faring rules. Each station is assigned with a positive integer $c_i$&nbsp;！ the fare zone of the station. The cost of travel from $v$ to $u$ is defined as $c_u - c_v$ roubles. Of course, such travel only allowed in case there is a metro line, the trains on which go from $v$ to $u$. Mayor doesn't want to have any travels with a negative cost, so it was decided to assign directions of metro lines and station fare zones in such a way, that fare zones are strictly increasing during any travel on any metro line.</p><p>Mayor wants firstly assign each station a fare zone and then choose a lines direction, such that all fare zones are increasing along any line. In connection with the approaching celebration of the day of the city, the mayor wants to assign fare zones so that the maximum $c_i$ will be as low as possible. Please help mayor to design a new assignment or determine if it's impossible to do. Please note that you only need to assign the fare zones optimally, you don't need to print lines' directions. This way, you solution will be considered correct if there will be a way to assign directions of every metro line, so that the fare zones will be strictly increasing along any movement of the trains.</p></div><div class="input-specification"><p>The first line contains an integers $n$, $m$ ($2 \le n, \le 500\,000,\ 1 \le m \le 500\,000$)&nbsp;！ the number of stations in the city and the number of metro lines.</p><p>Each of the following $n-1$ lines describes another metro tunnel. Each tunnel is described with integers $v_i$, $u_i$ ($1 \le v_i,\ u_i \le n$, $v_i \ne u_i$). It's guaranteed, that there is exactly one simple path between any two stations.</p><p>Each of the following $m$ lines describes another metro line. Each line is described with integers $a_i$, $b_i$ ($1 \le a_i,\ b_i \le n$, $a_i \neq b_i$).</p></div><div class="output-specification"><p>In the first line print integer $k$&nbsp;！ the maximum fare zone used.</p><p>In the next line print integers $c_1, c_2, \ldots, c_n$ ($1 \le c_i \le k$) &nbsp;！ stations' fare zones. </p><p>In case there are several possible answers, print any of them. In case it's impossible to assign fare zones, print "<span class="tex-font-style-tt">-1</span>".</p></div>

## Input

<p>The first line contains an integers $n$, $m$ ($2 \le n, \le 500\,000,\ 1 \le m \le 500\,000$)&nbsp;！ the number of stations in the city and the number of metro lines.</p><p>Each of the following $n-1$ lines describes another metro tunnel. Each tunnel is described with integers $v_i$, $u_i$ ($1 \le v_i,\ u_i \le n$, $v_i \ne u_i$). It's guaranteed, that there is exactly one simple path between any two stations.</p><p>Each of the following $m$ lines describes another metro line. Each line is described with integers $a_i$, $b_i$ ($1 \le a_i,\ b_i \le n$, $a_i \neq b_i$).</p>

## Output

<p>In the first line print integer $k$&nbsp;！ the maximum fare zone used.</p><p>In the next line print integers $c_1, c_2, \ldots, c_n$ ($1 \le c_i \le k$) &nbsp;！ stations' fare zones. </p><p>In case there are several possible answers, print any of them. In case it's impossible to assign fare zones, print "<span class="tex-font-style-tt">-1</span>".</p>

## Samples

```input1
3 1
1 2
2 3
1 3
```

```output1
3
1 2 3
```






```input2
4 3
1 2
1 3
1 4
2 3
2 4
3 4
```

```output2
-1
```






```input3
7 5
3 4
4 2
2 5
5 1
2 6
4 7
1 3
6 7
3 7
2 1
3 6
```

```output3
-1
```




## Note

<p>In the first example, line $1 \rightarrow 3$ goes through the stations 1, 2, 3 in this order. In this order the fare zones of the stations are increasing. Since this line has 3 stations, at least three fare zones are needed. So the answer 1, 2, 3 is optimal.</p><p>In the second example, it's impossible to assign fare zones to be consistent with a metro lines.</p>
