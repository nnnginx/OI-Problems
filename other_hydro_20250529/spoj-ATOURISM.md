<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/ATOURISM/en/">English</a></td> 
<td width="50%"><a href="/problems/ATOURISM/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>
There has been a growing interest in adventure tourism lately. However, organizing adventure tours is not an easy task. It requires very careful preparation with attention to specific details.
</p>
<p>
This tour has p young male and q female participants. In addition to the logistic and rescue team, the organizers also assign k more guides to join the tour. In the first stage of the tour, the road is quite narrow passing a cliff; the group will have to go in one line. To be able to help each other, a female participant has to go next to, i.e. before or after, a male participant or a guide. Furthermore, there must be at least one participant next to a guide. Given these constraints, there are several ways the group can form a line. Let��s denote B, G and M as a male participant, a female participant and a guide respectively. A line formation can be represented by a string of length (p+q+k) containing characters from the set (B, G, M). Two line formations are different if their string representations are different. For example, the group having 2 male, 2 female and a guide (p = q = 2, k = 1) has 24 different way to form a line as follows:
</p>

<p>
Given p, q, and k, let��s denote n as the number of different ways to form a line. Your task is to write a program to calculate the remainder of n divided by 10<sup>7</sup>.
</p>
<h3>Input</h3>
<p>
The input file consists of several data sets. The first line of the input file contains the number of data sets which is a positive integer and is not bigger than 20. The following lines describe the data sets.
</p>
<p>
For each data test, there is only one line containing three integers p, q and k (0 �� p, q �� 1 000, 0 �� k �� 10) separated by space.
</p>
<h3>Output</h3>
<p>
For each data test, write in one line the remainder of the number of different line formations divided by 10<sup>7</sup>.
</p>
<h3>Example</h3>
<pre><b>Sample Input</b>
1
2 2 1	

<b>Sample Output</b>
24
</pre>