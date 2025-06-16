<p>The police in Byteland got an anonymous tip that the local mafia bosses are     planning a big transport from the harbour to one of the secret warehouses in     the countryside.     The police knows the date of the transport and they know that the transport     will use the national highway network.</p>
<p>The highway network consists of two-way highway segments, each segment     directly connecting two distinct toll stations.     A toll station may be connected with many other stations.     A vehicle can enter or exit the highway network at toll stations only.     The mafia transport is known to enter the highways at the toll station     closest to the harbour and leave it at the toll station closest     to the warehouse (it will not leave and re-enter the highways in between).     Special police squads are to be located in selected toll stations.     When the transport enters a toll station under surveillance, it will be caught     by the police.</p>
<p>From this point of view, the easiest choice would be to place the police squad     either at the entry point or the exit point of the transport.     However, controlling each toll station has a certain cost, which may     vary from station to station.     The police wants to keep the overall cost as low as possible, so they     need to identify a <em>minimal controlling set</em> of toll stations, which     satisfies the two conditions:</p>
<ul>
<li> all traffic from the harbour to the warehouse must pass through at least         one station from that set, </li>
<li> the cost of monitoring these stations (i.e. the sum of their individual         monitoring costs) is minimal. </li>
</ul>
<p>You may assume that it is possible to get from the harbour to the warehouse     using the highways.</p>
<h3>Input</h3>
<p>The first line of the standard input contains two integers <span><img src="file://x88NUWNE.png" alt=""></span> and <span><img src="file://22W1VY6Z.png" alt=""></span> (<span><img src="file://7i1H7CyF.png" alt=""></span>, <span><img src="file://epO1CbxN.png" alt=""></span>) - the number of toll       stations and the number of direct highway segments.       The toll stations are numbered from <span><img src="file://LWmBVpT2.png" alt=""></span> to <span><img src="file://7CNKIprW.png" alt=""></span>.</p>
<p>The second line contains two integers <span><img src="file://PY28HRK2.png" alt=""></span> and <span><img src="file://XRVkJscj.png" alt=""></span> (<span><img src="file://EdKe5EgL.png" alt=""></span>,       <span><img src="file://Kvvld91x.png" alt=""></span>) - the numbers of the toll stations closest to the harbour       and to the warehouse, respectively.</p>
<p>The following <span><img src="file://m9Oncx8Q.png" alt=""></span> lines describe the monitoring costs. The <span><img src="file://QZdiRyS5.png" alt=""></span>-th of       these lines (for <span><img src="file://c62kMTYs.png" alt=""></span>) contains one integer - the monitoring       cost of the <span><img src="file://fDxCZsP3.png" alt=""></span>-th station (which is positive number not exceeding <span><img src="file://no2CLH9B.png" alt=""></span>).</p>
<p>The following <span><img src="file://7TaWtW9O.png" alt=""></span> lines describe the highway network. The <span><img src="file://wKxk4tc2.png" alt=""></span>-th of these       lines (for <span><img src="file://sycqzoyR.png" alt=""></span>) contains two integers <span><img src="file://ssnjfoXx.png" alt=""></span> and <span><img src="file://zkzUvg5h.png" alt=""></span> (<span><img src="file://6IyecHeT.png" alt=""></span>), indicating that there is a direct highway segment       between toll stations numbered <span><img src="file://goZVg3bM.png" alt=""></span> and <span><img src="file://0S4diAQy.png" alt=""></span>.       Each highway segment is listed once.</p>
<h3>Output</h3>
<p>The only line of the output should contain the numbers of toll stations in       a minimal controlling set, given in increasing order, separated by single       spaces. If there is more than one minimal controlling set, your program       may output anyone of them.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>5 6
5 3
2
4
8
3
10
1 5
1 2
2 4
4 5
2 3
3 4</pre>
<p>the correct result is:</p>
<pre>1 4</pre>
<p align="center"><img src="file://4fzcGBLF.png" alt=""></p>
<p>The figure shows the highway network with the toll station numbers     (in the upper-left corners) and the monitoring costs.     Stations number 1 and 4 constitute the minimal controlling set with     total controlling cost 5.</p>
<p><strong>&nbsp;</strong></p>