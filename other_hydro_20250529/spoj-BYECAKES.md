<p>
John is moving to a different city and he wants to use all his perishable food before doing it, to avoid wasting. Luckily all he has now is eggs, flour, sugar and milk, so he is going to make his famous cakes and give them to his friends as a goodbye gift. John only knows how to make an entire cake and not half a cake, a third of a cake, or any other portion. So, he will buy whatever is needed of each ingredient so that he can make an integer number of cakes and have nothing left. Of course, he wants to spend as little money as possible. You must help John to decide how much he should buy of each ingredient.</p>

<h3>Input</h3>
<p>The input contains several test cases. Each test case is described in a single line that contains eight integers E, F, S, M, E', F', S' and M' separated by single spaces. Values E and E' are numbers of eggs, F and F' are grams of flour, S and S' are grams of sugar, and M and M' are centiliters of milk. For each ingredient, X is the amount John has (0 ≤ X ≤ 1000), while X' is the amount needed to make a single cake (1 ≤ X ≤ 1000). The last line of the input contains the number −1 eight times separated by single spaces and should not be processed as a test case.</p>

<h3>Output</h3>
<p>For each test case output a single line with four non-negative integers separated by single spaces, representing the amount of each ingredient John needs to buy, in the same order and units as the input.</p>

<h3>Example</h3>
<pre><strong>Input:</strong><br>2 3 4 5 1 1 1 1<br>3 6 9 0 1 2 3 4<br>-1 -1 -1 -1 -1 -1 -1 -1<br><br><strong>Output:</strong>
3 2 1 0<br>0 0 0 12</pre>