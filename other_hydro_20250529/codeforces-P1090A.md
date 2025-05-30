## Description

<div><p>A conglomerate consists of $n$ companies. To make managing easier, their owners have decided to merge all companies into one. By law, it is only possible to merge two companies, so the owners plan to select two companies, merge them into one, and continue doing so until there is only one company left.</p><p>But anti-monopoly service forbids to merge companies if they suspect unfriendly absorption. The criterion they use is the difference in maximum salaries between two companies. Merging is allowed only if the maximum salaries are equal.</p><p>To fulfill the anti-monopoly requirements, the owners can change salaries in their companies before merging. But the labor union insists on two conditions: it is only allowed to increase salaries, moreover all the employees in one company must get the same increase.</p><p>Sure enough, the owners want to minimize the total increase of all salaries in all companies. Help them find the minimal possible increase that will allow them to merge companies into one.</p></div><div class="input-specification"><p>The first line contains a single integer $n$&nbsp;！ the number of companies in the conglomerate ($1 \le n \le 2 \cdot 10^5$). Each of the next $n$ lines describes a company. </p><p>A company description start with an integer $m_i$&nbsp;！ the number of its employees ($1 \le m_i \le 2 \cdot 10^5$). Then $m_i$ integers follow: the salaries of the employees. All salaries are positive and do not exceed $10^9$. </p><p>The total number of employees in all companies does not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>Output a single integer ！ the minimal total increase of all employees that allows to merge all companies.</p></div>

## Input

<p>The first line contains a single integer $n$&nbsp;！ the number of companies in the conglomerate ($1 \le n \le 2 \cdot 10^5$). Each of the next $n$ lines describes a company. </p><p>A company description start with an integer $m_i$&nbsp;！ the number of its employees ($1 \le m_i \le 2 \cdot 10^5$). Then $m_i$ integers follow: the salaries of the employees. All salaries are positive and do not exceed $10^9$. </p><p>The total number of employees in all companies does not exceed $2 \cdot 10^5$. </p>

## Output

<p>Output a single integer ！ the minimal total increase of all employees that allows to merge all companies.</p>

## Samples

```input1
3
2 4 3
2 2 1
3 1 1 1
```

```output1
13
```




## Note

<p>One of the optimal merging strategies is the following. First increase all salaries in the second company by $2$, and merge the first and the second companies. Now the conglomerate consists of two companies with salaries $[4, 3, 4, 3]$ and $[1, 1, 1]$. To merge them, increase the salaries in the second of those by $3$. The total increase is $2 + 2 + 3 + 3 + 3 = 13$.</p>
