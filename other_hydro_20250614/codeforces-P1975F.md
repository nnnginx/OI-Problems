## Description

<div><p>Define the <span class="tex-font-style-it">binary encoding</span> of a finite set of natural numbers $T \subseteq \{0,1,2,\ldots\}$ as $f(T) = \sum\limits_{i \in T} 2^i$. For example, $f(\{0,2\}) = 2^0 + 2^2 = 5$ and $f(\{\}) = 0$. Notice that $f$ is a bijection from all such sets to all non-negative integers. As such, $f^{-1}$ is also defined.</p><p>You are given an integer $n$ along with $2^n-1$ sets $V_1,V_2,\ldots,V_{2^n-1}$.</p><p>Find all sets $S$ that satisfy the following constraint: </p><ul> <li> $S \subseteq \{0,1,\ldots,n-1\}$. Note that $S$ can be <span class="tex-font-style-bf">empty</span>. </li><li> For all <span class="tex-font-style-bf">non-empty</span> subsets $T \subseteq \{0,1,\ldots,n-1\}$, $|S \cap T| \in V_{f(T)}$. </li></ul><p>Due to the large input and output, both input and output will be given in terms of binary encodings of the sets.</p></div><div class="input-specification"><p>The first line of input contains a single integer $n$ ($1 \leq n \leq 20$).</p><p>The second line of input contains $2^n-1$ integers $v_1,v_2,\ldots,v_{2^n-1}$ ($0 \leq v_i &lt; 2^{n+1}$)&nbsp;¡ª the sets $V_i$ given in their binary encoding where $V_i = f^{-1}(v_i)$.</p></div><div class="output-specification"><p>The first line of output should contain an integer $k$ indicating the number of possible $S$.</p><p>In the following $k$ lines, you should output $f(S)$ for all possible $S$ in <span class="tex-font-style-bf">increasing order</span>.</p></div>

## Input

<p>The first line of input contains a single integer $n$ ($1 \leq n \leq 20$).</p><p>The second line of input contains $2^n-1$ integers $v_1,v_2,\ldots,v_{2^n-1}$ ($0 \leq v_i &lt; 2^{n+1}$)&nbsp;¡ª the sets $V_i$ given in their binary encoding where $V_i = f^{-1}(v_i)$.</p>

## Output

<p>The first line of output should contain an integer $k$ indicating the number of possible $S$.</p><p>In the following $k$ lines, you should output $f(S)$ for all possible $S$ in <span class="tex-font-style-bf">increasing order</span>.</p>





```input1|
3
15 15 15 15 15 15 12
```




```input2|
5
63 63 63 63 6 63 63 63 63 63 63 5 63 63 63 63 63 63 8 63 63 63 63 2 63 63 63 63 63 63 63
```




```output1
4
3
5
6
7
```




```output2
1
19
```



## Note

<p>In the first test case, one possible $S$ is $f^{-1}(3) = \{0,1\}$. All the non-empty subsets $T \subseteq \{0,1,2\}$ and the corresponding $|S \cap T|$, $f(T)$ and $V_f(T)$ are as follows:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$T$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$|S\cap T|$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$f(T)$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$V_{f(T)}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{0\}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{0,1,2,3\}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{1\}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{0,1,2,3\}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{2\}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$4$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{0,1,2,3\}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{0,1\}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{0,1,2,3\}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{0,2\}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$5$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{0,1,2,3\}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{1,2\}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$6$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{0,1,2,3\}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{0,1,2\}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$7$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\{2,3\}$</td></tr></tbody></table> </center>
