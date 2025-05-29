<p>The Kingdom of Gridland contains <strong>P</strong> provinces. Each province is defined as a <strong>2 x N</strong> grid where each cell in the grid represents a city. Every cell in the grid contains a single lowercase character denoting the first character of the city name corresponding to that cell.</p>

<p>From a city with the coordinates <strong>(i, j)</strong>, it is possible to move to any of the following cells in unit of time, provided that the destination cell is inside the grid:</p>

<li><strong>(i + 1, j)</strong></li>
<li><strong>(i, j + 1)</strong></li>
<li><strong>(i - 1, j)</strong></li>
<li><strong>(i, j - 1)</strong></li>

<p>A knight wants to visit all the cities in Gridland. He can start his journey in any city and immediately stops his journey after having visited each city at least once. Moreover, he always plans his journey in such a way that the total time required to complete it is minimum.</p>

<p>After completing his tour of each province, the knight forms a string by concatenating the characters of all the cells in his path. How many distinct strings can he form in each province?</p>

<h3>Input</h3>
<p>The first line contains a single integer <strong>P</strong>, denoting the number of provinces. The <strong>3 * P</strong>  subsequent lines describe each province. The first line contains an integer <strong>N</strong>, denoting the number of columns in the province. Each of the next two lines contains a string <strong>S</strong>, of length <strong>N</strong> and consisting of only lowercase letters denoting the characters for the first and second row of the province.</p>

<h3>Constraints</h3>
<li><strong>1 ¡Ü P ¡Ü 15</strong></li>
<li><strong>1 ¡Ü N ¡Ü 600</strong></li>

<h3>Output</h3>
<p>For each province, print the number of distinct strings the knight can form on a new line.</p>
<h3>Sample Input</h3>
<pre>3
1
a
a
3
dab
abd
5
ababa
babab
</pre>
<h3>Sample Output</h3>
<pre>1
8
2
</pre>

<h3>Explanation</h3>
For the second province, here are all possible unique strings that can be formed: <i>abdbad, adabdb, badabd, bdbada, dababd, dabdba, dbabad, and dbadab</i>.

<h3>Reference</h3>
<a href="https://www.hackerrank.com/challenges/gridland-provinces/problem">HackerRank - Gridland Provinces</a>