<p><strong>[ The original version of this problem (in Spanish) can be found at <a title="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf" href="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf">http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf</a> ]</strong></p>
<p>Paul Erdös was a Hungarian mathematician of the 20th century who reached the highest levels of recognition. So much so that it is considered an honour not only having written an article with him, but also having shared authorship of a publication with one of his co-authors. Moreover, writing an article with someone who wrote an article with someone who wrote an article with Erdös is an important aspiration of many young researchers.</p>
<p>A natural consequence of such honours assignment, at least within the context of formal sciences, is the emergence of <em>Erdös numbers</em>. Erdös is the only person with an Erdös number of <strong>0</strong>, and for any other person <strong>p</strong>, his/her Erdös number <strong>n</strong> is defined by the shortest sequence of articles <strong>a<sub>1</sub>, ... , a<sub>n</sub></strong> such that Erdös is one of the authors of article <strong>a<sub>1</sub></strong>, <strong>p</strong> is one the authors of article <strong>a<sub>n</sub></strong>, and every pair of consecutive articles <strong>a<sub>i</sub></strong> and <strong>a</strong><sub>i+1 </sub>(for <strong>i = 1, 2, ..., N-1</strong>)&nbsp;have at least one author in common. If no sequence of articles linking Erdös and <strong>p</strong> exists, we shall say that <strong>p</strong>'s Erdös number is <em>undefined</em>.</p>
<p>Your task in this problem is to compute Erdös numbers based only on a corpus of articles and authors given as input. Unfortunately, current science demands scientists to increase very rapidly the number of articles they write, causing both the total number of articles and the number of authors per article to be huge. Of course, this reality is an obstacle that a correct solution to this problem should be able to handle.</p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Paul Erdös was a Hungarian mathematician of the 20th century who reached the highest levels of recognition. So much so that it is considered an honor not only having written an article with him, but also having shared autorship of a publication with one of his co-authors. Moreover, writing an article with someone who wrote an article with someone who wrote an article with Erdös is an important aspiration of many young researchers.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">A natural consequence of such honors assignment, at least within the context of formal sciences, is the emergence of Erdös numbers. Erdös is the only person with an Erdös number of 0, and for any other person p, his/her Erdös number n is defined by the shortest sequence of articles a_1, ... , a_n such that Erdös is one of the authors of article a_1, p is one the authors of article a_n, and every pair of consecutive articles a_i and a_{i+1} have at least one author in common. If no sequence of articles linking Erdös and p exists, we shall say that p's Erdös number is undefined.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">
<p>Your task in this problem is to compute Erdös numbers based only on a corpus of articles and authors given as input. Unfortunately, current science demands scientists to increase very rapidly the number of articles they write, causing both the total number of articles and the number of authors per article to be huge. Of course, this reality is an obstacle that a correct solution to this problem should be able to handl</p>
<p>&nbsp;</p>
</div>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains two integers <strong>A</strong> and <strong>N</strong>, where <strong>A</strong> represents the number of articles in the corpus to be analysed and <strong>N</strong> the number of people who appear in it (where <strong>2 ≤&nbsp;A, N&nbsp;</strong><strong>≤</strong><strong>&nbsp;10<sup>5</sup></strong>). People are identified with integers between <strong>1</strong> and <strong>N</strong>, and Erdös will always be the person identified with number <strong>1</strong>.</p>
<p>Each of the following <strong>A</strong> lines describes an article. Each of these lines begins with an integer <strong>C</strong> representing the number of authors of the article (<strong>2&nbsp;</strong><strong>≤</strong><strong>&nbsp;C&nbsp;</strong><strong>≤</strong><strong>&nbsp;10<sup>5</sup></strong>), and then there are <strong>C</strong> distinct integers <strong>P<sub>1</sub>, P<sub>2</sub>, ... , P<sub>C</sub></strong> representing the identifiers of the authors of the article (<strong>1&nbsp;</strong><strong>≤</strong><strong>&nbsp;P<sub>i</sub>&nbsp;</strong><strong>≤</strong><strong>&nbsp;N</strong>&nbsp;for <strong>i = 1, 2, ... , C</strong>). The sum of the number of authors over all articles does not exceed <strong>10<sup>5</sup></strong>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case you must print three integers <strong>D</strong>, <strong>M</strong> and <strong>S</strong>, where <strong>D</strong> represents the number of people on the corpus who have a well-defined Erdös number, <strong>M</strong> is the maximum Erdös number of one of those people and <strong>S</strong> is the sum of all the Erdös numbers belonging to people who have a well-defined Erdös number.</p>
<p>&nbsp;</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">3 5
2 1 5
3 5 2 3
3 3 2 4</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">5 3 8</span></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">5 11
2 10 11
4 1 3 5 7
6 2 3 4 5 6 7
4 3 5 7 9
3 8 1 5</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">9 2 12</span></pre>
<h3>Example 3</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">6 31
9 1 2 3 15 20 25 30 9 10
10 2 25 7 9 3 11 12 13 14 4
10 11 12 13 14 4 16 17 18 19 5
2 5 7
9 21 22 23 24 26 27 28 29 7
3 22 6 21</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">29 4 63</span><span style="white-space: normal;">&nbsp;</span></pre>