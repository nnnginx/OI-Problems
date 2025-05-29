<p>Given polynomial of degree d, f(x)=c<sub>0</sub>+c<sub>1</sub>x+c<sub>2</sub>x<sup>2</sup>+c<sub>3</sub>x<sup>3</sup>+...+c<sub>d</sub>x<sup>d</sup></p>
<p>For each polynomial f(x) there exists polynomial g(x) such that:</p>
<p>-&gt; f(x)=g(x)-g(x-1) for each integer x</p>
<p>-&gt; g(0)=0</p>
<p>Your task is to calculate polynomial h(x)=g(x)/x</p>
<p>(Note : degree of polynomial h(x) = degree of polynomial f(x))</p>
<h3>Input</h3>
<p>The first line of input contain an integer T, T is number of test cases (0&lt;T¡Ü10<sup>4</sup>)</p>
<p>Each test case consist of 2 lines:</p>
<p>- First line of the test case contain an integer d, d is degree of polynomial f(x) (0¡Üd¡Ü18)</p>
<p>- Next line contains d+1 integers c<sub>0</sub>,c<sub>1</sub>,...,c<sub>d</sub>, separated by space,&nbsp;represent the coefficient of polynomial f(x)&nbsp;(-2<sup>31</sup>&lt;c<sub>0</sub>,c<sub>1</sub>,...,c<sub>d</sub>&lt;2<sup>31</sup>&nbsp;and c<sub>d</sub>¡Ù0)</p>
<h3>Output</h3>
<p>For each test case, output the coefficient of polynomial h(x) separated by space. Each coefficient of polynomial h(x) is guaranteed to be an integer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5</pre>
<pre>0</pre>
<pre>13</pre>
<pre>1</pre>
<pre>-1 2</pre>
<pre>1</pre>
<pre>0 2</pre>
<pre>2</pre>
<pre>2 -5 9</pre>
<pre>3</pre>
<pre>23 9 21 104

<strong>Output:</strong>
13</pre>
<pre>0 1</pre>
<pre>1 1</pre>
<pre>1 2 3</pre>
<pre>31 41 59 26</pre>
<pre><span style="font-weight: bold;"><br></span></pre>
<pre><span style="font-weight: bold;">---------------------------------------------------------------</span></pre>
<pre><strong>Explanation for the first test case :</strong></pre>
<pre>f(x)=13</pre>
<pre>g(x) that satisfy: g(x)-g(x-1)=f(x)=13 and g(0)=0 is: g(x)=13x</pre>
<pre>h(x)=g(x)/x so h(x)=13</pre>
<pre>output : 13</pre>
<pre><strong>Explanation for the second test case :</strong></pre>
<pre>f(x)=-1+2x</pre>
<pre>g(x) that satisfy: g(x)-g(x-1)=f(x)=-1+2x and g(0)=0 is: g(x)=x<sup>2</sup></pre>
<pre>h(x)=g(x)/x so h(x)=x=0+1x</pre>
<pre>output : 0 1</pre>
<pre><strong>Explanation for the third test case :</strong></pre>
<pre>f(x)=0+2x</pre>
<pre>g(x) that satisfy: g(x)-g(x-1)=f(x)=2x and g(0)=0 is: g(x)=x+x<sup>2</sup></pre>
<pre>h(x)=g(x)/x so h(x)=1+1x</pre>
<pre>output : 1 1</pre>
<pre>---------------------------------------------------------------</pre>
<p>&nbsp;</p>
<p><strong>See also:</strong> <a title="TJANDRA" href="../TJANDRA/" target="_blank">Another problem added by Tjandra Satria Gunawan</a></p>