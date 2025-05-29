## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">I'm praying for owning a transparent heart; as well as eyes with tears more than enough...</span></div><div class="epigraph-source">�� Escape Plan, <a href="https://www.youtube.com/watch?v=GPnymcrXgX0"><span class="tex-font-style-it">Brightest Star in the Dark</span></a></div></div><p><span class="tex-font-style-it">Iris looked at the stars and a beautiful problem emerged in her mind. She is inviting you to solve it so that a meteor shower is believed to form.</span></p><p>There are $n$ stars in the sky, arranged in a row. Iris has a telescope, which she uses to look at the stars.</p><p>Initially, Iris observes stars in the segment $[1, n]$, and she has a <span class="tex-font-style-it">lucky value</span> of $0$. Iris wants to look for the star in the middle position for each segment $[l, r]$ that she observes. So the following recursive procedure is used:</p><ul> <li> First, she will calculate $m = \left\lfloor \frac{l+r}{2} \right\rfloor$. </li><li> If the length of the segment (i.e. $r - l + 1$) is even, Iris will divide it into two equally long segments $[l, m]$ and $[m+1, r]$ for further observation. </li><li> Otherwise, Iris will aim the telescope at star $m$, and her <span class="tex-font-style-it">lucky value</span> will increase by $m$; subsequently, if $l \neq r$, Iris will continue to observe two segments $[l, m-1]$ and $[m+1, r]$. </li></ul><p>Iris is a bit lazy. She defines her laziness by an integer $k$: as the observation progresses, she will not continue to observe any segment $[l, r]$ with a length <span class="tex-font-style-bf">strictly less than</span> $k$. In this case, please predict her final <span class="tex-font-style-it">lucky value</span>.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;�� the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains two integers $n$ and $k$ ($1 \leq k \leq n \leq 2\cdot 10^9$).</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;�� the final <span class="tex-font-style-it">lucky value</span>.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;�� the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains two integers $n$ and $k$ ($1 \leq k \leq n \leq 2\cdot 10^9$).</p>

## Output

<p>For each test case, output a single integer&nbsp;�� the final <span class="tex-font-style-it">lucky value</span>.</p>





```input1|2,4,6
6
7 2
11 3
55 13
5801 6
8919 64
8765432 1
```




```output1
12
18
196
1975581
958900
38416403456028
```



## Note

<p>In the first test case, at the beginning, Iris observes $[1, 7]$. Since $[1, 7]$ has an odd length, she aims at star $4$ and therefore increases her <span class="tex-font-style-it">lucky value</span> by $4$. Then it is split into $2$ new segments: $[1, 3]$ and $[5, 7]$. The segment $[1, 3]$ again has an odd length, so Iris aims at star $2$ and increases her <span class="tex-font-style-it">lucky value</span> by $2$. Then it is split into $2$ new segments: $[1, 1]$ and $[3, 3]$, both having a length less than $2$, so no further observation is conducted. For range $[5, 7]$, the progress is similar and the <span class="tex-font-style-it">lucky value</span> eventually increases by $6$. Therefore, the final <span class="tex-font-style-it">lucky value</span> is $4 + 2 + 6 = 12$.</p><p>In the last test case, Iris finally observes all the stars and the final <span class="tex-font-style-it">lucky value</span> is $1 + 2 + \cdots + 8\,765\,432 = 38\,416\,403\,456\,028$.</p>
