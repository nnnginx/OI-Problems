<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td style="text-align: center;" width="50%"><a href="/problems/MTEMP/en/">English</a></td>
<td style="text-align: center;" width="50%"><a href="/problems/MTEMP/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p>
</p><p>John never knew he had a grand-uncle, until he received the notary’s letter. He learned that his late grand-uncle had gathered a lot of money, somewhere in South-America, and that John was the only inheritor. </p><p>John did not need that much money for the moment. But he realized that it 
would be a good idea to store this capital in a safe place, and have it
grow until he decided to retire. The bank convinced him that a certain kind of 
bond was interesting for him. This kind of bond has a ﬁxed value, and gives
a ﬁxed amount of yearly interest, payed to the owner at the end of each year. </p><pre><br></pre>

<p>The bond has no ﬁxed term. Bonds are available in different sizes.  The larger ones usually give a better interest. Soon John realized that the optimal set of bonds to buy was not trivial to ﬁgure out. Moreover, after a few  years his capital would have grown, and the schedule had to be re-evaluated. Assume the following bonds are available:</p>
<pre><pre>Value Annual interest
4000 400
3000 250

<br></pre>
</pre>
<p>With a capital of 10 000$ one could buy two bonds of 4000$, giving a yearly interest  of 800$. Buying two bonds of 3000$, and one of 4000$ is a better idea, as it gives a  yearly interest of e900. After two years the capital has grown to 11800$, and it  makes sense to sell a 3000$ one and buy a 4000$ one, so the annual interest  grows to 1050$.</p>
<p>This iswhere this story grows unlikely: the bank does not charge for buying and selling bonds. Next year the total sum is 12850$, which allows for three times 4000$, giving a yearly interest of 1200$. Here is your problem: given an amount to begin with, a number of years, and a set of bonds with their values and interests, ﬁnd out how big the amount may grow  in the given period, using the best schedule for buying and selling bonds.</p>
<pre><h3 style="text-align: center;">Input</h3>
</pre>
<p>&nbsp;</p>
<pre><p>The ﬁrst line contains a single positive integer N which is the number 
of test cases.  
The ﬁrst line of a test case contains two positive integers: 
the amount to start with (at most 1000 000$), and the number of years the 
capital may grow (at most 40).
The following line contains a single number: the number d (1 ≤ d ≤ 10) of 
available bonds.
The next d lines each contain the description of a bond. 
The description of a bond consists of two positive integers: the value 
of the bond, and the yearly interest for that bond. The
value of a bond 
is always a multiple of 1000$. The interest of a bond is never more than
10% of its value

SAMPLE INPUT
1
10000 4
2
4000 400
3000 250
</p>
<h3 style="text-align: center;">Output</h3>
<p>For each test case, output – on a separate line – the capital at the end
of the period, after an optimal schedule of buying and selling.

SAMPLE OUTPUT
14050
</p>
 </pre>