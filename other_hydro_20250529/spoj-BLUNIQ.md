<p>In Lapak City, every tourist is given a unique code based on their favorite number. If their favorite number is already used as a unique code, that tourist will be given the smallest unused unique code that is larger than his favorite number. For example, a tourist with 42 as his favorite number visits Lapak City. However, unique code 42 is already used. So that tourist is given the unique code 43. If 43 is also used, then that tourist is given the unique code 44, etc.</p>
<p>Every tourist that leaves Lapak City will delete their unique code, that means their code can be used for other newcomer if needed. Continuing the previous example, if the tourist with unique code 43 left Lapak City, and a tourist with favorite number 43 enters, that new tourist will be given the unique code 43.</p>
<p>Initially, all code is unused and no tourist is in Lapak City. On one day, there are N tourist event on Lapak City. Help Lapak City to determine unique code for the tourist.</p>
<h3>Input</h3>
<p>First line of input is N, the number of event (1 <span style="text-decoration: underline;">&lt;</span>&nbsp;N <span style="text-decoration: underline;">&lt;</span>&nbsp;100000). Next N lines contain the events. For every tourist that visits Lapak City, the input is "1 x", with x is the favorite number of that tourist (1 <span style="text-decoration: underline;">&lt;</span>&nbsp;x <span style="text-decoration: underline;">&lt;</span>&nbsp;1 000 000 000). For every tourist that leaves Lapak City, the input is "2 x", with x is the unique code of that tourist.</p>
<h3>Output</h3>
<p>For each visiting tourist, output their unique code.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
1 42
1 42
1 43
2 43
1 42

<strong>Output:</strong>
42
43
44
43
</pre>