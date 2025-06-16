<p>Today is the town¡¯s celebration day, on which tradition dictates that all townspeople go partying. Each of them should attend a party at one of the pubs, and dance and drink to the point of intoxication. Later on, once all the parties have come to an end, after-parties start being thrown at other pubs, and every villager then goes to one. In order for the villagers to make as many acquaintances as possible, no two of them attend the same two parties.</p>
<p>Needless to say, such practice causes everyone to have a severe blackout regarding the events of the night, but people are still curious to know what happened. Unfortunately, all they seem to be able to remember is who coincided with them at some point, but they have serious trouble identifying when or where. And as their memory of even this piece of information may be shaky (to say the least), they need help in figuring out whether all their recollections are consistent or if, on the contrary, some of the townspeople must have made a mistake (either by failing to remember someone else who was there, or by incorrectly thinking they met someone they didn¡¯t). Can you help them?</p>
<p>For example, in a town of 4 people, if we are told that villagers 0, 1 and 2 all met one another, and villagers 2 and 3 met as well, the data is consistent because there might have been parties <em>P</em>0 and <em>P</em>1, and after-parties <em>A</em>0, <em>A</em>1 and <em>A</em>2, such that person 0 went to <em>P</em>0 and <em>A</em>0, person 1 to <em>P</em>0 and <em>A</em>1, person 2 to <em>P</em>0 and <em>A</em>2, and person 3 to <em>P</em>1 and <em>A</em>2; this arrangement satisfies all required conditions. However, if persons 0 and 3 claimed to have met too, the data would become inconsistent.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The input file will contain several test cases. Each of them begins with a line containing two integers: 1 ¡Ü <em>n</em> ¡Ü 100, the number of villagers; and 0 ¡Ü <em>m</em> ¡Ü 1000. <em>m</em> lines follow, each containing a pair of integers <em>i</em> and <em>j</em>, 0 ¡Ü <em>i</em>, <em>j</em> &lt; <em>n</em>, <em>i</em> ¡Ù <em>j</em>, meaning that persons numbered <em>i</em> and <em>j</em> remember having been together in a pub. No pair of people will appear twice.</p>
<p>Different test cases will be separated by a blank line. A line with <em>n</em> = <em>m</em> = 0 signals the end of the input.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each test case, print ¡°YES¡± if there is a configuration of parties, after-parties, and villagers attending them under the conditions described, such that the pairs of people who met each other are exactly those in the input data. Print ¡°NO¡± otherwise.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">4 4
0 1
0 2
1 2
2 3

4 5
0 1
0 2
1 2
2 3
0 3

7 11
0 1
0 2
0 4
1 3
1 5
1 6
2 4
2 5
3 5
3 6
5 6

0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">YES
NO
YES
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: David Garc¨ªa Soriano</em></blockquote>