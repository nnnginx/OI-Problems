## ��Ŀ����
There was an ICPC contest two thousand years ago in the Qin dynasty. There were $m$ problems and $n$ teams in the contest. We only know how many problems each team solved and how much total time they used from the historical records. These are called the $\textbf{final result}$s of the teams. We don't know which problems they solved or their submission times.

Recently, we seem to had a discovery. We found the $\textbf{frozen scoreboard}$ of the teams. From the frozen scoreboard of a team, we know their submissions during the whole contest, but we don't know the verdicts of the submissions in the last hour. And some people found that for some teams, their frozen scoreboards may contradict their final results in the historical records.

Given the final results and the frozen scoreboards of the teams, please construct a $\textbf{final scoreboard}$ for each team that is consistent with both its final result and its frozen scoreboard.

From the submissions during the contest, we can calculate the final scoreboard and the final result as follows:

For a fixed team $i$, its $\textbf{final scoreboard}$ is an array of $m$ elements where the $j$-th element shows some information about team $i$'s submissions on problem $j$. 

- If team $i$ didn't submit to problem $j$, the cell should be a single character ``.`` (without quotes). 

- If team $i$ submitted $x$ times to problem $j$ and none of the submissions was accepted, the cell should contain $-\ x$. 

- Otherwise, consider all submissions from team $i$ to problem $j$. Each submission has a submission time. Suppose the earliest accepted submission is the $x$-th one. Then the cell should contain $+\ x/y$ where $y~(0\le y\le 299)$ is the submission time of the $x$-th submission. $y$ is an integer representing the submission time in minutes.

Note that in the final scoreboard, we don't care about submissions after the first accepted one. It is possible that two or more submissions happened in the same minute.

The $\textbf{final result}$ of a team is computed from its $\textbf{final scoreboard}$. For each team, we can calculate the number of problems it solved. This number is equal to the number of ``+`` in the team's final scoreboard.

We can also calculate its total time. If team $i$ solved problem $j$ in the $y$-th minute after $x-1$ unaccepted submissions (in other words, the $j$-th cell of its final scoreboard is $+\ x/y$), problem $j$ contributes $20(x-1)+y$ time to team $i$. If team $i$ didn't solve problem $j$, problem $j$ contributes $0$ time to team $i$, no matter team $i$ submitted to problem $j$ or not. The total time of team $i$ is the sum of contributions of each problem.

The rules for the $\textbf{frozen scoreboard}$ will be introduced in the input section. We will distinguish submissions in the final hour and other submissions. A submission was in the final hour if its submission time is between $240$ and $299$.

## �����ʽ
The first line contains two integers $n, m~(1\le n\le 1000, 1\le m\le 13)$, the number of teams in the contest, and the number of problems in the contest.

Then there are $n$ blocks describing the $\textbf{final result}$ and the $\textbf{frozen scoreboard}$ of each team.

The $i$-th block represents team $i$. In the $i$-th block, the first line contains two integers $a_i, b_i~(0\le a_i\le m, 0\le b_i\le 10^5)$, the number of problems team $i$ solved $\textbf{during the whole contest}$ and the total time of team $i$ for solving the $a_i$ problems. These two numbers represent the final result of the contest. The next $m$ lines describe the status of team $i$ in the frozen scoreboard. For each $1\le j\le m$, 

- If the $j$-th line is $+\ x/y$ $(1\le x\le 100, 0\le y\le 239)$, team $i$ solved problem $j$ at time $y$ and the accepted solution is their $x$-th submission on problem $j$.
- If the $j$-th line is $?\ x\ y$ $(1\leq x \leq y \leq 100)$, team $i$ didn't solve the problem $j$ in the first four hours. Team $i$ submitted problem $j$ for $y$ times in which $x$ submissions are in the last hour. Note that submissions made in the last hour after the accepted one will count in the $\textbf{frozen scoreboard}$, but not in the $\textbf{final scoreboard}$.
- If the $j$-th line is $-\ x$, team $i$ didn't solve the problem $j$ in the first four hours. Team $i$ submitted problem $j$ for $x~(1\le x\le 100)$ times before the last hour and did not submit problem $j$ in the last hour.
- If the $j$-th line is a single character ``.`` (without quotes), team $i$ didn't submit problem $j$ at all.

## �����ʽ
For each team $i$, if its final result contradicts its frozen scoreboard, output $\texttt{No}$ in one line. Otherwise, output $\texttt{Yes}$ in the first line and then output $m$ lines, describing a final scoreboard that is consistent with both the final result and the frozen scoreboard of team $i$. The $j$-th line should contain 

- $+\ x/y$ $(1\le x \le 100, 0\le y \le 299)$, if the $x$-th submission from team $i$ to problem $j$ is accepted and is in the $y$-th minute of the contest. All submissions from team $i$ to team $j$ before the $x$-th one was not accepted. Please don't output extra spaces before and after slash ``/``. 
- $-\ x$ $(1\le x\le 100)$, if team $i$ submitted to problem $j$ for $x$ times and none of the submissions was accepted.
- $.$ if team $i$ didn't submit to problem $j$ at all. 

If there are multiple solutions, output any.

$\textbf{Please note that in the input and the output, there is always a space following each ?, +, and -.}$

## ��Ŀ����
### ��Ŀ����

2000 ����ǰ���س������ٰ��һ�� ICPC �������������� $m$ ���⣬$n$ ���Ŷӡ�����֪��ÿ��������˶��ٵ����Լ�����ʷ��¼������ʱ����Щ�������ŶӵĽ�����������ǲ�֪������ÿ�����Ƿ���ɡ���ʱ��á�

