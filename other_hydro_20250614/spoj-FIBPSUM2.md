<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.css" integrity="sha384-wITovz90syo1dJWVh32uuETPVEtGigN07tkttEqPv+uR2SE/mbQcG7ATL28aI9H0" crossorigin="anonymous">
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/katex.min.js" integrity="sha384-/y1Nn9+QQAipbNQWU65krzJralCnuOasHncUFXGkdwntGeSvQicrYkiUBwsgUqc1" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/KaTeX/0.7.1/contrib/auto-render.min.js"></script>
<script>// <![CDATA[
document.addEventListener("DOMContentLoaded", function(){
  renderMathInElement(
    document.body,{
      delimiters: [
        {left: "$$", right: "$$", display: true},
        {left: "$", right: "$", display: false}]})});
// ]]></script>
<p><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">This problem is a harder version of <a href="../../FIBPWSUM/">FIBPWSUM</a>.</span></p>
<p><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">The Fibonacci numbers is defined by</span></p>
<p><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">$$ f_0=0, f_1=1, $$</span></p>
<p><span style="font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; color: #555555;"><span style="font-size: 14px;">and</span></span></p>
<p><span style="font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; color: #555555;"><span style="font-size: 14px;">$$ f_n = f_{n-1}+f_{n-2} $$</span></span></p>
<p><span style="font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; color: #555555;"><span style="font-size: 14px;">for $n &gt; 1$.&nbsp;</span></span></p>
<p><span style="font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; color: #555555;"><span style="font-size: 14px;">&nbsp;</span></span><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">Given three integers $N$, $C$ and $K$</span><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">, compute the summation</span></p>
<p><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">$$ \sum_{n=0}^N f_{Cn}^K. $$</span></p>
<p><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">&nbsp;</span><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">Since the answer can be huge, output it modulo $10^9+7$</span><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">.</span></p>
<h3>Input</h3>
<p><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">The first line contains an integer $T$</span><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">, denoting the number of test cases. Each test case contains three space separated integers in the order: $N$, $C$&nbsp;</span><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">and $K$</span><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">.</span></p>
<h3>Constraints</h3>
<p><span style="box-sizing: border-box; font-weight: 700; color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;"> </span></p>
<li style="box-sizing: border-box;"><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">$1 \leq T \leq 100$</span></li>
<li style="box-sizing: border-box;"><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">$1 \leq N, C \leq 10^{18}$</span></li>
<li style="box-sizing: border-box;"><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">$1 \leq K \leq 10^5$</span></li>
<h3>Output</h3>
<p><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">For each test case, output a single line in the format&nbsp;</span><em>¡°Case X: Y¡±</em><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">&nbsp;without the quotes. Here,&nbsp;</span><span style="box-sizing: border-box; font-weight: 700; color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">X</span><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">&nbsp;is the case number and&nbsp;</span><span style="box-sizing: border-box; font-weight: 700; color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">Y</span><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">&nbsp;is the desired answer denoting the sum of the series.</span></p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>5<br>10 1 1<br>5 2 2<br>3 3 4<br>1000000007 7 9<br>996969696969696 9 6</pre>
<pre><strong>Output:<br></strong>Case 1: 143<br>Case 2: 3540<br>Case 3: 1340448<br>Case 4: 880410497<br>Case 5: 689328397</pre>
<h3>Credits</h3>
<ul>
<li><span style="font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; color: #555555;"><span style="font-size: 14px;"><a href="../../../users/sgtlaugh/">sgtlaugh</a> - <a href="../FIBPWSUM/">FIBPWSUM</a></span></span></li>
<li><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;"><a href="http://acm.zju.edu.cn/onlinejudge/showProblem.do?problemCode=3774">ZOJ 3774. Power of Fibonacci</a></span></li>
</ul>
<h3>Information</h3>
<p><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">There are two test files. The first file is randomly generated while the second file is not.</span></p>
<p><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;">@Speed Adicts: My solution runs in 1.94s. (approx less than 1s per file)</span></p>
<p><span style="font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; color: #555555;"><span style="font-size: 14px;"><br></span></span></p>
<p><span style="font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; color: #555555;"><span style="font-size: 14px;"><br></span></span></p>
<p><span style="color: #555555; font-family: &quot;Open Sans&quot;, &quot;Helvetica Neue&quot;, Helvetica, Arial, sans-serif; font-size: 14px;"><br></span></p>