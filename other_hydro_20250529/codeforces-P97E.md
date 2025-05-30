## Description

<div><p>After a revolution in Berland the new dictator faced an unexpected challenge: the country has to be somehow ruled. The dictator is a very efficient manager, yet he can't personally give orders to each and every citizen. That's why he decided to pick some set of leaders he would control. Those leaders will directly order the citizens. However, leadership efficiency turned out to vary from person to person (i.e. while person A makes an efficient leader, person B may not be that good at it). That's why the dictator asked world-famous berland scientists for help. The scientists suggested an innovatory technology — to make the leaders work in pairs.</p><p>A relationship graph is some undirected graph whose vertices correspond to people. A simple path is a path with no repeated vertices. Long and frighteningly expensive research showed that a pair of people has maximum leadership qualities if a graph of relationships has a simple path between them with an odd number of edges. The scientists decided to call such pairs of different people <span class="tex-font-style-it">leader pairs</span>. Secret services provided the scientists with the relationship graph so that the task is simple — we have to learn to tell the dictator whether the given pairs are leader pairs or not. Help the scientists cope with the task.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of vertices and edges in the relationship graph correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain pairs of integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> which mean that there is an edge between the <span class="tex-span"><i>a</i></span>-th and the <span class="tex-span"><i>b</i></span>-th vertices (the vertices are numbered starting from <span class="tex-span">1</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>). It is guaranteed that the graph has no loops or multiple edges.</p><p>Next line contains number <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of pairs the scientists are interested in. Next <span class="tex-span"><i>q</i></span> lines contain these pairs (in the same format as the edges, the queries can be repeated, a query can contain a pair of the identical vertices).</p></div><div class="output-specification"><p>For each query print on a single line "Yes" if there's a simple odd path between the pair of people; otherwise, print "No".</p></div>


## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of vertices and edges in the relationship graph correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain pairs of integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> which mean that there is an edge between the <span class="tex-span"><i>a</i></span>-th and the <span class="tex-span"><i>b</i></span>-th vertices (the vertices are numbered starting from <span class="tex-span">1</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>). It is guaranteed that the graph has no loops or multiple edges.</p><p>Next line contains number <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of pairs the scientists are interested in. Next <span class="tex-span"><i>q</i></span> lines contain these pairs (in the same format as the edges, the queries can be repeated, a query can contain a pair of the identical vertices).</p>


## Output

<p>For each query print on a single line "Yes" if there's a simple odd path between the pair of people; otherwise, print "No".</p>


## Samples

```input1
7 7
1 3
1 4
2 3
2 4
5 6
6 7
7 5
8
1 2
1 3
1 4
2 4
1 5
5 6
5 7
6 7

```

```output1
No
Yes
Yes
Yes
No
Yes
Yes
Yes

```




## Note

<p>Notes to the samples:</p><p>1) Between vertices 1 and 2 there are 2 different simple paths in total: 1-3-2 and 1-4-2. Both of them consist of an even number of edges. </p><p>2) Vertices 1 and 3 are connected by an edge, that's why a simple odd path for them is 1-3.</p><p>5) Vertices 1 and 5 are located in different connected components, there's no path between them.</p>

