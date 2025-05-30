## Description

<div><p>Hanh lives in a shared apartment. There are $n$ people (including Hanh) living there, each has a private fridge. </p><p>$n$ fridges are secured by several steel chains. Each steel chain connects two <span class="tex-font-style-bf">different</span> fridges and is protected by a digital lock. The owner of a fridge knows passcodes of all chains connected to it. A fridge can be open only if all chains connected to it are unlocked. For example, if a fridge has no chains connected to it at all, then any of $n$ people can open it.</p><center> <img class="tex-graphics" src="./30659/file/o9O1BvRJ.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">For exampe, in the picture there are $n=4$ people and $5$ chains. The first person knows passcodes of two chains: $1-4$ and $1-2$. The fridge $1$ can be open by its owner (the person $1$), also two people $2$ and $4$ (acting together) can open it.</span> </center><p>The weights of these fridges are $a_1, a_2, \ldots, a_n$. To make a steel chain connecting fridges $u$ and $v$, you have to pay $a_u + a_v$ dollars. Note that the landlord allows you to create <span class="tex-font-style-bf">multiple chains connecting the same pair of fridges</span>. </p><p>Hanh's apartment landlord asks you to create exactly $m$ steel chains so that all fridges are private. A fridge is private if and only if, among $n$ people living in the apartment, only the owner can open it (i.e. no other person acting alone can do it). In other words, the fridge $i$ is not private if there exists the person $j$ ($i \ne j$) that the person $j$ can open the fridge $i$.</p><p>For example, in the picture all the fridges are private. On the other hand, if there are $n=2$ fridges and only one chain (which connects them) then both fridges are not private (both fridges can be open not only by its owner but also by another person).</p><p>Of course, the landlord wants to minimize the total cost of all steel chains to fulfill his request. Determine whether there exists any way to make exactly $m$ chains, and if yes, output any solution that minimizes the total cost. </p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $T$ ($1 \le T \le 10$). Then the descriptions of the test cases follow.</p><p>The first line of each test case contains two integers $n$, $m$ ($2 \le n \le 1000$, $1 \le m \le n$)&nbsp;！ the number of people living in Hanh's apartment and the number of steel chains that the landlord requires, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^4$)&nbsp;！ weights of all fridges.</p></div><div class="output-specification"><p>For each test case:</p><ul> <li> If there is no solution, print a single integer $-1$. </li><li> Otherwise, print a single integer $c$&nbsp;！ the minimum total cost. The $i$-th of the next $m$ lines contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$, $u_i \ne v_i$), meaning that the $i$-th steel chain connects fridges $u_i$ and $v_i$. An arbitrary number of chains can be between a pair of fridges. </li></ul><p>If there are multiple answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $T$ ($1 \le T \le 10$). Then the descriptions of the test cases follow.</p><p>The first line of each test case contains two integers $n$, $m$ ($2 \le n \le 1000$, $1 \le m \le n$)&nbsp;！ the number of people living in Hanh's apartment and the number of steel chains that the landlord requires, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^4$)&nbsp;！ weights of all fridges.</p>

## Output

<p>For each test case:</p><ul> <li> If there is no solution, print a single integer $-1$. </li><li> Otherwise, print a single integer $c$&nbsp;！ the minimum total cost. The $i$-th of the next $m$ lines contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$, $u_i \ne v_i$), meaning that the $i$-th steel chain connects fridges $u_i$ and $v_i$. An arbitrary number of chains can be between a pair of fridges. </li></ul><p>If there are multiple answers, print any.</p>

## Samples

```input1
3
4 4
1 1 1 1
3 1
1 2 3
3 3
1 2 3
```

```output1
8
1 2
4 3
3 2
4 1
-1
12
3 2
1 2
3 1
```



