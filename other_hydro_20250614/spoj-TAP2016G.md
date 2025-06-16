<p><strong>[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2016 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at <a href="http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf</a>&nbsp;]</strong></p>
<p>Nlogononia's train network consists of <strong>N</strong> stations, each of them strategically placed in a different city of the kingdom. Certain pairs of stations are connected by railways, and on each railway there is a train service going on both directions. For centuries the <em>Institute for the Cities' Perfect Connection&nbsp;</em>(ICPC) has been in charge of optimizing public transportation in Nlogonia, so today the train network is so efficient there is exactly one way to travel between any pair of cities using trains. Note that it may be necessary for a traveller to successively take several trains, in case there is no direct connection between the pair of stations he is traveling to/from. In other realms this might be considered an inconvenience, but Nlogonia's inhabitants are happy knowing that they will not waste a single minute thinking about which route to take from one city to another.</p>
<p>The ticket for each train service has certain price, so that a passenger taking one or more trains to travel between two cities has to buy the corresponding tickets before boarding each train. Nlogonia's currency is also extremely efficient, as there are bills with values corresponding to every non-negative power of two. This is, the denomination of bills in Nlogonia is of <strong>2<sup>0</sup> = 1</strong> unit, <strong>2<sup>1</sup> = 2</strong>&nbsp;units, <strong>2<sup>2</sup> = 4</strong>&nbsp;units, and so on. As a result of this monetary eficiency, Nlogonians always pay their tickets by providing the minimum number of bills with which it is possible to reach the exact amount of the ticket they are buying.</p>
<p>To speed up ticket buying, the <em>Agency for Counting Money</em>&nbsp;(ACM) would like to introduce the following offer. When a passenger is going to make a trip, he can pay all the tickets he will be needing in advance. When doing so, he must present all the bills he would use along his journey, and the ACM will only take one bill of each denomination for which the passenger provided an odd amount of bills. In this way, if for example a passenger wants to buy three tickets with prices of <strong>3</strong>, <strong>7</strong>&nbsp;and <strong>10</strong>&nbsp;units, he will present two bills for the first ticket (with denominations <strong>1</strong>&nbsp;and <strong>2</strong>), three bills for the second one (with denominations <strong>1</strong>, <strong>2</strong>&nbsp;and <strong>4</strong>) and two bills for the third (with denominations <strong>2</strong>&nbsp;and <strong>8</strong>). The ACM would then take only one of the bills with denomination <strong>2</strong>, along with each of the bills with denominations <strong>4</strong>&nbsp;and <strong>8</strong>, returning to the passenger two bills of denomination <strong>1</strong>, as well as two bills with denomination <strong>2</strong>.</p>
<p>Now the ACM's steering committee is worried because this offer might be too expensive for the kingdom's treasury. There is certainly good cause for this, as one should note that it is even possible to travel for free (<em>e.g.</em>&nbsp;any round trip will be free, as an even number of tickets of each value will always be required). Your job is to evaluate the extent of the problem, for which the ACM has commanded you to determine the maximum price a passenger might have to pay when starting his journey from each of the <strong>N</strong>&nbsp;train stations in Nlogonia.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. The first line contains an integer number <strong>N</strong>, representing the number of train stations in Nlogonia (<strong>2 ¡Ü&nbsp;N&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;10<sup>5</sup></strong>). Train stations in Nlogonia are numbered from <strong>1</strong>&nbsp;to <strong>N</strong>. Each of the following <strong>N-1</strong>&nbsp;lines contains three integer numbers <strong>A</strong>, <strong>B</strong>&nbsp;and <strong>C</strong>, indicating there is a railway directly connecting stations <strong>A</strong>and <strong>B</strong>, being <strong>C</strong>&nbsp;the price of the ticket for the train service operating on said railway (<strong>1 </strong><strong>¡Ü</strong><strong>&nbsp;A, B&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;N</strong>&nbsp;and <strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;C&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;10<sup>9</sup></strong>, with <strong>A ¡Ù&nbsp;B</strong>). The description of the railway network is always such that for each pair of distinct stations there exists one and only one sequence of train services connecting them.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print <strong>N</strong>&nbsp;lines each containing one integer number. The number printed on the <strong>i</strong>-th line should correspond to the maximum value of the tickets that may be payed by a passenger starting his journey at the station identified by the number <strong>i</strong>, when the offer described in the problem statement is applied.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input #1:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">4
1 2 3
2 3 7
3 4 10</span>

<strong>Output #1:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">14
13
10
14</span><span style="white-space: normal;">
</span></pre>
<pre><strong>Input #2:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">6
1 2 1
3 2 2
2 4 3
4 5 4
4 6 5</span>

<strong>Output #2:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">7
7
5
5
7
7</span></pre>
<pre><strong>Input #3:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">7
1 2 1
1 3 2
1 4 3
1 5 4
1 6 5
1 7 6</span>

<strong>Output #3:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">6
7
7
7
7
7
7</span></pre>