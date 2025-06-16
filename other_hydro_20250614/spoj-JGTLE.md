<p>Ananta Jalil is a multi talented person. He can make any task possible which is impossible to others. Recently he has learned programming basic. In a problem, he submitted the following solution:</p>

<pre>#include &lt;stdio.h&gt;

int main()
{
    int t;
    scanf("%d", &amp;t);
    for(int tc = 1; tc &lt;= t; ++tc) {
        int a, b, c;
        scanf("%d %d %d", &amp;a, &amp;b, &amp;c);
        long long result = 0;
        for(int i = 1; i &lt;= a; ++i) {
            for(int j = 1; j &lt;= b; ++j) {
                for(int k = 1; k &lt;= c; ++k) {
                    result += j * k;
                }
            }
        }
        printf("Case %d: %lld\n", tc, result);
    }
    return 0;
}
</pre>

<p>But he got TLE (Time Limit Exceeded) as he is novice in programming. That¡¯s why his solution was not efficient. So you are here to write an optimized solution for Jalil which will give the same output.</p>

<h3>Input</h3>
<p>The first line of input will contain a positive integer T denoting the number of test cases.</p>
<p>In each test case, there will be 3 positive integers a, b and c.</p>

<h3>Constraints</h3>
<ul>
<li>T &lt;= 1000</li>
<li>a &lt;= 30</li>
<li>b &lt;= 100000</li>
<li>c &lt;= 10000</li>
</ul>

<h3>Output</h3>
<p>For each test case, print the output as same as the above program.</p>

<h3>Example</h3>
<h4>Input</h4>
<pre>3
1 4 3
3 4 2
143 342 777</pre>

<h4>Output</h4>
<pre>Case 1: 60
Case 2: 90
Case 3: 2535110464887</pre>