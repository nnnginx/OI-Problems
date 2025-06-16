<p> As you might already know, Ada the Ladybug is a farmer. She grows
vegetables in a long furrow. All of the vegetables have some height. Local
politicians tax small vegetables, but as the furrow is very long, they always
tax just a part of it. 

</p><p> The taxes always have some limit on height. They are calculated very
simply: Tax collectors multiply the heights of all vegetables, which are
lesser or equal to limit and are on desired segment.

</p><p> The taxes might be very high so tax collectors just round their income and
take only <b>1000000007</b> (<b>10<sup>9</sup>+7</b>) banknotes. They are very kind, so they always leave
the rest to Ada. She is interested in how much they will leave her.

</p><p><b>NOTE:</b> If none of the vegeteble is lesser/equal to given limit, Ada is
left with symbolical 1 "money".



</p><h3>Input</h3>

<p>The first line contains an integer <b> 1 ¡Ü N, Q ¡Ü 3*10<sup>5</sup></b>,
the number of vegetables Ada grows and the number of times the tax collectors
come.

</p><p>The second line contains <b>N</b> integers <b>1 ¡Ü A<sub>i</sub> ¡Ü
    3*10<sup>5</sup></b>, the heights of vegetables.

</p><p>The next <b>Q</b> lines contains three integers <b>0 ¡Ü L ¡Ü R &lt; N</b>,
the left and right vegetables of segment and <b>1¡Ü H ¡Ü
3*10<sup>5</sup></b>, the limit.


</p><h3>Output</h3>

Print a single line for each query with the number of money Ada will be left with
after each tax collecting.

<h3>Example Input</h3>
<pre>10 6
1 2 3 4 5 10 9 8 7 6
5 5 5
0 2 3
0 9 9
4 8 8
2 4 11
2 2 3
</pre>
<h3>Example Output</h3>
<pre>1
6
362880
280
60
3
</pre>