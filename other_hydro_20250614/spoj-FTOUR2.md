<p>After the success of 2nd anniversary (take a look at problem <b>FTOUR</b> for more details), this 3rd year, Travel Agent SPOJ goes on with another discount tour.</p>

<p> The tour will be held on <i>ICPC</i> island, a miraculous one on the Pacific Ocean. We list <b>N</b> places (indexed from 1 to <b>N</b>) where the visitors can have a trip. Each road connecting them has an <i>interest value</i>, and this value can be <i>negative</i> (if there is nothing interesting to view there). Simply, these <b>N</b> places along with the roads connecting them form a <i>tree structure</i>. We will choose <i>two places</i> as the departure and destination of the tour.</p>

<p> Since September is the festival season of local inhabitants, some places are extremely crowded (we call them <i>crowded places</i>). Therefore, the organizer of the excursion hopes the tour will visit <i>at most <b>K</b> crowded places</i> (too tiring to visit many of them) and of course, the <i>total number of interesting value</i> should be maximum.</p>

<p>Briefly, you are given a map of <b>N</b> places, an integer <b>K</b>, and <b>M</b> id numbers of <i>crowded place</i>. Please help us to find the optimal tour. Note that we can visit each place only <i>once</i> (or our customers easily feel bored), also the departure and destination places <i>don't need to be different</i>.</p>

<h3>Input</h3>
<p>There is exactly one case. First one line, containing 3 integers <b>N K M</b>, with 1 &lt;= <b>N</b> &lt;= 200000, 0 &lt;= <b>K</b> &lt;= <b>M</b>, 0 &lt;= <b>M</b> &lt;= <b>N</b>.
</p><p>Next <b>M</b> lines, each line includes an id number of a <i>crowded place</i>.
</p><p>The last (<b>N</b> - 1) lines describe (<b>N</b> - 1) two-way roads connected <b>N</b> places, form <b>a b i</b>, with <b>a, b</b> is the id of 2 places, and <b>i</b> is its <i>interest value</i> (-10000 &lt;= <b>i</b> &lt;= 10000).

</p><h3>Output</h3>
<p>Only one number, the maximum total interest value we can obtain.

</p><h3>Example</h3>

<pre><b>Input:</b>
8 2 3
3
5
7
1 3 1
2 3 10
3 4 -2
4 5 -1
5 7 6
5 6 5
4 8 3


<b>Output:</b>
12
</pre>

<h3>Explanation</h3>
<p>We choose 2 and 6 as the departure and destination place, so the tour will be 2 -&gt; 3 -&gt; 4 -&gt; 5 -&gt; 6, total interest value = 10 + (-2) + (-1) + 5 = 12
<br>
<b>* Added some unofficial cases</b>
</p>