<p>Some 2000 years ago the Roman Empire covered a large part of Europe including the entire coast of the Mediterranean. The transportation network of that empire
consisted of roads and sea routes (the two are considered equivalent and simply called roads for this problem). Each road connected exactly two cities and the road network was such that every city can be reached from Rome. However, building this network required resources (cobblestone and buoys) proportional to the total length of the network. In order to cut down on building costs and maintainance and spend the rest of the money on wine, the empire built the cheapest possible network.

</p><p>Additionally, each road had a single signpost that listed all of the other roads it connected to (at any of its two cities). There were <i>N</i> roads in the empire labeled <i>1</i>, <i>2</i>, ..., <i>N</i>.  It is believed that a traveller once travelled all roads and for each road wrote down the numbers on its signpost, thus making a map.

</p><p>2000 years later a young archaeologist found something that looks suspiciously like that map. Your job is to write a program that determines if this can really be a map of the Roman empire and for each road output the two cities it connected.  Note that roads in a valid map are always between two distinct cities.

</p><p>(Disclaimer: The description of the transportation network is for this problem only and may not necessarily be what the Roman Empire actually did. Do not cite this in your history papers: I made it up.)

</p><h3>Input</h3>
<p>The first line of input contains <i>N</i>, <i>1</i> ¡Ü <i>N</i> ¡Ü <i>500</i>.
Each of the next <i>N</i> lines contains a space-separated list of integers. The <i>i</i>-th of these lines describes the "roads" that connect to "road" <i>i</i>. The first number on the line specifies the number of those "roads", <i>d<sub>i</sub></i>, and the following <i>d<sub>i</sub></i> numbers specify their labels.

</p><p>Note that although at this point we don't know if the map is valid, the input is consistent, i.e. if a road <i>x</i> is on the signpost of <i>y</i>, then <i>y</i> will be on the signpost of <i>x</i>. (Otherwise the archaeologist would know this is not a Roman map right away).

</p><h3>Output</h3>
<p>If the input <i><b>cannot</b></i> describe a valid map according to the description, output "NO" on the first (and only) line of output.

</p><p>Otherwise, output "YES" and on each of the next <i>N</i> lines, write two integers separated by space, the numbers of the two cities that the road connected. City labeling is up to you with the only restriction that all city labels must be integers between <i>1</i> and <i>M</i>, where <i>M</i> is the total number of cities. Of course, a city can only have one label.

</p><p>Note that since we don't know the actual locations of the cities or whether the roads were straight, we have no idea what the total cost of the network might have been. 
The archaeologist is willing to accept any map for which she can't determine if there is a cheaper network without knowing the actual costs. It is assumed that each road had some positive cost.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
2 3 2
2 1 3
2 2 1

<b>Output:</b>
YES
1 3
4 1
1 2
</pre>