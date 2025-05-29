<p>Shortly after his abdication from the Bytelandian throne Johnny decided to go into farming. Water melons were a natural choice as his first crop ever, since they seemed easy enough to grow and look after. So, he sold all his beer bottles and for the money he purchased a 1km x 1km square field. Here it was that he planted the water melon seeds. (The word 'planted' is really a bit of a euphemism for walking across a field gorging on a water melon and spitting out the pips but, for the sake of politeness, let us leave it this way).
</p><p>
To everyone's surprise a lot of the seeds sprouted stems, and soon enough many of the plants showed signs of fruit (and some had even more than one!). Then quite unexpectedly, when the water melons were still a little too unripe to eat, winter set in. Johnny knows that he has to construct a green house to protect the field but, with his rather limited budget, he cannot afford the glass to cover the whole area. He has decided that it is enough that <i>k</i> fruit survive the ordeal under a glazed roof. For reasons of architectural planning in Byteland it is necessary that the green house be a rectangle with sides parallel to the edges of the plot.
</p><p>
You have been requested to help Johnny minimise investement costs. Since glass is paid for by the square meter, design a green house with the smallest possible area fulfilling the imposed conditions.

</p><h3>Input</h3>
<p>The first line of input contains the integer <i>t</i>&lt;=100, the number of test cases. <i>t</i> test cases follow.
</p><p>
Every test case begins with a line containing two integers <i>n k</i>, denoting the total number of plants and the number of water melon fruit to be protected, respectively (1&lt;=<i>n</i>&lt;=1000, 1&lt;=<i>k</i>&lt;=10<sup>6</sup>, <i>k</i> doesn't exceed the total number of fruit in the plantation). Each of the next <i>n</i> lines describes a single plant, the <i>i</i>-th line containing three integers <i>x<sub>i</sub> y<sub>i</sub> f<sub>i</sub></i> - the X and Y coordinates of the plant, and the number of water melon fruit on it, respectively (1&lt;=<i>x<sub>i</sub>, y<sub>i</sub>, f<sub>i</sub></i>&lt;=1000).

</p><h3>Output</h3>
<p>For each test case output a single integer, denoting the area of the smallest possible rectangular glass house with horizontal and vertical edges, sufficient to cover at least <i>k</i> fruit of the plantation.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
6 11
1 1 2
1 2 2
3 1 2
3 2 3
4 2 5
3 3 2

<b>Output:</b>
2
</pre>
<p>
<img src="/content/adrian:watermelon.png" alt="Illustration of sample test data">
</p>