<p>Once upon a time there was a very peaceful country named Nlogonia. Back then, Poly the Shoemaker could come to the country and travel freely from city to city doing his job  without any harassment. This task was very easy, as every city in Nlogonia had a direct road to every other city in the country. He could then easily travel the whole country visiting each city exactly once and fixing everybody's shoes.</p>
<p>But not anymore. The times have changed and war has come to Nlogonia. The age when people could travel freely is over.</p>
<p>Confederations identified by colors were formed among the cities all over the country, and now each city belongs to at least one and at most two confederations. When trying to enter a city, you must give to the border officer a ticket from one of the confederations this city belongs to. When leaving the city, you receive a ticket from the other confederation the city belongs to (i.e. different from the one you gave when entering) or from the same confederation if the city only belongs to one.</p>
<p>As Poly the Shoemaker is a long time friend of Nlogonia, he is allowed to choose a ticket and a city he wants to enter as the first city in the country,  but after that he must obey the confederations rules. He wants to do the same routine he did before, visiting each city exactly once in Nlogonia, but now it's not easy for him to do this, even though he can choose where to start his journey.</p>
<p>For example, suppose there are four cities, labeled from 0 to 3. City 0 belongs to confederations <em>red</em> and <em>green</em>; city 1 belongs only to <em>red</em>; city 2 belongs to <em>green</em> and <em>yellow</em>; and city 3 belongs to <em>blue</em> and <em>red</em>. If Poly the Shoemaker chooses to start at city 0, he can enter it carrying either the <em>red</em> or the  <em>green</em> ticket and leave receiving the other.  Should he choose the <em>red</em> ticket, he will leave with a <em>green</em> ticket,  and then there is only city 2 he can travel to. When leaving city 2 he receives the <em>yellow</em> ticket and now can't go anywhere else. If he had chosen the <em>green</em> ticket as the first he would receive the <em>red</em> one when leaving,  and then he could travel to cities 1 or 3. If he chooses city 3, when leaving he will receive the <em>blue</em> ticket and again can't go anywhere else. If he chooses city 1, he receives the <em>red</em> ticket again when leaving (city 1 belongs only to the <em>red</em> confederation) and can only travel to city 3 and will never get to city 2. Thus, it is not possible to visit each city exactly once starting at city 0. It is possible, however, starting at city 2 with the <em>yellow</em> ticket,  leaving the city with the <em>green</em> ticket, then visiting city 0, leaving with <em>red</em> ticket, then visiting city 1, leaving with <em>red</em> ticket again and, at last, visiting city 3.</p>
<p>As you can see, it got really difficult for Poly the Shoemaker to accomplish the task, so he asks you to help him. He wants to know if it's possible to choose a city to start such that he can travel all cities from Nlogonia exactly once.</p>
<p>Can you help Poly the Shoemaker?</p>
<h3>Input</h3>
<p>The input contains several test cases. The first line of a test case contains two integers <em>N</em> and <em>C</em>, separated by one space, indicating  respectively the number of cities (1   �� <em>N</em> �� 500) and confederations  (1   �� <em>C</em> �� 100) in the country. Each of the next <em>C</em> lines describes a confederation. It starts with one integer <em>K</em> (0   �� <em>K</em> �� <em>N</em>) and then <em>K</em> integers representing the cities which belong to this confederation. All integers are separated by single spaces  and cities are numbered from 0 to <em>N</em> -1. Each city will appear at least once and at most twice and no city will be repeated on the same confederation.</p>
<p>The end of input is indicated by a line containing two zeroes separated by a single space.</p>
<h3>Output</h3>
<p>For each test case in the input, your program must print a single line, containing the integer <tt>-1</tt> if it's not possible to match the requirements or one integer representing the city where Poly the Shoemaker can start his journey. If there are multiple correct answers, print the smallest one.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 4
1 3
3 0 1 3
2 0 2
1 2
3 4
1 0
3 0 1 2
1 1
1 2
3 4
1 1
2 1 0
2 0 2
1 2
0 0


<strong>Output:</strong>
2
-1
1

</pre>