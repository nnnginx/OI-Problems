<p align="justify">Cities of the ancient country GRAPH connected by two-way (bidirectional) roads so that from any city you can get to any other city. The Sultan wants to destroy some roads and divide the country into two separate (disconnected) areas, so that from the city of one area it was impossible to get to the city of another area. You are the Minister of transportation and your task is to minimize the number of roads that need to be destroyed. You have a lot of time and the Sultan hopes :-) that you will solve this task.</p>
<h3>Input</h3>
<p align="justify">The first line of input will contain one integer number <em>8&nbsp;¡Ü&nbsp;N&nbsp;¡Ü&nbsp;1400</em>, number of cities in GRAPH. Follow <em>N</em> lines. Each line represents cities (direct neighbors) connected to the city number <em>i</em> (cities numbering is zero based) by one road. There will be 7 input files.</p>
<h3>Output</h3>
<p align="justify">One integer number. The minimum number of roads that need to be destroyed.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
8
1 2
0 2 3 
0 1 3
1 2 4
3 5 6
4 6 7
4 5 7
5 6
</pre>
<pre><strong>Output:</strong>
1
</pre>
<h4>Example explanation</h4>
<p align="justify">Destroy only one road from the third city to the fourth city and Sultan will be happy.</p>
<p><img title="DISGRAPH" src="../../content/julkas:DISGRAPH.png" alt="DISGRAPH" width="100%"></p>