��������Ƿ�����ÿ����**����ļƷְ�**���ӸüƷְ��ϣ����ǿ��Կ���ÿ�����ڱ����е��ύ��������ǲ�֪�������һСʱ���ύ���з֡�һЩ�˷��֣�����һЩ����˵�����Ƕ���ļƷְ��������������ʷ��¼�е����ճɼ���ì�ܡ�

��������յ÷ֺͶ���ļƷְ壬Ϊ���Ӵ���һ���������ս���Ͷ���ļƷְ�һ�µ����ռƷְ塣

�������¹���������Ʒְ���ܷ֣�

���ڸ����Ķ��� $i$����**���յļƷְ�**��һ�� $m$ Ԫ���飬���е� $j$ ��Ԫ�ظ������� $i$ �ڵ� $j$ ���ϵ��ύ��Ϣ��

- ������� $i$ û���ύ���� $j$����� ```.```��

- ������� $i$ ������ $j$ �ύ�� $x$ �ε���δͨ������� $-x$��

- ���򣬿��Ƕ��� $i$ ������ $j$ ��������������ÿ���ύ����һ���ύʱ�䣬���һ��ͨ���������ǵ� $x$ �����⣬�ڵ� $y$ ����ʱ�ύ����� $+x/y$������ $0\leq y\leq299$��

�����ռƷְ��ϣ�ֻ���ǵ�һ��ͨ�����ύ��ͬһ�����ڿ����ж���ύ��

һ����������յ÷��Ǹö�������˶��ٵ��⣬���ö����ռƷְ��� ```+``` �ĸ�����

һ����������ʱ�����·�ʽ���㡣������� $i$ �ڵ� $y$ ��������˵� $j$ ���⣬�����ǰ�� $x-1$ ��ʧ�ܵ��ύ�������ռƷְ��ϵ� $j$ ���������Ϊ $+x/y$�������������ʱ��Ϊ $20(x-1)+y$�� ������� $i$ û����ɵ� $j$ ���⣬���������ʱ��Ϊ $0$�������Ƿ��ύ�������� $i$ ����ʱ����ÿ������ʱ���ܺ͡�

### �����ʽ

��һ�а����������� $n,m\;(1\leq n\leq1000,1\leq m\leq13)$��Ϊ�����������Ŀ������

������ $n$ �飬����ÿ����������յ÷ֺͶ���ļƷְ塣

�� $i$ ���ʾ���� $i$��ÿһ���У���һ�а����������� $a_i,b_i\;(0\leq a_i\leq m,0\leq b_i\leq10^5)$��Ϊ���� $i$ ��**����������**��ɵ���Ŀ������ÿ�������ʱ�������������Ǳ��������ս����

������ $m$ �У��������� $i$ �ڼƷְ��ϵ����ݡ��������� $1\leq j\leq m$��

- ����� $j$ ���� $+\,x/y\;(1\leq x\leq100,0\leq y\leq239)$����ʾ���� $i$ �ڵ� $y$ ���ӣ��� $x$ ���ύʱͨ������ $j$��

- ����� $j$ ���� $?\,x\,y\;(1\leq x\leq y\leq100)$����ʾ���� $i$ û����ǰ�ĸ�Сʱ�������� $j$����������ύ�� $y$ �Σ����� $x$ �������һСʱ�ڡ����һСʱ����ͨ��������ύ��¼����**����ļƷְ�**����ʾ����������**���ռƷְ�**����ʾ��

- ����� $j$ ���� $-x$����ʾ���� $i$ û����ǰ��Сʱ�������� $j$��������������һ��Сʱǰ�ύ�� $x\,(1\leq x\leq100)$ �Σ���û�������һСʱ�������� $j$��

- ����� $j$ ����һ����һ���ַ� ```.```����ʾ���� $i$ û���ύ���� $j$��

### �����ʽ

����ÿ������ $i$��������ս���Ͷ���ļƷְ���ì�ܣ����һ�� $\texttt{No}$�����򣬵�һ����� $\texttt{Yes}$�������� $m$ �У�����һ�ֶ��� $i$ ���ܵļƷְ壬�������ս���Ͷ���ļƷְ塣���У��� $j$ ��Ӧ�ð�����

- $+\,x/y\,(1\leq x\leq100,0\leq y\leq299)$��������� $i$ �ڵ� $x$ ���ύ���� $y$ ����������� $j$������֮ǰû�ж���ͨ������⡣��Ҫ���ַ� ```/``` ǰ���������Ŀո�

- $-x\,(1\leq x\leq100)$��������� $i$ �ύ�� $x$ ���� $j$���Ҿ�δͨ����

- ```.```��������� $i$ û���ύ�� $j$��

����ж��ֿ��ܵĴ𰸣��������һ�ּ��ɡ�

**��ע�⣬�����������У�```?,+,-``` ������һ���ո�**

```input1
1 13
7 951
+ 1/6
? 3 4
+ 4/183
- 2
+ 3/217
.
.
.
+ 2/29
+ 1/91
.
+ 1/22
.
```

```output1
Yes
+ 1/6
+ 2/263
+ 4/183
- 2
+ 3/217
.
.
.
+ 2/29
+ 1/91
.
+ 1/22
.
```

```input2
6 2
1 100
.
? 3 4
2 100
+ 1/1
+ 1/2
0 0
- 5
- 6
2 480
? 100 100
? 100 100
2 480
? 99 100
? 100 100
1 2000
? 100 100
? 100 100
```

```output2
No
No
Yes
- 5
- 6
Yes
+ 1/240
+ 1/240
No
Yes
+ 87/280
- 100
```

## ��ʾ
Here is an example of the frozen scoreboard in the first sample.

![](https://cdn.luogu.com.cn/upload/image_hosting/jw4c3965.png)

