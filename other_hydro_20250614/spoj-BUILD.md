<p>A Millionaire Eccentric Mathematician purchases a small Island, to build his residence. In order to keep away Trespassers, he decides to Build some Beacons (Towers) on the perimeter of the Island. To build these Beacons, he visits the Mainland to purchase Stone. <br><br>Being obsessed with Prime Numbers, the stone blocks he orders are all Regular Tridecagons (13 Sides). However, their heights are variable. On delivery of the Blocks, he orders them to be flattened perfectly from the top and the bottom, so that the Tridecagonal shape is viewable from the Top (or Bottom), in such a way that the Height of each block measures to a power of 2. The stones, procured from various sources, are of Variable strength.
He intends to build the Beacons by placing Stone Blocks one over the other. The heights of the Towers are specified by the Mathematician, and they are also Prime Numbers. He instructs the Architect to make sure that once the Beacons are complete, the strengths of the used stones add up to the Maximum Possible Number.<br><br>

The Architect, not knowing how the job can be done, or even whether it CAN be done, with such complicated restrictions, approaches you to find this out for him.<br><br>


</p><h3>Input</h3>
<p>First line of input contains a positive integer T, the number of test cases. The first line of each test case contains a positive integer K, equal to the total number of stones available. This line is followed by K lines, each containing a pair of positive integers X,Y. Here X denotes the height of that stone (here the height would be 2<sup>X</sup>) and Y denotes its value. Followed is a line containing an integer N, the number of towers. Each of the next N lines contain a single positive number, which is the height H of the corresponding tower the mathematician wants to build.

</p><h3>Output</h3>
<p>Output contains T lines, one for each test case, containing a number denoting the maximum sum total of strengths of rocks used to construct the Beacons if solution is possible, else the message "Plan Failed!".

</p><h3>Example</h3>

<pre><b>Input:</b>
1
2
2 3
0 4
1
5


<b>Output:</b>
7
</pre>


<h3>Constraints and Limits</h3>
<p> T ¡Ü11, H &lt; 10^281, 0 ¡Ü X ¡Ü 977, 0 &lt; Y ¡Ü 977, 0 ¡Ü k ¡Ü 977 , N ¡Ü 97
</p>