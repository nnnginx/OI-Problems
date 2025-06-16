<p>Mirko lives in a small town with a harbour: once in a blue moon a ship passes by. However, to this day Mirko remembers the day when all the ships who had ever visited the harbour showed up. He denoted this day by index 1. Many days have passed since, but Mirko noted each day when at least one ship visited the harbour, naming these days entertaining. Additionally, Mirko has noticed that each ship visits the harbour periodically, at regular intervals. For instance, an interval of length 3 implies that some ship visited the harbour on days 1, 4, 7, 10 etc.</p>

<p>Given Mirko¡¯s list of entertaining days (including today which is considered to be an entertaining day as well), compute the minimum possible number of ships visiting his harbour.</p>

<p>Notes: All entertaining days appear on Mirko¡¯s list. It is guaranteed that the given data is consistent - in other words, a solution will always exist.</p>

<h3>Input</h3>
<p>The first line of input contains an integer N (2 ¡Ü N ¡Ü 5000), the number of entertaining days. The following N lines contain indices of entertaining days, one per line, in ascending order. The first and the last indices, representing the day from which Mirko started monitoring harbour traffic and today, respectively, will always appear on the list. The first index will always be 1, and the last one (index of today) will be less than 109.</p>

<h3>Output</h3>
<p>The first and only line of output must contain the required minimum number of ships.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
5
1
7
10
13
19

<strong>Output:</strong>
2</pre>