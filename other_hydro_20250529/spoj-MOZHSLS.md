<p>After solving the problem ¡°<strong><strong><strong>MOZHSLM</strong></strong></strong>¡± Sharmeen become familiar with subsequence and somehow become interested in substring. Instead of learning more about substring she started asking some ludicrous questions to Mozahid about substring. Become tired of answering Sharmeen¡¯s ludicrous questions Mozahid gives Sharmeen another problem which is slightly harder than the previous one. Mozahid will give Sharmeen a string of lowercase English letters and some queries. In each query he will give her a substring of that string. Sharmeen has to answer how many different subsequence of ¡®<strong>sms</strong>¡¯ exists in that substring. Can you help Sharmeen solving this problem?</p>
<h3>Input</h3>
<p>Given a string of lowercase English letters of length N( 1 &lt;= N &lt;= 10^5 ) in first line. In the second line given an integer Q( 1 &lt;= Q &lt;= 10^5 ), which is the number of queries. In each query you will be given two integer L , R ( 1 &lt;= L &lt;= R &lt;= N ). L is the starting position of the substring and R is the ending position of the substring( 1 based position ).</p>
<h3>Output</h3>
<p>For each query you have to output an integer in one line which is the number of different subsequence of ¡®sms¡¯ in that substring.</p>
<p>&nbsp;</p>
<p><strong>N.B.</strong> Substring is a consecutive sequence of characters of a string. Where subsequence not necessarily need to be consecutive. But for both you have to maintain the order. For clearance ¡®skmjssm¡¯ has 2 different subsequence of ¡®sms¡¯.&nbsp; {1,3,5} &amp; {1,3,6} ( 1 based position ). For better understanding see the sample input output.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>sasmasamsas</p><p>3</p><p>1 6</p><p>3 9</p>8 11

<strong>Output:</strong>
<p>2</p><p>4</p>0</pre>
<p>[ This problem originally written by MD. Mozahidul Islam Bhuiyan(kissu_pari_na) ]</p>