## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">Be careful not to make a mistake. You might have to start all over again.</span></div><div class="epigraph-source">！ Someone, probably</div></div></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 10^5$) ！ the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 2$) ！ the array $a$.</p></div><div class="output-specification"><p>Output a single integer&nbsp;！ the number of solutions, modulo $20240401$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 10^5$) ！ the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 2$) ！ the array $a$.</p>

## Output

<p>Output a single integer&nbsp;！ the number of solutions, modulo $20240401$.</p>





```input1|
7
1 1 2 1 1 2 0
```




```input2|
7
1 1 2 1 1 1 0
```




```input3|
7
0 1 2 1 1 1 0
```




```output1
1
```




```output2
2
```




```output3
0
```



## Note

<p>In the first sample, the array looks like this:</p><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{darkgreen}{2} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{darkgreen}{2} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{gray}{0} $</td></tr></tbody></table><p></p><p>Obviously, the answer here is $1 \pmod{20240401}$.</p><p>In the second sample, the array looks like this:</p><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{darkgreen}{2} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{gray}{0} $</td></tr></tbody></table><p></p><p>I do not know why the answer here is $2 \pmod{20240401}$, I had to take a guess.</p><p>In the third sample, the array looks like this:</p><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{gray}{0} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{darkgreen}{2} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{blue}{1} $</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \color{gray}{0} $</td></tr></tbody></table><p></p><p>If the answer here is not $0 \pmod{20240401}$, I am literally going to explode.</p>
