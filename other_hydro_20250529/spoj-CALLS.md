<p> A young archeologist Senoj Anaidni recently made a very important discovery which will make him famous (or at least he thinks so). He found several scraps of paper resembling advertisement flyers of an ancient phone company. His research showed that modern phone companies follow a few basic rules to compose their flyers (and there is no reason to assume that old companies were an exception). <br><br>

Each company operates certain number of phone lines. Each phone line connects a pair of cities, and it can be used in both directions. The cost of using each line is a fixed positive number. A call from city A to city B may be routed through one or more other cities, in which case the cost of the call is the sum of the costs of all lines used. (In fact, sometimes it is cheaper to route the call through several other cities than to use the direct connection, even if there exists one.) <br><br>

To make the information comprehensible to the customer, the phone company lists the cost of the cheapest possible call between every pair of cities serviced by the company. To impress the customer even more, the company also lists the number of lines it operates. <br><br>

Indeed, each of Senoj's ancient flyers start like this: "Using our 47 telephone lines, we serve 10 most important cities of the world! A call from Sparta to Troja costs 12 dennario, Sparta to Athens is 15 dennario, ...". The list of all pairs of cities and the respective costs of the cheapest possible call between them follows. <br><br>

This supports Senoj's hypothesis about the origin of the papers, but he is not sure whether they are really genuine. Other archeologists often play dirty jokes on him by making ridiculous forgeries in a hope, that he will make a fool of himself. Luckily, they are often not very meticulous, so we can safely assume, that a flyer is a forgery if and only if it could not have been published by any phone company. 
<br>
</p>

<h3>Input</h3>
<p>
The first line of the input file gives the number <i>t</i> of flyers found by Senoj. [<i>t</i> &lt;= 50] Each flyer is described in a separate block starting with a line containing two integers - N and K - where N is the number of cities and K is the number of phone lines. [N &lt;= 300 K &lt;= 1200] The block continues with N-1 lines giving the costs of the cheapest calls between all pairs of cities. In particular, the i-th line contains (N-i) numbers, where j-th number represents the cost of a call between the cities i and (i+j). 
</p>

<h3>Output</h3>
<p>For every input block, output a line containing either "YES" or "NO". "YES" should be printed, if it is possible to assign costs to the phone lines operated by the company so that the cheapest calls are as advertised in the flyer. "NO" should be printed if this is not possible.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
3 3
1 2
2
3 2
1 2
2


<b>Output:</b>
YES
NO

</pre>