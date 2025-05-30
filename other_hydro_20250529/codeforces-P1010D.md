## Description

<div><p>Natasha travels around Mars in the Mars rover. But suddenly it broke down, namely&nbsp;！ the logical scheme inside it. The scheme is an undirected tree (connected acyclic graph) with a root in the vertex $1$, in which every leaf (excluding root) is an input, and all other vertices are logical elements, including the root, which is output. One bit is fed to each input. One bit is returned at the output.</p><p>There are four types of logical elements: <a href="https://en.wikipedia.org/wiki/Logical_conjunction">AND</a> ($2$ inputs), <a href="https://en.wikipedia.org/wiki/Logical_disjunction">OR</a> ($2$ inputs), <a href="https://en.wikipedia.org/wiki/Exclusive_or">XOR</a> ($2$ inputs), <a href="https://en.wikipedia.org/wiki/Negation">NOT</a> ($1$ input). Logical elements take values from their direct descendants (inputs) and return the result of the function they perform. Natasha knows the logical scheme of the Mars rover, as well as the fact that only one input is broken. In order to fix the Mars rover, she needs to change the value on this input.</p><p>For each input, determine what the output will be if Natasha changes this input.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^6$)&nbsp;！ the number of vertices in the graph (both inputs and elements).</p><p>The $i$-th of the next $n$ lines contains a description of $i$-th vertex: the first word "AND", "OR", "XOR", "NOT" or "IN" (means the input of the scheme) is the vertex type. If this vertex is "IN", then the value of this input follows ($0$ or $1$), otherwise follow the indices of input vertices of this element: "AND", "OR", "XOR" have $2$ inputs, whereas "NOT" has $1$ input. The vertices are numbered from one.</p><p>It is guaranteed that input data contains a correct logical scheme with an output produced by the vertex $1$.</p></div><div class="output-specification"><p>Print a string of characters <span class="tex-font-style-tt">'0'</span> and <span class="tex-font-style-tt">'1'</span> (without quotes)&nbsp;！ answers to the problem for each input in the ascending order of their vertex indices.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^6$)&nbsp;！ the number of vertices in the graph (both inputs and elements).</p><p>The $i$-th of the next $n$ lines contains a description of $i$-th vertex: the first word "AND", "OR", "XOR", "NOT" or "IN" (means the input of the scheme) is the vertex type. If this vertex is "IN", then the value of this input follows ($0$ or $1$), otherwise follow the indices of input vertices of this element: "AND", "OR", "XOR" have $2$ inputs, whereas "NOT" has $1$ input. The vertices are numbered from one.</p><p>It is guaranteed that input data contains a correct logical scheme with an output produced by the vertex $1$.</p>

## Output

<p>Print a string of characters <span class="tex-font-style-tt">'0'</span> and <span class="tex-font-style-tt">'1'</span> (without quotes)&nbsp;！ answers to the problem for each input in the ascending order of their vertex indices.</p>

## Samples

```input1
10
AND 9 4
IN 1
IN 1
XOR 6 5
AND 3 7
IN 0
NOT 10
IN 1
IN 1
AND 2 8

```

```output1
10110
```




## Note

<p>The original scheme from the example (before the input is changed):</p><p><img class="tex-graphics" src="./29432/file/2P7wAwfe.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Green indicates bits <span class="tex-font-style-tt">'1'</span>, yellow indicates bits <span class="tex-font-style-tt">'0'</span>.</p><p>If Natasha changes the input bit $2$ to $0$, then the output will be $1$.</p><p>If Natasha changes the input bit $3$ to $0$, then the output will be $0$.</p><p>If Natasha changes the input bit $6$ to $1$, then the output will be $1$.</p><p>If Natasha changes the input bit $8$ to $0$, then the output will be $1$.</p><p>If Natasha changes the input bit $9$ to $0$, then the output will be $0$.</p>
