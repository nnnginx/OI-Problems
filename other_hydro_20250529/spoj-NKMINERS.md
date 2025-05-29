<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/NKMINERS/en/">English</a></td> 
<td width="50%"><a href="/problems/NKMINERS/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p>
There are two coal mines, each employing a group of miners. Mining coal is hard work, so miners need food to
keep at it. Every time a shipment of food arrives at their mine, the miners produce some amount of coal. There
are three types of food shipments: meat shipments, fish shipments and bread shipments.</p>
<p>Miners like variety in their diet and they will be more productive if their food supply is kept varied. More
precisely, every time a new shipment arrives to their mine, they will consider the new shipment and the
previous two shipments (or fewer if there haven't been that many) and then:</p>
<ul>
<li>If all shipments were of the same type, they will produce one unit of coal.</li>
<li>If there were two different types of food among the shipments, they will produce two units of coal.</li>
<li>If there were three different types of food, they will produce three units of coal.</li>
</ul>
<p>We know in advance the types of food shipments and the order in which they will be sent. It is possible to
influence the amount of coal that is produced by determining which shipment should go to which mine.
Shipments cannot be divided; each shipment must be sent to one mine or the other in its entirety.</p>
<p>The two mines don't necessarily have to receive the same number of shipments (in fact, it is permitted to send all
shipments to one mine).</p>

<h3>Task</h3>
<p>Your program will be given the types of food shipments, in the order in which they are to be sent. Write a
program that finds the largest total amount of coal that can be produced (in both mines) by deciding which
shipments should be sent to mine 1 and which shipments should be sent to mine 2.</p>

<h3>Input</h3>
<p>The first line of input contains an integer N (1 ¡Ü N ¡Ü 100 000), the number of food shipments.</p>
<p>The second line contains a string consisting of N characters, the types of shipments in the order in which they
are to be distributed. Each character will be one of the uppercase letters 'M' (for meat), 'F' (for fish) or 'B' (for
bread).</p>

<h3>Output</h3>
<p>Output a single integer, the largest total amount of coal that can be produced.</p>

<h3>Grading</h3>
<p>In test cases worth a total of 45 points, the number of shipments N will be at most 20.</p>

<h3>Example</h3>
<pre><b>Input</b>
6
MBMFFB

<b>Output</b>
12
</pre>

<pre><b>Input</b>
16
MMBMBBBBMMMMMBMB

<b>Output</b>
29
</pre>