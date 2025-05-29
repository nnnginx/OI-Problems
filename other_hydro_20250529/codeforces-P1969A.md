## Description

<div><p>Monocarp wants to throw a party. He has $n$ friends, and he wants to have at least $2$ of them at his party.</p><p>The $i$-th friend's best friend is $p_i$. All $p_i$ are distinct, and for every $i \in [1, n]$, $p_i \ne i$.</p><p>Monocarp can send invitations to friends. The $i$-th friend comes to the party if <span class="tex-font-style-bf">both the $i$-th friend and the $p_i$-th friend</span> receive an invitation (note that the $p_i$-th friend doesn't have to actually come to the party). Each invitation is sent to exactly one of the friends.</p><p>For example, if $p = [3, 1, 2, 5, 4]$, and Monocarp sends invitations to the friends $[1, 2, 4, 5]$, then the friends $[2, 4, 5]$ will come to the party. The friend $1$ won't come since his best friend didn't receive an invitation; the friend $3$ won't come since he didn't receive an invitation.</p><p>Calculate the minimum number of invitations Monocarp has to send so that <span class="tex-font-style-bf">at least $2$</span> friends come to the party.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 5000$)&nbsp;！ the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains one integer $n$ ($2 \le n \le 50$)&nbsp;！ the number of friends; </li><li> the second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$; $p_i \ne i$; all $p_i$ are distinct). </li></ul></div><div class="output-specification"><p>Print one integer&nbsp;！ the minimum number of invitations Monocarp has to send.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 5000$)&nbsp;！ the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains one integer $n$ ($2 \le n \le 50$)&nbsp;！ the number of friends; </li><li> the second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$; $p_i \ne i$; all $p_i$ are distinct). </li></ul>

## Output

<p>Print one integer&nbsp;！ the minimum number of invitations Monocarp has to send.</p>





```input1|2,3,6,7
3
5
3 1 2 5 4
4
2 3 4 1
2
2 1
```




```output1
2
3
2
```



## Note

<p>In the first testcase, Monocarp can send invitations to friends $4$ and $5$. Both of them will come to the party since they are each other's best friends, and both of them have invitations.</p><p>In the second testcase, Monocarp can send invitations to friends $1, 2$ and $3$, for example. Then friends $1$ and $2$ will attend: friend $1$ and his best friend $2$ have invitations, friend $2$ and his best friend $3$ have invitations. Friend $3$ won't attend since his friend $4$ doesn't have an invitation. It's impossible to send invitations to fewer than $3$ friends in such a way that at least $2$ come.</p><p>In the third testcase, Monocarp can send invitations to both friends $1$ and $2$, and both of them will attend.</p>
