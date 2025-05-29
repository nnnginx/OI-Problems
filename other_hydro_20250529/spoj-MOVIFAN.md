<p><span style="font-size: small;">Alice is a cinephile. He wanted to watch a recently released movie. There are many movie shows whose start time and length are given.Your task is to help Alice count the number of ways he can watch the movie. Since he is a cinephile, he can watch many shows as long as they do not overlap.</span></p>
<h3>Input</h3>
<p><span style="font-size: small;">First line contains an integer t denotine number of test cases.</span></p>
<p><span style="font-size: small;">Each test case contains n,l denoting number of shows and length of the shows.</span></p>
<p><span style="font-size: small;">n integer follows denoting start time of show.</span></p>
<p>&nbsp;</p>
<p><span style="font-size: x-small;">1&lt;=t&lt;=10</span></p>
<p style="text-align: justify;"><span style="font-size: x-small;">1&lt;=n,l&lt;=</span><span style="font-family: Arial, Helvetica, sans-serif; color: #666666;"><span style="font-size: 12px;"><strong>300000</strong></span></span></p>
<p><span style="font-size: x-small;"><br></span></p>
<h3>Output</h3>
<p style="text-align: justify;"><span style="font-size: small;">Print the number of ways Alice can watch shows if he want to watch atleast one show modulo 1000000007</span><span style="font-size: small;"><span style="font-family: Arial, sans-serif; color: #666666;">.</span></span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3</pre>
<pre>3 4</pre>
<pre>3 8 12</pre>
<pre>3 1</pre>
<pre>1 2 3</pre>
<pre>3 3</pre>
<pre>3 5 9

<strong>Output:</strong>
7</pre>
<pre>7</pre>
<pre>5</pre>
<pre><span style="font-size: small;">For testcase1 ,Alice can watch 1 show in 3 ways,2 shows in 3 ways and 3 show in 1 way total ways=7</span></pre>
<pre><span style="font-size: small;">For test case3 Alice can watch 1 show in 3 ways, 2 shows in 2 ways ,total ways=5</span></pre>