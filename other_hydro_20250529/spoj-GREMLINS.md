<p>Gremlins are small funny furry creatures. Once they were considered to be evil but that time has past and most gremlins live a decent family life now.&nbsp;There are N distinct types of gremlins.</p>
<p>Their origin is rather mysterious. Legend says that T years ago, N gremlins, one of each type, were born in a lab accident.</p>
<p>Their reproduction method is, however, well studied. No mating ritual is required for gremlins to multiply. All they need is a few drops of water and the magic happens.</p>
<p>Once a <em>type i</em> gremlin starts its reproduction process, K<sub>i</sub> small furry balls are created. For each furry ball we know what is the type of gremlin that will hatch from the furry ball and how long will it take for that to happen. Unfortunately, the original gremlin dies in the process.&nbsp;A <em>type i</em> gremlin will start its reproduction process exactly Y<sub>i</sub> years after it is <strong>born</strong>&nbsp;(ie. hatched from the furry ball).</p>
<p>Knowledge about the ancestors of a gremlin is passed on genetically, so each gremlin knows a list of his ancestors as soon as it is born.</p>
<p>Write a program that will find the length of the longest list of ancestors among all gremlins that ever lived (gremlins that still live are included, but unhatched furry balls are not), given the information about reproduction process and time elapsed since the lab accident that created initial gremlins, assuming<strong>&nbsp;all gremlins that were supposed to hatch this year have already hatched</strong>.</p>
<h3>Input</h3>
<p>The first line contains two integers N and T (1 ¡Ü N&nbsp;¡Ü 100, 1&nbsp;¡Ü T ¡Ü&nbsp;10<sup>15</sup>), the number of gremlin types and the number of year that has passed since the lab accident.</p>
<p>The next 3¡¤N lines give reproduction details for each gremlin type.</p>
<p>The first line of i-th block contains two integers K<sub>i</sub> and Y<sub>i</sub><span style="font-family: Arial; border-collapse: collapse; white-space: pre; -webkit-border-horizontal-spacing: 2px; -webkit-border-vertical-spacing: 2px; "> (</span>1&nbsp;¡Ü&nbsp;Y<sub>i</sub>&nbsp;¡Ü 1000,&nbsp;1&nbsp;¡Ü K<sub>i</sub>&nbsp;¡Ü 1000).</p>
<p>The second line contains K<sub>i</sub> integers representing gremlin type for each furry ball.</p>
<p>The third line contain K<sub>i</sub>&nbsp;integers between 1 and 1000 representing hatching time for each furry ball, in years.</p>
<h3>Output</h3>
<p>Output the length of the longest list of ancestors among all gremlins that ever lived&nbsp;in a single line.</p>
<h3>Examples</h3>
<table style="width: 100%;" border="0" frame="void" align="center">
<tbody>
<tr>
<td align="left" valign="top">
<pre><strong>Input:</strong>
1 42
1 10
1
5







<strong>Output:</strong>
2</pre>
</td>
<td align="left" valign="top">
<pre><strong>Input:</strong>
2 42
1 10
1
5
1 5
1
5




<strong>Output:</strong>
3</pre>
</td>
<td align="left" valign="top">
<pre><strong>Input:</strong>
3 8
4 5
1 2 3 2
1 2 1 3
1 1
3
1
2 1
1 2
2 1

<strong>Output:</strong>
4</pre>
</td>
</tr>
</tbody>
</table>